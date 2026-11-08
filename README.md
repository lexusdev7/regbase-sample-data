# RegBase — Japan Corporate Registry Diff (free sample)

A free sample of the daily publication diff of Japan's corporate number
registry (published by the National Tax Agency): companies newly
registered, changed, closed, and revived, classified by change type.

## Files

- `sample_diff_20261106.csv` — the first 100 records of the 2026-11-06
  publication diff.
- `census_summary.json` — the full census of that day's diff:
  2,617 records (new 1,404 / changed 895 / closed 298 / revived 20),
  with breakdowns by change code and prefecture. The change-code census
  follows the NTA resource definition: code 22 is counted as revivals,
  not closures.

This sample is the same file published on Zenodo
(DOI: https://doi.org/10.5281/zenodo.24046548, license as recorded there)
and on Hugging Face:
https://huggingface.co/datasets/lexusdev7/regbase-jp-registry-diff-sample

## The full data and the API

- Full dated archives and analysis packs (BOOTH):
  https://regbase.booth.pm/
- Signed-record API (Ed25519-signed JSON records by corporate number):
  https://regbase.local-connect-design.trade
- Try the signature yourself — in-browser verification demo:
  https://regbase.local-connect-design.trade/verify
- API docs (Postman public workspace):
  https://www.postman.com/regbase-198277/workspace/regbase/overview
- The same three operations as Apify actors:
  https://apify.com/regbase/jp-diff-feed ,
  https://apify.com/regbase/jp-company-lookup ,
  https://apify.com/regbase/jp-signed-record

Source data: National Tax Agency corporate number publication
(https://www.houjin-bangou.nta.go.jp/).
