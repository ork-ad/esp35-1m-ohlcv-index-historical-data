# ESP35 1m OHLCV Index Historical Data — Free Sample

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Dataset rows](https://img.shields.io/badge/full_dataset-2_608_958_rows-blue)](https://ork.ad/) [![Updated](https://img.shields.io/badge/weekly_update-every_Sunday-green)](https://ork.ad/) [![Full data on ork.ad](https://img.shields.io/badge/download-ork.ad-orange)](https://ork.ad/)

### → [**Download the full ESP35 dataset on ork.ad**](https://ork.ad/)

**ESP35 1m OHLCV Stock index historical data** — ultra high-quality 1m OHLCV for **Spain 35**. Global cash and extended index sessions — Asia, Europe and US coverage, not US-hours only. Clean `time, open, high, low, close, volume` CSV for backtesting, algorithmic trading and quantitative research.

## Table of contents

- [Why this dataset?](#why-this-dataset)
- [Download sample CSV](#download-sample)
- [GitHub Pages preview](#github-pages)
- [Sample vs full dataset](#sample-vs-full-dataset)
- [Timeframes on ork.ad](#timeframes-on-orkad)
- [Weekly updates](#weekly-updates)
- [Data preview](#data-preview)
- [Schema](#schema)
- [Code examples](#code-examples)
- [Download full data on ork.ad](#download-full-data)

## Why this dataset?

- **Ultra high-quality 1m OHLCV** for **Spain 35** (Stock index)
- **Global cash and extended index sessions — Asia, Europe and US coverage, not US-hours only**
- **Clean CSV schema** — `time, open, high, low, close, volume` (no gaps in formatting)
- **Free evaluation sample** on GitHub (`1m`) · **13 timeframes** on [ork.ad](https://ork.ad/) · **2,608,958** `1m` rows in the full archive
- Built for **backtesting**, **algorithmic trading** and **quantitative finance** workflows
- **Weekly refresh** — [ork.ad](https://ork.ad/) every **Sunday**; GitHub `1m` sample updated in sync

> **Sample on GitHub** · `ESP35_1m.csv` (88,451 rows, `2026-01-05` → `2026-07-03`). **Full archive on [ork.ad](https://ork.ad/)** — **2,608,958** `1m` rows (~127.14 MB), **13 timeframes** (``1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W``), `2008-09-10` → `2026-07-03`.

## Download sample

**[ESP35_1m.csv](https://github.com/ork-ad/esp35-1m-ohlcv-index-historical-data/blob/main/ESP35_1m.csv)** on GitHub ([raw CSV](https://raw.githubusercontent.com/ork-ad/esp35-1m-ohlcv-index-historical-data/main/ESP35_1m.csv)) · [GitHub Releases](https://github.com/ork-ad/esp35-1m-ohlcv-index-historical-data/releases) when the release workflow is active.

## GitHub Pages

Interactive chart & stats: **[https://ork-ad.github.io/esp35-1m-ohlcv-index-historical-data/](https://ork-ad.github.io/esp35-1m-ohlcv-index-historical-data/)**

## Sample vs full dataset

| | **Sample (this repo)** | **Full dataset ([ork.ad](https://ork.ad/))** |
|---|--:|---|
| Instrument | Spain 35 · Stock index | Spain 35 · Stock index |
| Timeframes | `1m` (sample) | **13** — `1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W` |
| 1m rows | 88,451 | **2,608,958** |
| Size | 4.97 MB | ~127.14 MB |
| Period | `2026-01-05` → `2026-07-03` | `2008-09-10` → `2026-07-03` |
| File | `ESP35_1m.csv` | ZIP on [ork.ad](https://ork.ad/) |
| Updates | Weekly (Sunday) — GitHub sample | Weekly (Sunday) — all timeframes |

## Timeframes on ork.ad

This GitHub repository ships a **`1m` evaluation sample** only. On **[ork.ad](https://ork.ad/)**, each full asset archive is delivered as a ZIP with **13 gap-free OHLCV timeframes** (one CSV per timeframe):

**1m** · **3m** · **5m** · **15m** · **30m** · **1H** · **2H** · **4H** · **8H** · **12H** · **16H** · **1D** · **1W**

GitHub = `1m` sample · [ork.ad](https://ork.ad/) = all **13** timeframes above for the same instrument.

## Weekly updates

- **[ork.ad](https://ork.ad/)** — Full datasets on ork.ad are updated every Sunday.
- **GitHub (this repo)** — GitHub samples are refreshed weekly (every Sunday), in sync with ork.ad.

When a new `1m` sample is published on GitHub, the README, chart preview and CSV reflect the latest week of data.

## Data preview

First and latest rows from the GitHub sample **`ESP35_1m.csv`**:

**First rows**

| time | open | high | low | close | volume |
| --- | --- | --- | --- | --- | --- |
| 2026-01-05T07:01:00Z | 17475.44 | 17632.5 | 17475.44 | 17616 | 13 |
| 2026-01-05T07:02:00Z | 17616 | 17616 | 17594.48 | 17601.49 | 21 |
| 2026-01-05T07:03:00Z | 17601.49 | 17601.49 | 17584.5 | 17588.48 | 12 |
| 2026-01-05T07:04:00Z | 17588.48 | 17596 | 17588.48 | 17592.48 | 11 |
| 2026-01-05T07:05:00Z | 17592.48 | 17592.48 | 17573.48 | 17587.48 | 13 |

**Last rows**

| time | open | high | low | close | volume |
| --- | --- | --- | --- | --- | --- |
| time | open | high | low | close | volume |
| 2026-07-03T17:44:00Z | 19835.96 | 19839.95 | 19835.95 | 19836.96 | 6 |
| 2026-07-03T17:45:00Z | 19836.96 | 19837.96 | 19836.96 | 19837.96 | 2 |
| 2026-07-03T17:47:00Z | 19837.96 | 19841.97 | 19837.95 | 19841.97 | 4 |
| 2026-07-03T17:48:00Z | 19841.97 | 19841.97 | 19836.95 | 19836.97 | 3 |

## Schema

```text
time,open,high,low,close,volume
```

## Code examples

### pandas

```python
import pandas as pd

df = pd.read_csv('ESP35_1m.csv', parse_dates=['time'])
df.set_index('time', inplace=True)
print(df.describe())
print(df.resample('1h').agg({'open': 'first', 'high': 'max',
                              'low': 'min', 'close': 'last', 'volume': 'sum'}).head())
```

### backtrader

```python
import backtrader as bt
import pandas as pd

df = pd.read_csv('ESP35_1m.csv', parse_dates=['time'])
df.set_index('time', inplace=True)

class PandasData(bt.feeds.PandasData):
    params = (('datetime', None), ('open', 'open'), ('high', 'high'),
              ('low', 'low'), ('close', 'close'), ('volume', 'volume'))

cerebro = bt.Cerebro()
cerebro.adddata(PandasData(dataname=df))
# cerebro.addstrategy(YourStrategy)
# cerebro.run()
```

### vectorbt

```python
import pandas as pd
import vectorbt as vbt

df = pd.read_csv('ESP35_1m.csv', parse_dates=['time'])
close = df.set_index('time')['close']
fast, slow = vbt.MA.run(close, 10), vbt.MA.run(close, 50)
entries = fast.ma_crossed_above(slow)
exits = fast.ma_crossed_below(slow)
pf = vbt.Portfolio.from_signals(close, entries, exits, init_cash=10_000, freq='1min')
print(pf.stats())
```

## Download full data

The complete **ESP35** archive on **[ork.ad](https://ork.ad/)** includes **13 OHLCV timeframes** (`1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W`) — **2,608,958** rows at `1m`, plus all other timeframes in the same ZIP.

**[→ Get the full ESP35 dataset on ork.ad](https://ork.ad/)**

---
*GetData · ESP35 1m OHLCV sample on GitHub · Full historical data on [ork.ad](https://ork.ad/) · 2026-07-06 UTC*