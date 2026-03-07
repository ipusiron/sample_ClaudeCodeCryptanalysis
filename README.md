# sample_ClaudeCodeCryptanalysis

同人誌『Claude Code暗号解読決戦　ミジンコ vs. AIエージェント』（著：IPUSIRON、「技術書典20」初頒布）のサンプルファイルを管理する

## リポジトリ構成

### チャレンジ暗号文と平文（`challege/`）

3つのチャレンジ暗号文と、それぞれに対応する元の平文を収録しています。

| フォルダー | 暗号方式 | 鍵 |
|---|---|---|
| `challege/ciphertext1/` | ヴィジュネル暗号 | "EAGLE"（5文字） |
| `challege/ciphertext2/` | ヴィジュネル暗号 | "LIBERTYEAGLEJUSTICE"（19文字） |
| `challege/ciphertext3/` | ヴィジュネル暗号＋コラムナー転置暗号（二重暗号） | "LIBERTYEAGLEJUSTICE"（19文字）＋"FREEDOM"（7文字） |

各フォルダーには `ciphertext.txt`（暗号文）、`plaintext.txt`（平文）、`README.md`（暗号の仕様）が含まれています。

### 偉人会議プロンプト（`cryptanalysis/ijinkaigi_prompt/`）

偉人会議プロジェクトで使用するプロンプトファイル（`prompt.txt`）を収録しています。

### 偉人会議プロジェクトのCLAUDE.md（`cryptanalysis/ijinkaigi_project/`）

偉人会議プロジェクト用の `CLAUDE.md` ファイルを収録しています。

## 関連リンク

- 書籍購入：https://hack.booth.pm/items/8015186
- 著者ブログ：https://akademeia.info
- 著者X：https://x.com/ipusiron

## ライセンス

暗号文および平文は学習・研究目的での利用を歓迎します。
