# Esperanta Artikolo-Korpuso

エスペラント学習・輪読用に収集した記事コーパスの保管リポジトリ。

> 各記事の著作権は掲載サイト・著者に帰属します。各記事には出典 URL を記載しています。
> 引用・再配布の際は各サイトの利用条件を確認してください。

収集ツール: [esperanta-artikolo-kolektilo](https://github.com/Esperanto-Societo-de-Kioto-Universitato/esperanta-artikolo-kolektilo)

## 収録内容(2026-09-15 時点)

| フォルダ | 期間 | 記事数 | 内容 |
|---|---|---|---|
| `取得文書ekde20260303/` | 2025-03-03〜2026-03-03 | 1198 | 7サイト(Pola Retradio 含む)。Monato は ID プローブで補完済み |
| `取得文書ekde20260401/` | 2026-03-04〜2026-08-13 | 366 | 6サイト(Pola Retradio 除外) |
| `取得文書ekde20260814/` | 2026-08-14〜2026-09-14 | 86 | 6サイト(Pola Retradio 除外) |

- 3つのフォルダで **2025-03-03〜2026-09-14 が切れ目なし**(計1650本)。フォルダ間で同じ URL は重複しない
- 各記事は md / txt / csv / jsonl の4形式
- サイト×月の内訳・既知の注意点は各フォルダ内の `MANIFEST.md` を参照

## 更新手順

kolektilo 側の作業フォルダで新しい期間を取得したのち、同フォルダの
`sync_korpuso.sh` を実行すると、取得文書フォルダがここへ同期され
commit & push される。
