# weather-pattern-classification-data

NDL manual weather chart archive (JPEG, 2000-01-01 to 2022-09-30, 0Z/12Z).

Manually collected from the National Diet Library Digital Collections
(https://dl.ndl.go.jp/pid/12896309) and converted from PDF to PNG to JPEG,
because the NDL site returns 401 Unauthorized on direct PDF download and
requires a browser-authenticated session.

Used by [awg-yk/weather-pattern-classification](https://github.com/awg-yk/weather-pattern-classification)
via `scripts/fetch_manual_chart.py`, which fetches individual files from
this repo's raw URLs by date rather than cloning it.

## Layout

```
data/raw/ndl_manual/jpg/{Js,JS}_{YYYYMMDDHH}_page001.jpg
```

Filename prefix case varies (`Js_`/`JS_`) depending on when a given file was
collected; downstream code tries both.
