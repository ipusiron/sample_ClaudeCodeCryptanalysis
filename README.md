# sample_ClaudeCodeCryptanalysis

商業誌『生成AI時代の暗号技術入門』（インプレスの「技術の泉」シリーズとして刊行）と同人誌『Claude Code暗号解読決戦　ミジンコ vs. AIエージェント』（技術書典20で頒布）で用いるサンプルファイルを管理します。

## リポジトリ構成

### チャレンジ暗号文と平文（`challenge/`）

3つのチャレンジ暗号文と、それぞれに対応する元の平文を収録しています。平文は3つともアメリカ独立宣言です。

| フォルダー | 暗号方式 | 鍵 |
|---|---|---|
| `challenge/ciphertext1/` | ヴィジュネル暗号 | "EAGLE"（5文字） |
| `challenge/ciphertext2/` | ヴィジュネル暗号 | "LIBERTYEAGLEJUSTICE"（19文字） |
| `challenge/ciphertext3/` | ヴィジュネル暗号と縦列転置式暗号の積暗号 | "LIBERTYEAGLEJUSTICE"（19文字）＋"FREEDOM"（7文字） |

各フォルダーには次のファイルが含まれています。

| ファイル | 内容 |
|---|---|
| `ciphertext.txt` | 暗号文 |
| `plaintext.txt` | 平文 |
| `key.txt` | 鍵文字列のみ（プログラムから読み込む用） |
| `answer.txt` | 暗号方式・鍵長・モードなどの鍵情報（YAML形式） |
| `README.md` | 暗号の仕様 |

このほか、`ciphertext1/` と `ciphertext2/` には復号結果（`decrypted_text.txt`／`decrypted.txt`）、`ciphertext2/` と `ciphertext3/` には解読セッションの記録（`log/`）を収録しています。

### 平文の全文（`plaintext/`）

3つのチャレンジ暗号文に共通する平文（アメリカ独立宣言の英文全文）を `declaration.txt` として収録しています。各フォルダーの `plaintext.txt` と同じ内容です。

### 偉人会議プロンプト（`cryptanalysis/council-prompt/`）

偉人会議で使用するプロンプトファイル（`prompt.txt`）を収録しています。

### 偉人会議プロジェクトのCLAUDE.md（`cryptanalysis/council-cryptanalysis/`）

偉人会議プロジェクト用の `CLAUDE.md` ファイルを収録しています。

### Agent TeamsプロジェクトのCLAUDE.md（`cryptanalysis/agent-teams-cryptanalysis/`）

Agent Teamsによる暗号解読プロジェクト用の `CLAUDE.md` ファイルを収録しています。`CLAUDE2.md` は、`CLAUDE.md` にGit連携（コミットのタイミング、コミットメッセージの規約、コミット手順）の節を加えたものです。

## 関連リンク

- 書籍『生成AI時代の暗号技術入門』購入：[https://nextpublishing.jp/book/19897.html](https://nextpublishing.jp/book/19897.html)（インプレスの書籍ページ）、[https://akademeia.info/?page_id=50528](https://akademeia.info/?page_id=50528)（サポートページ）
- 書籍『Claude Code暗号解読決戦　ミジンコ vs. AIエージェント』購入：[https://hack.booth.pm/items/8015186](https://hack.booth.pm/items/8015186)
- 著者ブログ：[https://akademeia.info](https://akademeia.info)
- 著者X：[https://x.com/ipusiron](https://x.com/ipusiron)

## ライセンス

暗号文および平文は学習・研究目的での利用を歓迎します。
