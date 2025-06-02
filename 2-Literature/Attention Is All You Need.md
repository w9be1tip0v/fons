---
title: "Attention Is All You Need"
source: "https://arxiv.org/html/1706.03762v7"
author: "Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Łukasz Kaiser, Illia Polosukhin"
published: "2017"
created: 2025-06-03
description: "Seminal paper introducing the Transformer architecture based entirely on attention mechanisms, revolutionizing NLP and machine learning."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - role/author
  - target/starterkit
---
arXiv:1706.03762v7 \[cs.CL\] 02 Aug 2023

Provided proper attribution is provided, Google hereby grants permission to reproduce the tables and figures in this paper solely for use in journalistic or scholarly works.

Ashish Vaswani  
Google Brain  
avaswani@google.com  
&Noam Shazeer <sup>1</sup> <sup>1</sup> footnotemark: 1  
Google Brain  
noam@google.com  
&Niki Parmar <sup>1</sup> <sup>1</sup> footnotemark: 1  
Google Research  
nikip@google.com  
&Jakob Uszkoreit <sup>1</sup> <sup>1</sup> footnotemark: 1  
Google Research  
usz@google.com  
&Llion Jones <sup>1</sup> <sup>1</sup> footnotemark: 1  
Google Research  
llion@google.com  
&Aidan N. Gomez <sup>1</sup> <sup>1</sup> footnotemark: 1  
University of Toronto  
aidan@cs.toronto.edu &Łukasz Kaiser <sup>1</sup> <sup>1</sup> footnotemark: 1  
Google Brain  
lukaszkaiser@google.com  
&Illia Polosukhin <sup>1</sup> <sup>1</sup> footnotemark: 1  
illia.polosukhin@gmail.com  
Equal contribution. Listing order is random. Jakob proposed replacing RNNs with self-attention and started the effort to evaluate this idea. Ashish, with Illia, designed and implemented the first Transformer models and has been crucially involved in every aspect of this work. Noam proposed scaled dot-product attention, multi-head attention and the parameter-free position representation and became the other person involved in nearly every detail. Niki designed, implemented, tuned and evaluated countless model variants in our original codebase and tensor2tensor. Llion also experimented with novel model variants, was responsible for our initial codebase, and efficient inference and visualizations. Lukasz and Aidan spent countless long days designing various parts of and implementing tensor2tensor, replacing our earlier codebase, greatly improving results and massively accelerating our research. Work performed while at Google Brain.Work performed while at Google Research.

###### Abstract

The dominant sequence transduction models are based on complex recurrent or convolutional neural networks that include an encoder and a decoder. The best performing models also connect the encoder and decoder through an attention mechanism. We propose a new simple network architecture, the Transformer, based solely on attention mechanisms, dispensing with recurrence and convolutions entirely. Experiments on two machine translation tasks show these models to be superior in quality while being more parallelizable and requiring significantly less time to train. Our model achieves 28.4 BLEU on the WMT 2014 English-to-German translation task, improving over the existing best results, including ensembles, by over 2 BLEU. On the WMT 2014 English-to-French translation task, our model establishes a new single-model state-of-the-art BLEU score of 41.8 after training for 3.5 days on eight GPUs, a small fraction of the training costs of the best models from the literature. We show that the Transformer generalizes well to other tasks by applying it successfully to English constituency parsing both with large and limited training data.

## 1 Introduction

Recurrent neural networks, long short-term memory \[\] and gated recurrent \[\] neural networks in particular, have been firmly established as state of the art approaches in sequence modeling and transduction problems such as language modeling and machine translation \[, , \]. Numerous efforts have since continued to push the boundaries of recurrent language models and encoder-decoder architectures \[, , \].

Recurrent models typically factor computation along the symbol positions of the input and output sequences. Aligning the positions to steps in computation time, they generate a sequence of hidden states $h_{t}$ , as a function of the previous hidden state $h_{t-1}$ and the input for position $t$ . This inherently sequential nature precludes parallelization within training examples, which becomes critical at longer sequence lengths, as memory constraints limit batching across examples. Recent work has achieved significant improvements in computational efficiency through factorization tricks \[\] and conditional computation \[\], while also improving model performance in case of the latter. The fundamental constraint of sequential computation, however, remains.

Attention mechanisms have become an integral part of compelling sequence modeling and transduction models in various tasks, allowing modeling of dependencies without regard to their distance in the input or output sequences \[, \]. In all but a few cases \[\], however, such attention mechanisms are used in conjunction with a recurrent network.

In this work we propose the Transformer, a model architecture eschewing recurrence and instead relying entirely on an attention mechanism to draw global dependencies between input and output. The Transformer allows for significantly more parallelization and can reach a new state of the art in translation quality after being trained for as little as twelve hours on eight P100 GPUs.

## 2 Background

The goal of reducing sequential computation also forms the foundation of the Extended Neural GPU \[\], ByteNet \[\] and ConvS2S \[\], all of which use convolutional neural networks as basic building block, computing hidden representations in parallel for all input and output positions. In these models, the number of operations required to relate signals from two arbitrary input or output positions grows in the distance between positions, linearly for ConvS2S and logarithmically for ByteNet. This makes it more difficult to learn dependencies between distant positions \[\]. In the Transformer this is reduced to a constant number of operations, albeit at the cost of reduced effective resolution due to averaging attention-weighted positions, an effect we counteract with Multi-Head Attention as described in section .

Self-attention, sometimes called intra-attention is an attention mechanism relating different positions of a single sequence in order to compute a representation of the sequence. Self-attention has been used successfully in a variety of tasks including reading comprehension, abstractive summarization, textual entailment and learning task-independent sentence representations \[, , , \].

End-to-end memory networks are based on a recurrent attention mechanism instead of sequence-aligned recurrence and have been shown to perform well on simple-language question answering and language modeling tasks \[\].

To the best of our knowledge, however, the Transformer is the first transduction model relying entirely on self-attention to compute representations of its input and output without using sequence-aligned RNNs or convolution. In the following sections, we will describe the Transformer, motivate self-attention and discuss its advantages over models such as \[, \] and \[\].

## 3 Model Architecture

