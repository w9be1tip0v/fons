# Obsidian Zettelkasten ナレッジベース構成ガイド

> [!info] 概要
> Niklas Luhmannの原則に基づき、Sönke Ahrensの「How to Take Smart Notes」方法論を実装したObsidianナレッジベースの完全な構成ガイド

## 🏗️ フォルダ構造

### 1️⃣ フリーティングノート（1_Fleeting）
```
1_Fleeting/
├── About - 1_Fleeting Notes.md
└── 日々のアイデア・メモ
```

**目的**: 一時的なアイデアやインスピレーションを素早く記録
**ルール**:
- 思いついたアイデアをそのまま記録
- 定期的に見直し、価値のあるものを2_Literatureや3_Permanentに昇格
- 短期間で処理（週に1-2回見直し）

### 2️⃣ 文献ノート（2_Literature）
```
2_Literature/
├── _About - 2_Literature Notes.md
├── [書籍タイトル] - [著者名].md
├── [人物名].md
├── [概念・用語].md
└── Tags provide architecture.md
```

**目的**: 外部ソースから得た知識を整理・要約
**ルール**:
- 情報源を明記
- 自分の言葉で要約
- 重要な引用は正確に記録
- ソース単位でノートを作成

### 3️⃣ 永続ノート（3_Permanent）
```
3_Permanent/
├── _About - 3_Permanent Notes.md
├── [独立したアイデア].md
└── Basic Zettelkasten vs Extended Digital Zettelkasten.md
```

**目的**: 完全に処理された、独立したアイデアや洞察
**ルール**:
- 一つのアイデア、一つのノート
- 自分の言葉で記述
- 他のノートと意味のあるリンク
- 将来の自分が理解できる内容

### 4️⃣ プロジェクトノート（4_Project）
```
4_Project/
├── About - 4_Project Notes.md
├── [プロジェクト名]/
│   ├── _MOC - [プロジェクト名].md
│   ├── Project Log - [プロジェクト名].md
│   └── History - [プロジェクト名].md
└── Posts Zettelkasten/
```

**目的**: 特定の期限付きプロジェクトに関連する情報
**ルール**:
- プロジェクト毎にフォルダ作成
- MOC（Map of Content）で全体を統括
- 完了後はアーカイブ

### 5️⃣ 構造ノート（5_Structure）
```
5_Structure/
├── _About - 5_Structure Notes.md
├── Index - Zettelkasten.md
├── Terms - Zettelkasten.md
├── Glossary.md
├── Books.md
├── Quotes.md
├── ARCO View.md
├── Inspect View.md
├── 7 Days Created Chart.md
└── Canvases/
    ├── About - 1_Fleeting Notes.canvas
    ├── About - 2_Literature Notes.canvas
    ├── About - 3_Permanent Notes.canvas
    ├── About - 4_Project Notes.canvas
    └── About - 5_Structure Notes.canvas
```

**目的**: システム全体のナビゲーションと関連ノートの整理
**ルール**:
- 関連ノートのハブとして機能
- 定期的に更新
- Dataviewクエリで動的生成

## 🏷️ タグ体系

### タイプ分類
- `#type/fleeting` - フリーティングノート
- `#type/literature` - 文献ノート  
- `#type/permanent` - 永続ノート
- `#type/project` - プロジェクトノート
- `#type/structure` - 構造ノート

### 構造分類
- `#structure/moc` - Map of Content
- `#structure/index` - インデックス
- `#structure/about` - 説明ページ
- `#structure/canvas` - キャンバス
- `#structure/list` - リスト

### テーマ分類
- `#theme/zettelkasten` - Zettelkasten関連
- `#theme/productivity` - 生産性
- `#theme/learning` - 学習
- `#theme/research` - 研究

### ターゲット分類
- `#target/project` - プロジェクト関連
- `#target/github` - GitHub関連
- `#target/starterkit` - スターターキット

## 📝 テンプレート構成

### 基本テンプレート
- **2_Book Template** - 書籍レビュー用
- **2_Person Template** - 人物記録用
- **2_Quote Template** - 引用記録用
- **2_Term Template** - 用語定義用
- **2_Tool Template** - ツール評価用
- **3_Note Template** - 永続ノート用
- **3_Question Template** - 質問記録用
- **5_Structure Template** - 構造ノート用

### プロジェクト用テンプレート
- **4_Post Template** - ブログ投稿用
- **4_E-book Template** - 電子書籍用
- **5_Meeting Notes Template** - 会議記録用
- **5_OKR Template** - 目標管理用

### 生産性テンプレート
- **5_BuJo - Daily Log** - デイリーログ
- **5_BuJo - Weekly Log** - ウィークリーログ
- **5_BuJo - Monthly Log** - マンスリーログ
- **5_BuJo - Future Log** - フューチャーログ

## 🔗 リンク戦略

### 内部リンク
```markdown
[[ノート名]]           # 基本リンク
[[ノート名|表示名]]    # エイリアスリンク
[[ノート名#見出し]]    # セクションリンク
![[ノート名]]          # 埋め込みリンク
```

### バックリンク活用
- 関連ノートの自動発見
- アイデアの進化追跡
- 知識のクラスター化

### MOCによる構造化
- 関連トピックの集約
- ナビゲーションハブ
- 知識マップの作成

## 📊 Dataview活用

### 動的クエリ例
```dataview
TABLE WITHOUT ID 
	file.link as "Recent Notes", 
	(date(today) - file.cday).day as "Days Old",
	template_type as "Type"
FROM "3_Permanent" 
WHERE template_type
SORT file.cday desc 
LIMIT 10
```

### ホームページ機能
- ランダム引用表示
- 最近の活動表示
- 統計情報表示

## 🔄 ワークフロー

### 日次プロセス
1. **新しいアイデア** → `1_Fleeting` に記録
2. **読書・研究** → `2_Literature` でまとめ
3. **アイデア処理** → 価値あるものを `3_Permanent` に昇格

### 週次レビュー
1. `1_Fleeting` の整理・処理
2. リンクの強化
3. 孤立ノートの発見・接続

### 月次メンテナンス
1. 構造の見直し
2. タグの整理
3. プロジェクトの進捗確認

## ⚙️ 推奨プラグイン

### 必須プラグイン
- **Dataview** - 動的クエリ
- **Templates** - テンプレート管理
- **Obsidian Git** - バージョン管理

### 推奨プラグイン
- **Graph Analysis** - グラフ解析
- **Tag Wrangler** - タグ管理
- **Calendar** - 時系列ナビゲーション
- **Kanban** - プロジェクト管理

## 📈 成長戦略

### スタート期（0-3ヶ月）
- 基本構造の理解
- テンプレートの習得
- 日次習慣の確立

### 発展期（3-12ヶ月）  
- 知識ネットワークの拡大
- 専門分野の深化
- 個人的カスタマイズ

### 成熟期（12ヶ月以降）
- システムの最適化
- 高度なクエリ活用
- 知識の外部発信

---

> [!success] 成功の鍵
> **継続性** > 完璧性。まずは小さく始めて、徐々にシステムを成長させることが重要です。

**参考文献**:
- Sönke Ahrens「How to Take Smart Notes」
- [Obsidian-Zettelkasten-Starter-Kit](https://github.com/groepl/Obsidian-Zettelkasten-Starter-Kit)
- [Obsidian公式ドキュメント](https://obsidian.md) 