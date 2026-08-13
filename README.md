# Esperanta Artikolo-Korpuso（プライベート）

エスペラント学習・輪読用に収集した記事コーパスの保管リポジトリ。

> **重要**: 記事本文の著作権は各サイト・各著者に帰属します。このリポジトリは
> **プライベート運用が前提**であり、内容の再配布・一般公開はしないでください。

収集ツール(公開リポジトリ): [esperanta-artikolo-kolektilo](https://github.com/Esperanto-Societo-de-Kioto-Universitato/esperanta-artikolo-kolektilo)

## 収録内容(2026-08-13 時点)

| フォルダ | 期間 | 記事数 | 内容 |
|---|---|---|---|
| `取得文書ekde20260303/` | 2025-03-03〜2026-03-03 | 1197 | 7サイト(Pola Retradio 含む)。Monato は ID プローブで補完済み |
| `取得文書ekde20260401/` | 2026-03-04〜2026-08-13 | 363 | 6サイト(Pola Retradio 除外) |

- 2つのフォルダで **2025-03-03〜2026-08-13 が切れ目なし**(計1560本)
- 各記事は md / txt / csv / jsonl の4形式
- サイト×月の内訳・既知の注意点は各フォルダ内の `MANIFEST.md` を参照

## 更新手順

kolektilo 側の作業フォルダで新しい期間を取得したのち、同フォルダの
`sync_korpuso.sh` を実行すると、取得文書フォルダがここへ同期され
commit & push される。