![Refer to caption](https://arxiv.org/html/extracted/1706.03762v7/Figures/ModalNet-21.png)

Figure 1: The Transformer - model architecture.

Most competitive neural sequence transduction models have an encoder-decoder structure \[, , \]. Here, the encoder maps an input sequence of symbol representations $(x_{1},...,x_{n})$ to a sequence of continuous representations $\mathbf{z}=(z_{1},...,z_{n})$ . Given $\mathbf{z}$ , the decoder then generates an output sequence $(y_{1},...,y_{m})$ of symbols one element at a time. At each step the model is auto-regressive \[\], consuming the previously generated symbols as additional input when generating the next.

The Transformer follows this overall architecture using stacked self-attention and point-wise, fully connected layers for both the encoder and decoder, shown in the left and right halves of Figure , respectively.

### 3.1 Encoder and Decoder Stacks

##### Encoder:

The encoder is composed of a stack of $N=6$ identical layers. Each layer has two sub-layers. The first is a multi-head self-attention mechanism, and the second is a simple, position-wise fully connected feed-forward network. We employ a residual connection \[\] around each of the two sub-layers, followed by layer normalization \[\]. That is, the output of each sub-layer is $\mathrm{LayerNorm}(x+\mathrm{Sublayer}(x))$ , where $\mathrm{Sublayer}(x)$ is the function implemented by the sub-layer itself. To facilitate these residual connections, all sub-layers in the model, as well as the embedding layers, produce outputs of dimension $d_{\text{model}}=512$ .

##### Decoder:

The decoder is also composed of a stack of $N=6$ identical layers. In addition to the two sub-layers in each encoder layer, the decoder inserts a third sub-layer, which performs multi-head attention over the output of the encoder stack. Similar to the encoder, we employ residual connections around each of the sub-layers, followed by layer normalization. We also modify the self-attention sub-layer in the decoder stack to prevent positions from attending to subsequent positions. This masking, combined with fact that the output embeddings are offset by one position, ensures that the predictions for position $i$ can depend only on the known outputs at positions less than $i$ .

### 3.2 Attention

An attention function can be described as mapping a query and a set of key-value pairs to an output, where the query, keys, values, and output are all vectors. The output is computed as a weighted sum of the values, where the weight assigned to each value is computed by a compatibility function of the query with the corresponding key.

#### 3.2.1 Scaled Dot-Product Attention

We call our particular attention "Scaled Dot-Product Attention" (Figure ). The input consists of queries and keys of dimension $d_{k}$ , and values of dimension $d_{v}$ . We compute the dot products of the query with all keys, divide each by $\sqrt{d_{k}}$ , and apply a softmax function to obtain the weights on the values.

In practice, we compute the attention function on a set of queries simultaneously, packed together into a matrix $Q$ . The keys and values are also packed together into matrices $K$ and $V$ . We compute the matrix of outputs as:

<table><tbody><tr><td></td><td><math><semantics><mrow><mrow><mi>Attention</mi> <mo>⁢</mo> <mrow><mo>(</mo><mi>Q</mi><mo>,</mo><mi>K</mi><mo>,</mo><mi>V</mi><mo>)</mo></mrow></mrow> <mo>=</mo> <mrow><mi>softmax</mi> <mo>⁢</mo> <mrow><mo>(</mo><mfrac><mrow><mi>Q</mi> <mo>⁢</mo> <msup><mi>K</mi> <mi>T</mi></msup></mrow> <msqrt><msub><mi>d</mi> <mi>k</mi></msub></msqrt></mfrac><mo>)</mo></mrow> <mo>⁢</mo> <mi>V</mi></mrow></mrow> <annotation-xml><apply><apply><ci>Attention</ci> <vector><ci>𝑄</ci> <ci>𝐾</ci> <ci>𝑉</ci></vector></apply> <apply><ci>softmax</ci> <apply><apply><ci>𝑄</ci> <apply><csymbol>superscript</csymbol> <ci>𝐾</ci> <ci>𝑇</ci></apply></apply> <apply><apply><csymbol>subscript</csymbol> <ci>𝑑</ci> <ci>𝑘</ci></apply></apply></apply> <ci>𝑉</ci></apply></apply></annotation-xml> <annotation>\mathrm{Attention}(Q,K,V)=\mathrm{softmax}(\frac{QK^{T}}{\sqrt{d_{k}}})V</annotation> <annotation>roman_Attention ( italic_Q, italic_K, italic_V ) = roman_softmax ( divide start_ARG italic_Q italic_K start_POSTSUPERSCRIPT italic_T end_POSTSUPERSCRIPT end_ARG start_ARG square-root start_ARG italic_d start_POSTSUBSCRIPT italic_k end_POSTSUBSCRIPT end_ARG end_ARG ) italic_V</annotation></semantics></math></td><td></td><td rowspan="1"><span>(1)</span></td></tr></tbody></table>

The two most commonly used attention functions are additive attention \[\], and dot-product (multiplicative) attention. Dot-product attention is identical to our algorithm, except for the scaling factor of $\frac{1}{\sqrt{d_{k}}}$ . Additive attention computes the compatibility function using a feed-forward network with a single hidden layer. While the two are similar in theoretical complexity, dot-product attention is much faster and more space-efficient in practice, since it can be implemented using highly optimized matrix multiplication code.

While for small values of $d_{k}$ the two mechanisms perform similarly, additive attention outperforms dot product attention without scaling for larger values of $d_{k}$ \[\]. We suspect that for large values of $d_{k}$ , the dot products grow large in magnitude, pushing the softmax function into regions where it has extremely small gradients <sup>1</sup> <sup>1</sup> 1 To illustrate why the dot products get large, assume that the components of $q$ and $k$ are independent random variables with mean $00$ and variance $1$ . Then their dot product, $q\cdot k=\sum_{i=1}^{d_{k}}q_{i}k_{i}$ , has mean $00$ and variance $d_{k}$ .. To counteract this effect, we scale the dot products by $\frac{1}{\sqrt{d_{k}}}$ .

#### 3.2.2 Multi-Head Attention

![Refer to caption](https://arxiv.org/html/extracted/1706.03762v7/Figures/ModalNet-19.png)

Figure 2: (left) Scaled Dot-Product Attention. (right) Multi-Head Attention consists of several attention layers running in parallel.

Instead of performing a single attention function with $d_{\text{model}}$ -dimensional keys, values and queries, we found it beneficial to linearly project the queries, keys and values $h$ times with different, learned linear projections to $d_{k}$ , $d_{k}$ and $d_{v}$ dimensions, respectively. On each of these projected versions of queries, keys and values we then perform the attention function in parallel, yielding $d_{v}$ -dimensional output values. These are concatenated and once again projected, resulting in the final values, as depicted in Figure .

Multi-head attention allows the model to jointly attend to information from different representation subspaces at different positions. With a single attention head, averaging inhibits this.

|  | $\displaystyle\mathrm{MultiHead}(Q,K,V)$ | $\displaystyle=\mathrm{Concat}(\mathrm{head_{1}},...,\mathrm{head_{h}})W^{O}$ |  |
| --- | --- | --- | --- |
|  | $\displaystyle\text{where}~{}\mathrm{head_{i}}$ | $\displaystyle=\mathrm{Attention}(QW^{Q}_{i},KW^{K}_{i},VW^{V}_{i})$ |  |

Where the projections are parameter matrices $W^{Q}_{i}\in\mathbb{R}^{d_{\text{model}}\times d_{k}}$ , $W^{K}_{i}\in\mathbb{R}^{d_{\text{model}}\times d_{k}}$ , $W^{V}_{i}\in\mathbb{R}^{d_{\text{model}}\times d_{v}}$ and $W^{O}\in\mathbb{R}^{hd_{v}\times d_{\text{model}}}$ .

In this work we employ $h=8$ parallel attention layers, or heads. For each of these we use $d_{k}=d_{v}=d_{\text{model}}/h=64$ . Due to the reduced dimension of each head, the total computational cost is similar to that of single-head attention with full dimensionality.

#### 3.2.3 Applications of Attention in our Model

The Transformer uses multi-head attention in three different ways:

- In "encoder-decoder attention" layers, the queries come from the previous decoder layer, and the memory keys and values come from the output of the encoder. This allows every position in the decoder to attend over all positions in the input sequence. This mimics the typical encoder-decoder attention mechanisms in sequence-to-sequence models such as \[, , \].
- The encoder contains self-attention layers. In a self-attention layer all of the keys, values and queries come from the same place, in this case, the output of the previous layer in the encoder. Each position in the encoder can attend to all positions in the previous layer of the encoder.
- Similarly, self-attention layers in the decoder allow each position in the decoder to attend to all positions in the decoder up to and including that position. We need to prevent leftward information flow in the decoder to preserve the auto-regressive property. We implement this inside of scaled dot-product attention by masking out (setting to $-\infty$ ) all values in the input of the softmax which correspond to illegal connections. See Figure .

### 3.3 Position-wise Feed-Forward Networks

In addition to attention sub-layers, each of the layers in our encoder and decoder contains a fully connected feed-forward network, which is applied to each position separately and identically. This consists of two linear transformations with a ReLU activation in between.

<table><tbody><tr><td></td><td><math><semantics><mrow><mrow><mi>FFN</mi> <mo>⁢</mo> <mrow><mo>(</mo><mi>x</mi><mo>)</mo></mrow></mrow> <mo>=</mo> <mrow><mrow><mrow><mi>max</mi> <mo>⁡</mo> <mrow><mo>(</mo><mn>0</mn><mo>,</mo><mrow><mrow><mi>x</mi> <mo>⁢</mo> <msub><mi>W</mi> <mn>1</mn></msub></mrow> <mo>+</mo> <msub><mi>b</mi> <mn>1</mn></msub></mrow><mo>)</mo></mrow></mrow> <mo>⁢</mo> <msub><mi>W</mi> <mn>2</mn></msub></mrow> <mo>+</mo> <msub><mi>b</mi> <mn>2</mn></msub></mrow></mrow> <annotation-xml><apply><apply><ci>FFN</ci> <ci>𝑥</ci></apply> <apply><apply><apply><cn>0</cn> <apply><apply><ci>𝑥</ci> <apply><csymbol>subscript</csymbol> <ci>𝑊</ci> <cn>1</cn></apply></apply> <apply><csymbol>subscript</csymbol> <ci>𝑏</ci> <cn>1</cn></apply></apply></apply> <apply><csymbol>subscript</csymbol> <ci>𝑊</ci> <cn>2</cn></apply></apply> <apply><csymbol>subscript</csymbol> <ci>𝑏</ci> <cn>2</cn></apply></apply></apply></annotation-xml> <annotation>\mathrm{FFN}(x)=\max(0,xW_{1}+b_{1})W_{2}+b_{2}</annotation> <annotation>roman_FFN ( italic_x ) = roman_max ( 0, italic_x italic_W start_POSTSUBSCRIPT 1 end_POSTSUBSCRIPT + italic_b start_POSTSUBSCRIPT 1 end_POSTSUBSCRIPT ) italic_W start_POSTSUBSCRIPT 2 end_POSTSUBSCRIPT + italic_b start_POSTSUBSCRIPT 2 end_POSTSUBSCRIPT</annotation></semantics></math></td><td></td><td rowspan="1"><span>(2)</span></td></tr></tbody></table>

While the linear transformations are the same across different positions, they use different parameters from layer to layer. Another way of describing this is as two convolutions with kernel size 1. The dimensionality of input and output is $d_{\text{model}}=512$ , and the inner-layer has dimensionality $d_{ff}=2048$ .

### 3.4 Embeddings and Softmax

Similarly to other sequence transduction models, we use learned embeddings to convert the input tokens and output tokens to vectors of dimension $d_{\text{model}}$ . We also use the usual learned linear transformation and softmax function to convert the decoder output to predicted next-token probabilities. In our model, we share the same weight matrix between the two embedding layers and the pre-softmax linear transformation, similar to \[\]. In the embedding layers, we multiply those weights by $\sqrt{d_{\text{model}}}$ .

### 3.5 Positional Encoding

Since our model contains no recurrence and no convolution, in order for the model to make use of the order of the sequence, we must inject some information about the relative or absolute position of the tokens in the sequence. To this end, we add "positional encodings" to the input embeddings at the bottoms of the encoder and decoder stacks. The positional encodings have the same dimension $d_{\text{model}}$ as the embeddings, so that the two can be summed. There are many choices of positional encodings, learned and fixed \[\].

In this work, we use sine and cosine functions of different frequencies:

|  | $\displaystyle PE_{(pos,2i)}=sin(pos/10000^{2i/d_{\text{model}}})$ |  |
| --- | --- | --- |
|  | $\displaystyle PE_{(pos,2i+1)}=cos(pos/10000^{2i/d_{\text{model}}})$ |  |

where $pos$ is the position and $i$ is the dimension. That is, each dimension of the positional encoding corresponds to a sinusoid. The wavelengths form a geometric progression from $2\pi$ to $10000\cdot 2\pi$ . We chose this function because we hypothesized it would allow the model to easily learn to attend by relative positions, since for any fixed offset $k$ , $PE_{pos+k}$ can be represented as a linear function of $PE_{pos}$ .

We also experimented with using learned positional embeddings \[\] instead, and found that the two versions produced nearly identical results (see Table row (E)). We chose the sinusoidal version because it may allow the model to extrapolate to sequence lengths longer than the ones encountered during training.

## 4 Why Self-Attention

In this section we compare various aspects of self-attention layers to the recurrent and convolutional layers commonly used for mapping one variable-length sequence of symbol representations $(x_{1},...,x_{n})$ to another sequence of equal length $(z_{1},...,z_{n})$ , with $x_{i},z_{i}\in\mathbb{R}^{d}$ , such as a hidden layer in a typical sequence transduction encoder or decoder. Motivating our use of self-attention we consider three desiderata.

One is the total computational complexity per layer. Another is the amount of computation that can be parallelized, as measured by the minimum number of sequential operations required.

The third is the path length between long-range dependencies in the network. Learning long-range dependencies is a key challenge in many sequence transduction tasks. One key factor affecting the ability to learn such dependencies is the length of the paths forward and backward signals have to traverse in the network. The shorter these paths between any combination of positions in the input and output sequences, the easier it is to learn long-range dependencies \[\]. Hence we also compare the maximum path length between any two input and output positions in networks composed of the different layer types.

Table 1: Maximum path lengths, per-layer complexity and minimum number of sequential operations for different layer types. $n$ is the sequence length, $d$ is the representation dimension, $k$ is the kernel size of convolutions and $r$ the size of the neighborhood in restricted self-attention.

| Layer Type | Complexity per Layer | Sequential | Maximum Path Length |
| --- | --- | --- | --- |
|  |  | Operations |  |
| Self-Attention | $O(n^{2}\cdot d)$ | $O(1)$ | $O(1)$ |
| Recurrent | $O(n\cdot d^{2})$ | $O(n)$ | $O(n)$ |
| Convolutional | $O(k\cdot n\cdot d^{2})$ | $O(1)$ | $O(log_{k}(n))$ |
| Self-Attention (restricted) | $O(r\cdot n\cdot d)$ | $O(1)$ | $O(n/r)$ |

As noted in Table , a self-attention layer connects all positions with a constant number of sequentially executed operations, whereas a recurrent layer requires $O(n)$ sequential operations. In terms of computational complexity, self-attention layers are faster than recurrent layers when the sequence length $n$ is smaller than the representation dimensionality $d$ , which is most often the case with sentence representations used by state-of-the-art models in machine translations, such as word-piece \[\] and byte-pair \[\] representations. To improve computational performance for tasks involving very long sequences, self-attention could be restricted to considering only a neighborhood of size $r$ in the input sequence centered around the respective output position. This would increase the maximum path length to $O(n/r)$ . We plan to investigate this approach further in future work.

A single convolutional layer with kernel width $k<n$ does not connect all pairs of input and output positions. Doing so requires a stack of $O(n/k)$ convolutional layers in the case of contiguous kernels, or $O(log_{k}(n))$ in the case of dilated convolutions \[\], increasing the length of the longest paths between any two positions in the network. Convolutional layers are generally more expensive than recurrent layers, by a factor of $k$ . Separable convolutions \[\], however, decrease the complexity considerably, to $O(k\cdot n\cdot d+n\cdot d^{2})$ . Even with $k=n$ , however, the complexity of a separable convolution is equal to the combination of a self-attention layer and a point-wise feed-forward layer, the approach we take in our model.

As side benefit, self-attention could yield more interpretable models. We inspect attention distributions from our models and present and discuss examples in the appendix. Not only do individual attention heads clearly learn to perform different tasks, many appear to exhibit behavior related to the syntactic and semantic structure of the sentences.

## 5 Training

This section describes the training regime for our models.

### 5.1 Training Data and Batching

We trained on the standard WMT 2014 English-German dataset consisting of about 4.5 million sentence pairs. Sentences were encoded using byte-pair encoding \[\], which has a shared source-target vocabulary of about 37000 tokens. For English-French, we used the significantly larger WMT 2014 English-French dataset consisting of 36M sentences and split tokens into a 32000 word-piece vocabulary \[\]. Sentence pairs were batched together by approximate sequence length. Each training batch contained a set of sentence pairs containing approximately 25000 source tokens and 25000 target tokens.

### 5.2 Hardware and Schedule

We trained our models on one machine with 8 NVIDIA P100 GPUs. For our base models using the hyperparameters described throughout the paper, each training step took about 0.4 seconds. We trained the base models for a total of 100,000 steps or 12 hours. For our big models,(described on the bottom line of table ), step time was 1.0 seconds. The big models were trained for 300,000 steps (3.5 days).

### 5.3 Optimizer

We used the Adam optimizer \[\] with $\beta_{1}=0.9$ , $\beta_{2}=0.98$ and $\epsilon=10^{-9}$ . We varied the learning rate over the course of training, according to the formula:

<table><tbody><tr><td></td><td><math><semantics><mrow><mrow><mi>l</mi> <mo>⁢</mo> <mi>r</mi> <mo>⁢</mo> <mi>a</mi> <mo>⁢</mo> <mi>t</mi> <mo>⁢</mo> <mi>e</mi></mrow> <mo>=</mo> <mrow><msubsup><mi>d</mi> <mtext>model</mtext> <mrow><mo>−</mo> <mn>0.5</mn></mrow></msubsup> <mo>⋅</mo> <mrow><mi>min</mi> <mo>⁡</mo> <mrow><mo>(</mo><mrow><mi>s</mi> <mo>⁢</mo> <mi>t</mi> <mo>⁢</mo> <mi>e</mi> <mo>⁢</mo> <mi>p</mi> <mo>⁢</mo> <mi>_</mi> <mo>⁢</mo> <mi>n</mi> <mo>⁢</mo> <mi>u</mi> <mo>⁢</mo> <msup><mi>m</mi> <mrow><mo>−</mo> <mn>0.5</mn></mrow></msup></mrow><mo>,</mo><mrow><mrow><mrow><mi>s</mi> <mo>⁢</mo> <mi>t</mi> <mo>⁢</mo> <mi>e</mi> <mo>⁢</mo> <mi>p</mi> <mo>⁢</mo> <mi>_</mi> <mo>⁢</mo> <mi>n</mi> <mo>⁢</mo> <mi>u</mi> <mo>⁢</mo> <mi>m</mi></mrow> <mo>⋅</mo> <mi>w</mi></mrow> <mo>⁢</mo> <mi>a</mi> <mo>⁢</mo> <mi>r</mi> <mo>⁢</mo> <mi>m</mi> <mo>⁢</mo> <mi>u</mi> <mo>⁢</mo> <mi>p</mi> <mo>⁢</mo> <mi>_</mi> <mo>⁢</mo> <mi>s</mi> <mo>⁢</mo> <mi>t</mi> <mo>⁢</mo> <mi>e</mi> <mo>⁢</mo> <mi>p</mi> <mo>⁢</mo> <msup><mi>s</mi> <mrow><mo>−</mo> <mn>1.5</mn></mrow></msup></mrow><mo>)</mo></mrow></mrow></mrow></mrow> <annotation-xml><apply><apply><ci>𝑙</ci> <ci>𝑟</ci> <ci>𝑎</ci> <ci>𝑡</ci> <ci>𝑒</ci></apply> <apply><ci>⋅</ci> <apply><csymbol>superscript</csymbol> <apply><csymbol>subscript</csymbol> <ci>𝑑</ci> <ci><mtext>model</mtext></ci></apply> <apply><cn>0.5</cn></apply></apply> <apply><apply><ci>𝑠</ci> <ci>𝑡</ci> <ci>𝑒</ci> <ci>𝑝</ci> <ci>_</ci> <ci>𝑛</ci> <ci>𝑢</ci> <apply><csymbol>superscript</csymbol> <ci>𝑚</ci> <apply><cn>0.5</cn></apply></apply></apply> <apply><apply><ci>⋅</ci> <apply><ci>𝑠</ci> <ci>𝑡</ci> <ci>𝑒</ci> <ci>𝑝</ci> <ci>_</ci> <ci>𝑛</ci> <ci>𝑢</ci> <ci>𝑚</ci></apply> <ci>𝑤</ci></apply> <ci>𝑎</ci> <ci>𝑟</ci> <ci>𝑚</ci> <ci>𝑢</ci> <ci>𝑝</ci> <ci>_</ci> <ci>𝑠</ci> <ci>𝑡</ci> <ci>𝑒</ci> <ci>𝑝</ci> <apply><csymbol>superscript</csymbol> <ci>𝑠</ci> <apply><cn>1.5</cn></apply></apply></apply></apply></apply></apply></annotation-xml> <annotation>lrate=d_{\text{model}}^{-0.5}\cdot\min({step\_num}^{-0.5},{step\_num}\cdot{% warmup\_steps}^{-1.5})</annotation> <annotation>italic_l italic_r italic_a italic_t italic_e = italic_d start_POSTSUBSCRIPT model end_POSTSUBSCRIPT start_POSTSUPERSCRIPT - 0.5 end_POSTSUPERSCRIPT ⋅ roman_min ( italic_s italic_t italic_e italic_p _ italic_n italic_u italic_m start_POSTSUPERSCRIPT - 0.5 end_POSTSUPERSCRIPT, italic_s italic_t italic_e italic_p _ italic_n italic_u italic_m ⋅ italic_w italic_a italic_r italic_m italic_u italic_p _ italic_s italic_t italic_e italic_p italic_s start_POSTSUPERSCRIPT - 1.5 end_POSTSUPERSCRIPT )</annotation></semantics></math></td><td></td><td rowspan="1"><span>(3)</span></td></tr></tbody></table>

This corresponds to increasing the learning rate linearly for the first $warmup\_steps$ training steps, and decreasing it thereafter proportionally to the inverse square root of the step number. We used $warmup\_steps=4000$ .

### 5.4 Regularization

We employ three types of regularization during training:

##### Residual Dropout

We apply dropout \[\] to the output of each sub-layer, before it is added to the sub-layer input and normalized. In addition, we apply dropout to the sums of the embeddings and the positional encodings in both the encoder and decoder stacks. For the base model, we use a rate of $P_{drop}=0.1$ .

##### Label Smoothing

During training, we employed label smoothing of value $\epsilon_{ls}=0.1$ \[\]. This hurts perplexity, as the model learns to be more unsure, but improves accuracy and BLEU score.

## 6 Results

### 6.1 Machine Translation

Table 2: The Transformer achieves better BLEU scores than previous state-of-the-art models on the English-to-German and English-to-French newstest2014 tests at a fraction of the training cost.

<table><tbody><tr><th rowspan="2"><span>Model</span></th><td colspan="2">BLEU</td><td></td><td colspan="2">Training Cost (FLOPs)</td></tr><tr><td>EN-DE</td><td>EN-FR</td><td></td><td>EN-DE</td><td>EN-FR</td></tr><tr><th>ByteNet <cite>[]</cite></th><td>23.75</td><td></td><td></td><td></td><td></td></tr><tr><th>Deep-Att + PosUnk <cite>[]</cite></th><td></td><td>39.2</td><td></td><td></td><td><math><semantics><mrow><mn>1.0</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>20</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>1.0</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>20</cn></apply></apply></annotation-xml> <annotation>1.0\cdot 10^{20}</annotation> <annotation>1.0 ⋅ 10 start_POSTSUPERSCRIPT 20 end_POSTSUPERSCRIPT</annotation></semantics></math></td></tr><tr><th>GNMT + RL <cite>[]</cite></th><td>24.6</td><td>39.92</td><td></td><td><math><semantics><mrow><mn>2.3</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>19</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>2.3</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>19</cn></apply></apply></annotation-xml> <annotation>2.3\cdot 10^{19}</annotation> <annotation>2.3 ⋅ 10 start_POSTSUPERSCRIPT 19 end_POSTSUPERSCRIPT</annotation></semantics></math></td><td><math><semantics><mrow><mn>1.4</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>20</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>1.4</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>20</cn></apply></apply></annotation-xml> <annotation>1.4\cdot 10^{20}</annotation> <annotation>1.4 ⋅ 10 start_POSTSUPERSCRIPT 20 end_POSTSUPERSCRIPT</annotation></semantics></math></td></tr><tr><th>ConvS2S <cite>[]</cite></th><td>25.16</td><td>40.46</td><td></td><td><math><semantics><mrow><mn>9.6</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>18</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>9.6</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>18</cn></apply></apply></annotation-xml> <annotation>9.6\cdot 10^{18}</annotation> <annotation>9.6 ⋅ 10 start_POSTSUPERSCRIPT 18 end_POSTSUPERSCRIPT</annotation></semantics></math></td><td><math><semantics><mrow><mn>1.5</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>20</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>1.5</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>20</cn></apply></apply></annotation-xml> <annotation>1.5\cdot 10^{20}</annotation> <annotation>1.5 ⋅ 10 start_POSTSUPERSCRIPT 20 end_POSTSUPERSCRIPT</annotation></semantics></math></td></tr><tr><th>MoE <cite>[]</cite></th><td>26.03</td><td>40.56</td><td></td><td><math><semantics><mrow><mn>2.0</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>19</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>2.0</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>19</cn></apply></apply></annotation-xml> <annotation>2.0\cdot 10^{19}</annotation> <annotation>2.0 ⋅ 10 start_POSTSUPERSCRIPT 19 end_POSTSUPERSCRIPT</annotation></semantics></math></td><td><math><semantics><mrow><mn>1.2</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>20</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>1.2</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>20</cn></apply></apply></annotation-xml> <annotation>1.2\cdot 10^{20}</annotation> <annotation>1.2 ⋅ 10 start_POSTSUPERSCRIPT 20 end_POSTSUPERSCRIPT</annotation></semantics></math></td></tr><tr><th>Deep-Att + PosUnk Ensemble <cite>[]</cite></th><td></td><td>40.4</td><td></td><td></td><td><math><semantics><mrow><mn>8.0</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>20</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>8.0</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>20</cn></apply></apply></annotation-xml> <annotation>8.0\cdot 10^{20}</annotation> <annotation>8.0 ⋅ 10 start_POSTSUPERSCRIPT 20 end_POSTSUPERSCRIPT</annotation></semantics></math></td></tr><tr><th>GNMT + RL Ensemble <cite>[]</cite></th><td>26.30</td><td>41.16</td><td></td><td><math><semantics><mrow><mn>1.8</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>20</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>1.8</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>20</cn></apply></apply></annotation-xml> <annotation>1.8\cdot 10^{20}</annotation> <annotation>1.8 ⋅ 10 start_POSTSUPERSCRIPT 20 end_POSTSUPERSCRIPT</annotation></semantics></math></td><td><math><semantics><mrow><mn>1.1</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>21</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>1.1</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>21</cn></apply></apply></annotation-xml> <annotation>1.1\cdot 10^{21}</annotation> <annotation>1.1 ⋅ 10 start_POSTSUPERSCRIPT 21 end_POSTSUPERSCRIPT</annotation></semantics></math></td></tr><tr><th>ConvS2S Ensemble <cite>[]</cite></th><td>26.36</td><td><span>41.29</span></td><td></td><td><math><semantics><mrow><mn>7.7</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>19</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>7.7</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>19</cn></apply></apply></annotation-xml> <annotation>7.7\cdot 10^{19}</annotation> <annotation>7.7 ⋅ 10 start_POSTSUPERSCRIPT 19 end_POSTSUPERSCRIPT</annotation></semantics></math></td><td><math><semantics><mrow><mn>1.2</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>21</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>1.2</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>21</cn></apply></apply></annotation-xml> <annotation>1.2\cdot 10^{21}</annotation> <annotation>1.2 ⋅ 10 start_POSTSUPERSCRIPT 21 end_POSTSUPERSCRIPT</annotation></semantics></math></td></tr><tr><th>Transformer (base model)</th><td>27.3</td><td>38.1</td><td></td><td colspan="2"><math><semantics><mrow><mn>3.3</mn> <mo>⋅</mo> <msup><mn>𝟏𝟎</mn> <mn>𝟏𝟖</mn></msup></mrow> <annotation-xml><apply><ci>bold-⋅</ci> <cn>3.3</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>18</cn></apply></apply></annotation-xml> <annotation>3.3\cdot 10^{18}</annotation> <annotation>bold_3.3 bold_⋅ bold_10 start_POSTSUPERSCRIPT bold_18 end_POSTSUPERSCRIPT</annotation></semantics></math></td></tr><tr><th>Transformer (big)</th><td><span>28.4</span></td><td><span>41.8</span></td><td></td><td colspan="2"><math><semantics><mrow><mn>2.3</mn> <mo>⋅</mo> <msup><mn>10</mn> <mn>19</mn></msup></mrow> <annotation-xml><apply><ci>⋅</ci> <cn>2.3</cn> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>19</cn></apply></apply></annotation-xml> <annotation>2.3\cdot 10^{19}</annotation> <annotation>2.3 ⋅ 10 start_POSTSUPERSCRIPT 19 end_POSTSUPERSCRIPT</annotation></semantics></math></td></tr></tbody></table>

On the WMT 2014 English-to-German translation task, the big transformer model (Transformer (big) in Table ) outperforms the best previously reported models (including ensembles) by more than $2.0$ BLEU, establishing a new state-of-the-art BLEU score of $28.4$ . The configuration of this model is listed in the bottom line of Table . Training took $3.5$ days on $8$ P100 GPUs. Even our base model surpasses all previously published models and ensembles, at a fraction of the training cost of any of the competitive models.

On the WMT 2014 English-to-French translation task, our big model achieves a BLEU score of $41.0$ , outperforming all of the previously published single models, at less than $1/4$ the training cost of the previous state-of-the-art model. The Transformer (big) model trained for English-to-French used dropout rate $P_{drop}=0.1$ , instead of $0.3$ .

For the base models, we used a single model obtained by averaging the last 5 checkpoints, which were written at 10-minute intervals. For the big models, we averaged the last 20 checkpoints. We used beam search with a beam size of $4$ and length penalty $\alpha=0.6$ \[\]. These hyperparameters were chosen after experimentation on the development set. We set the maximum output length during inference to input length + $50$ , but terminate early when possible \[\].

Table summarizes our results and compares our translation quality and training costs to other model architectures from the literature. We estimate the number of floating point operations used to train a model by multiplying the training time, the number of GPUs used, and an estimate of the sustained single-precision floating-point capacity of each GPU <sup>2</sup> <sup>2</sup> 2 We used values of 2.8, 3.7, 6.0 and 9.5 TFLOPS for K80, K40, M40 and P100, respectively..

### 6.2 Model Variations

Table 3: Variations on the Transformer architecture. Unlisted values are identical to those of the base model. All metrics are on the English-to-German translation development set, newstest2013. Listed perplexities are per-wordpiece, according to our byte-pair encoding, and should not be compared to per-word perplexities.

<table><tbody><tr><td></td><td rowspan="2"><span><math><semantics><mi>N</mi> <annotation-xml><ci>𝑁</ci></annotation-xml> <annotation>N</annotation> <annotation>italic_N</annotation></semantics></math></span></td><td rowspan="2"><span><math><semantics><msub><mi>d</mi> <mtext>model</mtext></msub> <annotation-xml><apply><csymbol>subscript</csymbol> <ci>𝑑</ci> <ci><mtext>model</mtext></ci></apply></annotation-xml> <annotation>d_{\text{model}}</annotation> <annotation>italic_d start_POSTSUBSCRIPT model end_POSTSUBSCRIPT</annotation></semantics></math></span></td><td rowspan="2"><span><math><semantics><msub><mi>d</mi> <mtext>ff</mtext></msub> <annotation-xml><apply><csymbol>subscript</csymbol> <ci>𝑑</ci> <ci><mtext>ff</mtext></ci></apply></annotation-xml> <annotation>d_{\text{ff}}</annotation> <annotation>italic_d start_POSTSUBSCRIPT ff end_POSTSUBSCRIPT</annotation></semantics></math></span></td><td rowspan="2"><span><math><semantics><mi>h</mi> <annotation-xml><ci>ℎ</ci></annotation-xml> <annotation>h</annotation> <annotation>italic_h</annotation></semantics></math></span></td><td rowspan="2"><span><math><semantics><msub><mi>d</mi> <mi>k</mi></msub> <annotation-xml><apply><csymbol>subscript</csymbol> <ci>𝑑</ci> <ci>𝑘</ci></apply></annotation-xml> <annotation>d_{k}</annotation> <annotation>italic_d start_POSTSUBSCRIPT italic_k end_POSTSUBSCRIPT</annotation></semantics></math></span></td><td rowspan="2"><span><math><semantics><msub><mi>d</mi> <mi>v</mi></msub> <annotation-xml><apply><csymbol>subscript</csymbol> <ci>𝑑</ci> <ci>𝑣</ci></apply></annotation-xml> <annotation>d_{v}</annotation> <annotation>italic_d start_POSTSUBSCRIPT italic_v end_POSTSUBSCRIPT</annotation></semantics></math></span></td><td rowspan="2"><span><math><semantics><msub><mi>P</mi> <mrow><mi>d</mi> <mo>⁢</mo> <mi>r</mi> <mo>⁢</mo> <mi>o</mi> <mo>⁢</mo> <mi>p</mi></mrow></msub> <annotation-xml><apply><csymbol>subscript</csymbol> <ci>𝑃</ci> <apply><ci>𝑑</ci> <ci>𝑟</ci> <ci>𝑜</ci> <ci>𝑝</ci></apply></apply></annotation-xml> <annotation>P_{drop}</annotation> <annotation>italic_P start_POSTSUBSCRIPT italic_d italic_r italic_o italic_p end_POSTSUBSCRIPT</annotation></semantics></math></span></td><td rowspan="2"><span><math><semantics><msub><mi>ϵ</mi> <mrow><mi>l</mi> <mo>⁢</mo> <mi>s</mi></mrow></msub> <annotation-xml><apply><csymbol>subscript</csymbol> <ci>italic-ϵ</ci> <apply><ci>𝑙</ci> <ci>𝑠</ci></apply></apply></annotation-xml> <annotation>\epsilon_{ls}</annotation> <annotation>italic_ϵ start_POSTSUBSCRIPT italic_l italic_s end_POSTSUBSCRIPT</annotation></semantics></math></span></td><td>train</td><td>PPL</td><td>BLEU</td><td>params</td></tr><tr><td></td><td>steps</td><td>(dev)</td><td>(dev)</td><td><math><semantics><mrow><mo>×</mo> <msup><mn>10</mn> <mn>6</mn></msup></mrow> <annotation-xml><apply><csymbol>absent</csymbol> <apply><csymbol>superscript</csymbol> <cn>10</cn> <cn>6</cn></apply></apply></annotation-xml> <annotation>\times 10^{6}</annotation> <annotation>× 10 start_POSTSUPERSCRIPT 6 end_POSTSUPERSCRIPT</annotation></semantics></math></td></tr><tr><td>base</td><td>6</td><td>512</td><td>2048</td><td>8</td><td>64</td><td>64</td><td>0.1</td><td>0.1</td><td>100K</td><td>4.92</td><td>25.8</td><td>65</td></tr><tr><td rowspan="4"><span>(A)</span></td><td></td><td></td><td></td><td>1</td><td>512</td><td>512</td><td></td><td></td><td></td><td>5.29</td><td>24.9</td><td></td></tr><tr><td></td><td></td><td></td><td>4</td><td>128</td><td>128</td><td></td><td></td><td></td><td>5.00</td><td>25.5</td><td></td></tr><tr><td></td><td></td><td></td><td>16</td><td>32</td><td>32</td><td></td><td></td><td></td><td>4.91</td><td>25.8</td><td></td></tr><tr><td></td><td></td><td></td><td>32</td><td>16</td><td>16</td><td></td><td></td><td></td><td>5.01</td><td>25.4</td><td></td></tr><tr><td rowspan="2"><span>(B)</span></td><td></td><td></td><td></td><td></td><td>16</td><td></td><td></td><td></td><td></td><td>5.16</td><td>25.1</td><td>58</td></tr><tr><td></td><td></td><td></td><td></td><td>32</td><td></td><td></td><td></td><td></td><td>5.01</td><td>25.4</td><td>60</td></tr><tr><td rowspan="7"><span>(C)</span></td><td>2</td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td>6.11</td><td>23.7</td><td>36</td></tr><tr><td>4</td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td>5.19</td><td>25.3</td><td>50</td></tr><tr><td>8</td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td>4.88</td><td>25.5</td><td>80</td></tr><tr><td></td><td>256</td><td></td><td></td><td>32</td><td>32</td><td></td><td></td><td></td><td>5.75</td><td>24.5</td><td>28</td></tr><tr><td></td><td>1024</td><td></td><td></td><td>128</td><td>128</td><td></td><td></td><td></td><td>4.66</td><td>26.0</td><td>168</td></tr><tr><td></td><td></td><td>1024</td><td></td><td></td><td></td><td></td><td></td><td></td><td>5.12</td><td>25.4</td><td>53</td></tr><tr><td></td><td></td><td>4096</td><td></td><td></td><td></td><td></td><td></td><td></td><td>4.75</td><td>26.2</td><td>90</td></tr><tr><td rowspan="4"><span>(D)</span></td><td></td><td></td><td></td><td></td><td></td><td></td><td>0.0</td><td></td><td></td><td>5.77</td><td>24.6</td><td></td></tr><tr><td></td><td></td><td></td><td></td><td></td><td></td><td>0.2</td><td></td><td></td><td>4.95</td><td>25.5</td><td></td></tr><tr><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td>0.0</td><td></td><td>4.67</td><td>25.3</td><td></td></tr><tr><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td>0.2</td><td></td><td>5.47</td><td>25.7</td><td></td></tr><tr><td>(E)</td><td></td><td colspan="7">positional embedding instead of sinusoids</td><td></td><td>4.92</td><td>25.7</td><td></td></tr><tr><td>big</td><td>6</td><td>1024</td><td>4096</td><td>16</td><td></td><td></td><td>0.3</td><td></td><td>300K</td><td><span>4.33</span></td><td><span>26.4</span></td><td>213</td></tr></tbody></table>

To evaluate the importance of different components of the Transformer, we varied our base model in different ways, measuring the change in performance on English-to-German translation on the development set, newstest2013. We used beam search as described in the previous section, but no checkpoint averaging. We present these results in Table .

In Table rows (A), we vary the number of attention heads and the attention key and value dimensions, keeping the amount of computation constant, as described in Section . While single-head attention is 0.9 BLEU worse than the best setting, quality also drops off with too many heads.

In Table rows (B), we observe that reducing the attention key size $d_{k}$ hurts model quality. This suggests that determining compatibility is not easy and that a more sophisticated compatibility function than dot product may be beneficial. We further observe in rows (C) and (D) that, as expected, bigger models are better, and dropout is very helpful in avoiding over-fitting. In row (E) we replace our sinusoidal positional encoding with learned positional embeddings \[\], and observe nearly identical results to the base model.

### 6.3 English Constituency Parsing

Table 4: The Transformer generalizes well to English constituency parsing (Results are on Section 23 of WSJ)

| Parser | Training | WSJ 23 F1 |
| --- | --- | --- |
| Vinyals & Kaiser el al. (2014) \[\] | WSJ only, discriminative | 88.3 |
| Petrov et al. (2006) \[\] | WSJ only, discriminative | 90.4 |
| Zhu et al. (2013) \[\] | WSJ only, discriminative | 90.4 |
| Dyer et al. (2016) \[\] | WSJ only, discriminative | 91.7 |
| Transformer (4 layers) | WSJ only, discriminative | 91.3 |
| Zhu et al. (2013) \[\] | semi-supervised | 91.3 |
| Huang & Harper (2009) \[\] | semi-supervised | 91.3 |
| McClosky et al. (2006) \[\] | semi-supervised | 92.1 |
| Vinyals & Kaiser el al. (2014) \[\] | semi-supervised | 92.1 |
| Transformer (4 layers) | semi-supervised | 92.7 |
| Luong et al. (2015) \[\] | multi-task | 93.0 |
| Dyer et al. (2016) \[\] | generative | 93.3 |

To evaluate if the Transformer can generalize to other tasks we performed experiments on English constituency parsing. This task presents specific challenges: the output is subject to strong structural constraints and is significantly longer than the input. Furthermore, RNN sequence-to-sequence models have not been able to attain state-of-the-art results in small-data regimes \[\].

We trained a 4-layer transformer with $d_{model}=1024$ on the Wall Street Journal (WSJ) portion of the Penn Treebank \[\], about 40K training sentences. We also trained it in a semi-supervised setting, using the larger high-confidence and BerkleyParser corpora from with approximately 17M sentences \[\]. We used a vocabulary of 16K tokens for the WSJ only setting and a vocabulary of 32K tokens for the semi-supervised setting.

We performed only a small number of experiments to select the dropout, both attention and residual (section ), learning rates and beam size on the Section 22 development set, all other parameters remained unchanged from the English-to-German base translation model. During inference, we increased the maximum output length to input length + $300$ . We used a beam size of $21$ and $\alpha=0.3$ for both WSJ only and the semi-supervised setting.

Our results in Table show that despite the lack of task-specific tuning our model performs surprisingly well, yielding better results than all previously reported models with the exception of the Recurrent Neural Network Grammar \[\].

In contrast to RNN sequence-to-sequence models \[\], the Transformer outperforms the BerkeleyParser \[\] even when training only on the WSJ training set of 40K sentences.

## 7 Conclusion

In this work, we presented the Transformer, the first sequence transduction model based entirely on attention, replacing the recurrent layers most commonly used in encoder-decoder architectures with multi-headed self-attention.

For translation tasks, the Transformer can be trained significantly faster than architectures based on recurrent or convolutional layers. On both WMT 2014 English-to-German and WMT 2014 English-to-French translation tasks, we achieve a new state of the art. In the former task our best model outperforms even all previously reported ensembles.

We are excited about the future of attention-based models and plan to apply them to other tasks. We plan to extend the Transformer to problems involving input and output modalities other than text and to investigate local, restricted attention mechanisms to efficiently handle large inputs and outputs such as images, audio and video. Making generation less sequential is another research goals of ours.

The code we used to train and evaluate our models is available at [https://github.com/tensorflow/tensor2tensor](https://github.com/tensorflow/tensor2tensor).

## References

## Attention Visualizations

![Refer to caption](https://arxiv.org/html/x1.png)

Figure 3: An example of the attention mechanism following long-distance dependencies in the encoder self-attention in layer 5 of 6. Many of the attention heads attend to a distant dependency of the verb ‘making’, completing the phrase ‘making…more difficult’. Attentions here shown only for the word ‘making’. Different colors represent different heads. Best viewed in color.

![Refer to caption](https://arxiv.org/html/x2.png)

Figure 4: Two attention heads, also in layer 5 of 6, apparently involved in anaphora resolution. Top: Full attentions for head 5. Bottom: Isolated attentions from just the word ‘its’ for attention heads 5 and 6. Note that the attentions are very sharp for this word.

![Refer to caption](https://arxiv.org/html/x4.png)

Figure 5: Many of the attention heads exhibit behaviour that seems related to the structure of the sentence. We give two such examples above, from two different heads from the encoder self-attention at layer 5 of 6. The heads clearly learned to perform different tasks.

[^1]: Jimmy Lei Ba, Jamie Ryan Kiros, and Geoffrey E Hinton.Layer normalization.arXiv preprint arXiv:1607.06450, 2016.

[^2]: Dzmitry Bahdanau, Kyunghyun Cho, and Yoshua Bengio.Neural machine translation by jointly learning to align and translate.CoRR, abs/1409.0473, 2014.

[^3]: Denny Britz, Anna Goldie, Minh-Thang Luong, and Quoc V. Le.Massive exploration of neural machine translation architectures.CoRR, abs/1703.03906, 2017.

[^4]: Jianpeng Cheng, Li Dong, and Mirella Lapata.Long short-term memory-networks for machine reading.arXiv preprint arXiv:1601.06733, 2016.

[^5]: Kyunghyun Cho, Bart van Merrienboer, Caglar Gulcehre, Fethi Bougares, Holger Schwenk, and Yoshua Bengio.Learning phrase representations using rnn encoder-decoder for statistical machine translation.CoRR, abs/1406.1078, 2014.

[^6]: Francois Chollet.Xception: Deep learning with depthwise separable convolutions.arXiv preprint arXiv:1610.02357, 2016.

[^7]: Junyoung Chung, Çaglar Gülçehre, Kyunghyun Cho, and Yoshua Bengio.Empirical evaluation of gated recurrent neural networks on sequence modeling.CoRR, abs/1412.3555, 2014.

[^8]: Chris Dyer, Adhiguna Kuncoro, Miguel Ballesteros, and Noah A. Smith.Recurrent neural network grammars.In Proc. of NAACL, 2016.

[^9]: Jonas Gehring, Michael Auli, David Grangier, Denis Yarats, and Yann N. Dauphin.Convolutional sequence to sequence learning.arXiv preprint arXiv:1705.03122v2, 2017.

[^10]: Alex Graves.Generating sequences with recurrent neural networks.arXiv preprint arXiv:1308.0850, 2013.

[^11]: Kaiming He, Xiangyu Zhang, Shaoqing Ren, and Jian Sun.Deep residual learning for image recognition.In Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition, pages 770–778, 2016.

[^12]: Sepp Hochreiter, Yoshua Bengio, Paolo Frasconi, and Jürgen Schmidhuber.Gradient flow in recurrent nets: the difficulty of learning long-term dependencies, 2001.

[^13]: Sepp Hochreiter and Jürgen Schmidhuber.Long short-term memory.Neural computation, 9(8):1735–1780, 1997.

[^14]: Zhongqiang Huang and Mary Harper.Self-training PCFG grammars with latent annotations across languages.In Proceedings of the 2009 Conference on Empirical Methods in Natural Language Processing, pages 832–841. ACL, August 2009.

[^15]: Rafal Jozefowicz, Oriol Vinyals, Mike Schuster, Noam Shazeer, and Yonghui Wu.Exploring the limits of language modeling.arXiv preprint arXiv:1602.02410, 2016.

[^16]: Łukasz Kaiser and Samy Bengio.Can active memory replace attention?In Advances in Neural Information Processing Systems, (NIPS), 2016.

[^17]: Łukasz Kaiser and Ilya Sutskever.Neural GPUs learn algorithms.In International Conference on Learning Representations (ICLR), 2016.

[^18]: Nal Kalchbrenner, Lasse Espeholt, Karen Simonyan, Aaron van den Oord, Alex Graves, and Koray Kavukcuoglu.Neural machine translation in linear time.arXiv preprint arXiv:1610.10099v2, 2017.

[^19]: Yoon Kim, Carl Denton, Luong Hoang, and Alexander M. Rush.Structured attention networks.In International Conference on Learning Representations, 2017.

[^20]: Diederik Kingma and Jimmy Ba.Adam: A method for stochastic optimization.In ICLR, 2015.

[^21]: Oleksii Kuchaiev and Boris Ginsburg.Factorization tricks for LSTM networks.arXiv preprint arXiv:1703.10722, 2017.

[^22]: Zhouhan Lin, Minwei Feng, Cicero Nogueira dos Santos, Mo Yu, Bing Xiang, Bowen Zhou, and Yoshua Bengio.A structured self-attentive sentence embedding.arXiv preprint arXiv:1703.03130, 2017.

[^23]: Minh-Thang Luong, Quoc V. Le, Ilya Sutskever, Oriol Vinyals, and Lukasz Kaiser.Multi-task sequence to sequence learning.arXiv preprint arXiv:1511.06114, 2015.

[^24]: Minh-Thang Luong, Hieu Pham, and Christopher D Manning.Effective approaches to attention-based neural machine translation.arXiv preprint arXiv:1508.04025, 2015.

[^25]: Mitchell P Marcus, Mary Ann Marcinkiewicz, and Beatrice Santorini.Building a large annotated corpus of english: The penn treebank.Computational linguistics, 19(2):313–330, 1993.

[^26]: David McClosky, Eugene Charniak, and Mark Johnson.Effective self-training for parsing.In Proceedings of the Human Language Technology Conference of the NAACL, Main Conference, pages 152–159. ACL, June 2006.

[^27]: Ankur Parikh, Oscar Täckström, Dipanjan Das, and Jakob Uszkoreit.A decomposable attention model.In Empirical Methods in Natural Language Processing, 2016.

[^28]: Romain Paulus, Caiming Xiong, and Richard Socher.A deep reinforced model for abstractive summarization.arXiv preprint arXiv:1705.04304, 2017.

[^29]: Slav Petrov, Leon Barrett, Romain Thibaux, and Dan Klein.Learning accurate, compact, and interpretable tree annotation.In Proceedings of the 21st International Conference on Computational Linguistics and 44th Annual Meeting of the ACL, pages 433–440. ACL, July 2006.

[^30]: Ofir Press and Lior Wolf.Using the output embedding to improve language models.arXiv preprint arXiv:1608.05859, 2016.

[^31]: Rico Sennrich, Barry Haddow, and Alexandra Birch.Neural machine translation of rare words with subword units.arXiv preprint arXiv:1508.07909, 2015.

[^32]: Noam Shazeer, Azalia Mirhoseini, Krzysztof Maziarz, Andy Davis, Quoc Le, Geoffrey Hinton, and Jeff Dean.Outrageously large neural networks: The sparsely-gated mixture-of-experts layer.arXiv preprint arXiv:1701.06538, 2017.

[^33]: Nitish Srivastava, Geoffrey E Hinton, Alex Krizhevsky, Ilya Sutskever, and Ruslan Salakhutdinov.Dropout: a simple way to prevent neural networks from overfitting.Journal of Machine Learning Research, 15(1):1929–1958, 2014.

[^34]: Sainbayar Sukhbaatar, Arthur Szlam, Jason Weston, and Rob Fergus.End-to-end memory networks.In C. Cortes, N. D. Lawrence, D. D. Lee, M. Sugiyama, and R. Garnett, editors, Advances in Neural Information Processing Systems 28, pages 2440–2448. Curran Associates, Inc., 2015.

[^35]: Ilya Sutskever, Oriol Vinyals, and Quoc VV Le.Sequence to sequence learning with neural networks.In Advances in Neural Information Processing Systems, pages 3104–3112, 2014.

[^36]: Christian Szegedy, Vincent Vanhoucke, Sergey Ioffe, Jonathon Shlens, and Zbigniew Wojna.Rethinking the inception architecture for computer vision.CoRR, abs/1512.00567, 2015.

[^37]: Vinyals & Kaiser, Koo, Petrov, Sutskever, and Hinton.Grammar as a foreign language.In Advances in Neural Information Processing Systems, 2015.

[^38]: Yonghui Wu, Mike Schuster, Zhifeng Chen, Quoc V Le, Mohammad Norouzi, Wolfgang Macherey, Maxim Krikun, Yuan Cao, Qin Gao, Klaus Macherey, et al.Google’s neural machine translation system: Bridging the gap between human and machine translation.arXiv preprint arXiv:1609.08144, 2016.

[^39]: Jie Zhou, Ying Cao, Xuguang Wang, Peng Li, and Wei Xu.Deep recurrent models with fast-forward connections for neural machine translation.CoRR, abs/1606.04199, 2016.

[^40]: Muhua Zhu, Yue Zhang, Wenliang Chen, Min Zhang, and Jingbo Zhu.Fast and accurate shift-reduce constituent parsing.In Proceedings of the 51st Annual Meeting of the ACL (Volume 1: Long Papers), pages 434–443. ACL, August 2013.