# Claude Code ワークショップ素材

AI木曜会「開発以外で使うClaude Code入門」講座で使う練習用ファイルです。

## このリポジトリの使い方

1. ファイルをダウンロードする（下記参照）
2. Claude Codeでこのフォルダを開く
3. 日本語で指示を出して、ファイルを操作してみる

---

## ダウンロード方法

### 方法A：ZIPダウンロード（git不要・かんたん）

1. このページの上部にある緑色の「Code」ボタンをクリック
2. 「Download ZIP」を選択
3. ダウンロードしたZIPファイルを展開する
4. わかりやすい場所（デスクトップなど）に置く

### 方法B：git clone（ターミナルが使える人）

```bash
git clone https://github.com/Akane2block/claude-code-workshop.git
```

---

## Claude Codeの始め方（3つの方法）

### 方法①：Claude Desktopの「Code」タブ（最もカンタン）

1. [Claude Desktop](https://claude.ai/download) をダウンロード・インストール
2. Claudeを開き、左下の「Code」タブをクリック
3. このフォルダを指定して開く
4. 日本語で指示を入力する

> ターミナル不要、git不要。一番かんたんな方法です。

### 方法②：VS Code + Claude Code拡張

1. [VS Code](https://code.visualstudio.com/) をインストール
2. VS Codeの拡張機能から「Claude Code」をインストール
3. VS Codeでこのフォルダを開く
4. Claude Codeパネルから指示を入力する

> ファイルの変更がリアルタイムで見えるので便利です。

### 方法③：CLIから起動（本格派向け）

1. [Node.js](https://nodejs.org/) をインストール（LTS版を推奨）
2. ターミナルで以下を実行：

```bash
npm install -g @anthropic-ai/claude-code
```

3. このフォルダに移動して `claude` と入力：

```bash
cd claude-code-workshop
claude
```

---

## 料金プランの注意点

Claude Codeを使うには **Claudeの有料プラン（Pro以上）** が必要です。

| プラン | 月額 | Claude Code利用 |
|--------|------|----------------|
| Free | 無料 | 使えない |
| Pro | $20 | 使えるが、すぐ制限に達しやすい |
| Max | $100〜 | がっつり使いたい人向け。制限が緩い |

> ワークショップで少し試す程度ならProでも大丈夫ですが、日常的に使うならMaxプランがおすすめです。

---

## フォルダ構成

```
claude-code-workshop/
├── README.md              ← このファイル
├── CLAUDE.md              ← Claude Code用のルールファイル（サンプル）
├── 01_議事録/              ← 練習用の議事録ファイル（3件）
├── 02_CSVデータ/           ← 練習用のCSVファイル（2件）
├── 03_告知文/              ← リライト練習用の告知文原稿
└── 04_CLAUDE_md_サンプル/   ← CLAUDE.mdの書き方サンプル集
```

---

## 練習してみよう

Claude Codeを起動したら、以下の指示を試してみてください：

### 基本操作
- 「このフォルダの中身を見て、概要をまとめて」
- 「01_議事録フォルダの中身を全部読んで、決定事項だけまとめて」

### CSV分析
- 「02_CSVデータのアンケート結果.csvを分析して、傾向を教えて」
- 「イベント参加者リスト.csvから、参加回数が多い順に並べ替えて」

### 文章のリライト
- 「03_告知文の原稿を、Slack投稿用に短くリライトして」
- 「同じ原稿をX（Twitter）用に140文字以内にまとめて」

### CLAUDE.mdの体験
- 「CLAUDE.mdに書いてあるルールを確認して」
- 「ルールに従って、告知文を書き直して」

---

## トラブルシューティング

### Claude Desktopで「Code」タブが表示されない
- アプリを最新版にアップデートしてください
- 有料プラン（Pro以上）に加入しているか確認してください

### VS CodeでClaude Code拡張が動かない
- VS Codeを再起動してみてください
- 拡張機能が最新版か確認してください

### CLIで `claude` コマンドが見つからない
- Node.jsが正しくインストールされているか確認：`node -v`
- npmでインストールされているか確認：`npm list -g @anthropic-ai/claude-code`
- ターミナルを一度閉じて開き直してみてください

### 「使用制限に達しました」と表示される
- Proプランでは短時間の集中利用で制限に達することがあります
- しばらく待つか、Maxプランへのアップグレードを検討してください
