# MANIFEST — 取得文書ekde20260814

- 生成日: 2026-09-15 20:04
- 総記事数: **86**
- 各記事は md / txt / csv / jsonl の4形式で保存（記事数は jsonl 行数）
- 記事本文はコーパスリポジトリ esperanta-artikolo-korpuso で管理（コード用リポジトリ kolektilo には含めない）
- 各記事の著作権は掲載サイト・著者に帰属する（出典 URL は各記事に記載）

## サイト × 月 記事数

| サイト | 2026-08 | 2026-09 | 合計 | 日付範囲 |
|---|---|---|---|---|
| el_popola_cxinio | 23 | 31 | **54** | 2026-08-14 〜 2026-09-14 |
| global_voices_eo | 2 | 2 | **4** | 2026-08-26 〜 2026-09-13 |
| libera_folio | 5 | 2 | **7** | 2026-08-18 〜 2026-09-08 |
| monato | 4 | 10 | **14** | 2026-08-17 〜 2026-09-07 |
| uea_facila | 5 | 2 | **7** | 2026-08-15 〜 2026-09-12 |

## 備考

### このフォルダの位置づけ

前フォルダ『取得文書ekde20260401』(〜2026-08-13) の続き。2026-09-15 実行。

- 収集期間: **2026-08-14 〜 2026-09-14**(6サイト、Pola Retradio はユーザー方針により除外)
- ジョブは 2026-07-01〜09-14 で実行し、07-01〜08-13 は前フォルダとの重複区間として、既存記事との突合と遅れて公開された記事の回収に使った(該当なし)。既存コーパスと URL 単位で重複除去済み。
- 出所ジョブ: `jobs/qsub_*_20260701_20260914_8w.sh`(一括投入は `submit_all_sites_20260701_20260914_8w.sh`、ログは `logs/*_20260701_20260914_8w.*`)。取得コードは kolektilo v1.3.0(本文の雑音除去を修正済み)。

### サイト別の注意点

- **Global Voices eo**: 2026-05-14 以降止まっていた更新が 2026-08-26 に再開した(4 本):
  - 2026-08-26『Ĉu vi volas antaŭenigi la lingvon Esperanto? Fariĝu tradukmanaĝero ĉe Lingua』(`/2026/08/15889/`)
  - 2026-08-30『Perditaj en traduko: Kiel modeloj de artefarita intelekto influas lingvokomunumojn kun malmultaj rimedoj』(`/2026/08/15862/`)
  - 2026-09-05『Identeco preter civitaneco: Kio restas kiam la ŝtato rifuzas agnoski vin?』(`/2026/09/15964/`)
  - 2026-09-13『Tra Latinameriko, la manifestacioj de la 1-a de majo elstarigas luktojn kaj solidarecon de laboristoj』(`/2026/09/15879/`)
  - 取得当日はサイトに接続できなくなり(計算ノード・ログインノードとも `No route to host`、ジョブは 3 回失敗)、同日まだ接続できていたうちにログインノードで同じ `Global Voices en Esperanto/parallel_scraper.py`(`--method auto`、修正後のコード)を 2025-03-01〜2026-09-14 で実行した結果から、本フォルダの期間分を採用した。
- **Monato**: `--method both`(Nova! ページ+ID プローブ)で取得。14 本のうち全文公開は 2 本で、残りは冒頭のみ(続きは購読者限定)。
- **UEA Facila**: 1 回目のジョブは、作業フォルダに置いていた HTTP キャッシュ(SQLite)への複数ノードからの同時アクセスで落ちたため、キャッシュの置き場所を直して再実行した。
- **Scivolemo**: サイト更新停止中のため 0 本(ファイルなし)。
- **El Popola Ĉinio**: 記事末尾のリンクの文言「Ĉina Fokuso / China Focus - Esperanto」を 54 本から除去した(取得後に見つかった除去処理の不具合を直して同じ処理を適用。修正後のコードで取り直した本文と一致することを確認済み)。
- **Libera Folio**: 特記事項なし。

