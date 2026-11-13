## 🌙 Post-Market Briefing: Friday, November 13, 2026

**Data notes (please read first)**
- **Retrieved:** 2026-11-13, 21:32–21:45 UTC (23:32–23:45 Bucharest; 16:32–16:45 ET).
- **Today's prices are provisional.** Massive (Polygon) refuses same-day bars on this plan ("today's data before end of day"), and its minute bars and `/v1/open-close` for today are also blocked. Today's open/high/low/close therefore come from **Twelve Data**. Its close is the last regular-session print (15:59 ET), not the official closing-auction price. Cross-checks against media quotes: MU $778.11 here vs. $778.31, NBIS $115.84 vs. $115.88, CRWV $53.11 vs. $53.13. Expect differences of a few cents.
- **History:** daily candles through Nov 12 are from Massive. All % changes are today's provisional close vs. the Massive Nov 12 close. "Week" is vs. the Nov 6 close.
- **Relative volume for today is NOT available.** Twelve Data's same-day volume is a partial feed (e.g. 731K shares for MU against a 30.8M 20-day average). I tested scaling it and the ratio is not stable, so I left it out. The table shows the confirmed Nov 12 relative volume for context. Any "on volume" call for today is **pending**.
- **After-hours:** Twelve Data extended quote with its own timestamp, taken about 40 minutes after the close. After-hours trading runs until 20:00 ET, so these are early prints.
- **Indicators:** computed by me from the candles: SMA 20/50/100/200, RSI(14, Wilder), MACD(12,26,9). They include today's provisional close. Intraday checks use 30-minute regular-session bars from Twelve Data.
- **Morning brief:** setups are checked against `reports/2026-11-13-market-intelligence.md`, which sits on branch `claude/pensive-clarke-fahuro` (not on this branch). The three extra candidates in that file are **CRDO, LUNR, KTOS**.
- **Labels:** **[Confirmed]** = SEC filing or company release. **[Reported]** = media. **[Est.]** = unconfirmed. **Opinion** = my analysis. Not personalised financial advice.

---

### 🧭 The day in three lines
1. **Chips and neoclouds sold off again.** SMH -3.0%, QQQ -1.2% and **QQQ closed back below its 200-day average** ($679.90 vs. $682.24). The 10-year yield reached about 5.17% intraday and the market fully prices a December Fed hike [Reported].
2. **NBIS -10% and CRWV -6%** on analyst target cuts for Nebius and a Bloomberg report that **Microsoft is cutting back the number of neocloud vendors it uses** [Reported].
3. **MU defended its 200-day average at the close ($778.11 vs. $765.61) but trades at $763.63 after hours, back below it.** Two morning setups triggered (MU, LUNR), one marginally (MRVL). **OUST fell 8.5% through its entry zone with no news.** No stop and no target was hit.

---

### 1. Session recap

| Ticker | Close (prov.) | % chg | Week | Open | High | Low (time ET) | After-hours (ET) | AH vs close | Rel. vol Nov 12 (context) |
|---|---|---|---|---|---|---|---|---|---|
| **SPY** | 754.27 | -0.38% | +2.6% | 759.99 | 760.08 | 747.94 (10:00) | 750.07 @ 16:41 | -0.6% | 0.77 |
| **QQQ** | 679.90 | -1.20% | +3.6% | 688.52 | 688.73 | 671.71 (11:00) | 674.57 @ 16:42 | -0.8% | 0.73 |
| **SMH** | 486.60 | -3.02% | +4.9% | 499.54 | 500.21 | 473.32 (11:00) | 481.51 @ 16:40 | -1.0% | 0.83 |
| RKLB | 61.53 | -3.96% | +15.9% | 63.70 | 64.21 | 59.80 (11:00) | 60.49 @ 16:40 | -1.7% | 0.63 |
| BKSY | 23.80 | +2.41% | +11.6% | 23.33 | 24.27 | 22.27 (09:30) | no post-close print | n/a | 1.23 |
| RDW | 7.74 | -3.67% | +7.3% | 7.96 | 8.04 | 7.46 (11:00) | 7.68 @ 16:38 | -0.7% | 0.88 |
| ASTS | 32.59 | -5.52% | +0.8% | 34.01 | 34.42 | 31.34 (11:00) | 32.14 @ 16:25 | -1.4% | 0.56 |
| MRVL | 156.75 | -4.68% | +11.0% | 161.83 | 163.88 | 149.19 (10:00) | 154.06 @ 16:37 | -1.7% | 0.72 |
| MU | 778.11 | -2.55% | +12.8% | 782.38 | 796.00 | 750.35 (11:00) | 763.63 @ 16:36 | -1.9% | 0.88 |
| VELO | 4.16 | -5.67% | -25.4% | 4.41 | 4.42 | 4.01 (11:00) | no post-close print | n/a | 1.31 |
| NBIS | 115.84 | -9.95% | -10.5% | 123.45 | 123.86 | 109.00 (10:00) | 113.76 @ 16:39 | -1.8% | 2.67 |
| CRWV | 53.11 | -6.17% | +14.5% | 56.01 | 56.36 | 49.25 (10:30) | 52.05 @ 16:40 | -2.0% | 1.44 |
| OUST | 33.48 | -8.54% | -3.8% | 36.25 | 36.25 | 32.43 (10:00) | 33.34 @ 16:06 | -0.4% | 0.57 |
| CRDO | 131.56 | -5.90% | +9.2% | 138.81 | 140.93 | 126.42 (10:00) | 129.00 @ 16:32 | -1.9% | 0.60 |
| LUNR | 13.00 | -0.23% | +24.2% | 13.14 | 13.45 | 12.00 (10:00) | no post-close print | n/a | 3.49 |
| KTOS | 33.91 | -2.42% | -3.4% | 34.69 | 34.91 | 33.36 (10:30) | no post-close print | n/a | 1.01 |

Low times are the start of the 30-minute bar that held the low.

- **Shape of the day:** every name except BKSY made its high in the first 30 minutes and its low between 10:00 and 11:30 ET, then ground higher into the close. The afternoon recovery was steady but shallow: most names closed in the lower half of their range.
- **After-hours is weaker, with no cause I could identify.** Every name with a post-close print is lower (MU -1.9%, CRWV -2.0%, CRDO -1.9%, NBIS -1.8%, QQQ -0.8%). A second source shows the same index drift (S&P -0.57%, Nasdaq-100 -0.78%) ([Stock Analysis](https://stockanalysis.com/markets/afterhours/)). I found no headline that explains it.
- **Indices [Reported]:** S&P 500 -0.40% to 7,561.67, Nasdaq Composite -0.91% to 25,136.27, Dow +0.10% to 52,347.55, Russell 2000 -0.31%. For the week the S&P gained about 2.5% and the Nasdaq about 2.3% ([CNBC](https://www.cnbc.com/2026/11/12/stock-market-today-live-updates.html), [Yahoo Finance](https://finance.yahoo.com/markets/live/stock-market-today-friday-november-13-dow-sp-500-nasdaq-nvidia-ppi-141451558.html)).
- **Chips [Reported]:** AMD about -9%, Broadcom about -5% to -6%, Intel about -5%. NVDA's move is reported as -2% by CNBC and "more than 4%" by Yahoo; I could not reconcile the two.
- **CRWV volume:** Twelve Data shows 121.7M shares for CRWV (20-day average 74.3M), but 65.8M of that sits in a single 30-minute bar at 14:30 ET with no price reaction. I treat it as **unverified**.

---

### 2. Morning setups: what happened

| Ticker | Morning plan | Result | Detail |
|---|---|---|---|
| **MU** | Buy $765–790; confirm a daily close above $763 plus a 1h higher low; stop $735 | ✅ **TRIGGERED** (at risk after hours) | Traded through the zone to $750.35 at ~11:00 ET, **below the 200 DMA intraday**. Hourly lows then rose every hour ($750 → $757 → $760 → $765 → $770) and it closed $778.11, above $763. Stop and targets untouched. **After-hours $763.63 is back at the confirmation line.** |
| **LUNR** | Buy $12.0–12.6 (breakout retest); stop $10.9 | ✅ **TRIGGERED** | Low was exactly $12.00. Spent 10:00–13:00 ET inside the zone, then closed $13.00, above the 50 DMA ($12.91). T1 $14.6 not reached. |
| **MRVL** | Conditional: $150–156 only if a 4h higher low holds above $147.8; stop $141 | ⚠️ **TRIGGERED (marginal)** | Low $149.19, under the zone but above $147.8. It also broke yesterday's low ($155.97), so the "higher low" is only vs. Nov 10 ($147.79). Closed $156.75. The morning signal was HOLD/MONITOR. |
| **RKLB** | Buy $59.5–62.5; confirm a 4h higher low, then a 1h close above the 1h EMA20; stop $56.5 | ⏸ **NOT TRIGGERED: in zone, no confirmation** | Low $59.80, closed $61.53 inside the zone. No hourly close got above the 1h EMA20 (~$62.4). It also closed back below the 50 DMA ($62.47). |
| **CRWV** | Buy $51–54; confirm a close above $50 plus a 4h bullish reversal candle; stop $47 | ⏸ **NOT TRIGGERED: confirmation incomplete** | Low $49.25, under both $50 and yesterday's $50.17 low. Closed $53.11, so the gap held on a closing basis, but the 09:30–13:30 4h bar closed red ($56.01 → $52.35). Stop not hit. |
| **CRDO** | Buy $128–134; confirm a 4h higher low above $126.9; stop $119.5 | ⏸ **NOT TRIGGERED: confirmation level broken** | Low $126.42, 48 cents under $126.9. Closed $131.56 inside the zone. Stop not hit. |
| **OUST** | Buy $34.0–35.7; confirm a 4h higher low or a 1h reclaim of the EMA20 in the zone; stop $31.4 | ❌ **NOT TRIGGERED: setup damaged** | Opened $36.25 and fell straight through the zone to $32.43 in the first hour. Never traded back above $33.94. Closed $33.48, below the zone, the 50 DMA ($35.61) and the $33.7 breakout level. Stop not hit. |
| **BKSY** | Buy $21–22 (gap retest); alternative: daily close above $24.92 on 1.5× volume | ⏸ **NOT TRIGGERED** | Low $22.27, 27 cents above the zone. High $24.27, close $23.80: no breakout. Only green name on the list. |
| **KTOS** | Only a sweep below $31.57 that reclaims it | ⏸ **NOT TRIGGERED** | Low $33.36. |
| **RDW** | No trade; reconsider on a daily close above $8.75 | ⏸ **NOT TRIGGERED** | Closed $7.74. |
| **ASTS** | No trade; reconsider on a close above $38.2, or a sweep below $27.6 that reverses | ⏸ **NOT TRIGGERED** | Closed $32.59. Low $31.34 broke the $31.96 support. |
| **NBIS** | No trade; long only if $113–119 holds **and** $141 is reclaimed | 🛑 **AVOID stands; support broke intraday** | Low $109.00, under the Nov 5 low ($113.30). Closed $115.84, back above it. |
| **VELO** | No trade | 🛑 **AVOID stands** | New low for the move at $4.01; closed $4.16. |

**No stop and no target was hit on any setup today.** Opinion: the dip was bought again, but with less conviction than Thursday. Three names (MU, MRVL, CRWV) undercut the levels they were supposed to hold before recovering, and the after-hours drift puts MU's trigger in doubt.

---

### 3. Earnings, filings and material news (Nov 13, incl. after-hours)

**Market-wide**
- **October PPI [Reported]:** +0.3% m/m against +0.4% expected (September was +1.3%). The annual rate is **+6.5%, the largest since November 2022**. I did not find the core figure ([CNBC](https://www.cnbc.com/2026/11/12/stock-market-today-live-updates.html)).
- **Rates [Reported]:** the 10-year yield reached about **5.17%** intraday, with closing readings of 5.13–5.15%. CME FedWatch shows a **100% chance of a hike on Dec 9**: about 87% for 25bp and 13% for 50bp. The dollar index is at its highest since April 2025 and Bitcoin fell below $70,000 ([CNBC](https://www.cnbc.com/2026/11/12/stock-market-today-live-updates.html), [Yahoo Finance](https://finance.yahoo.com/markets/live/stock-market-today-friday-november-13-dow-sp-500-nasdaq-nvidia-ppi-141451558.html)).
- **NVIDIA [Reported]:** HSBC cut NVDA to Hold with a $170 target (from $365). NVDA is down about 12% on the week. Results are still due **Tue Nov 17** after the close.

**NBIS**
- **Analyst target cuts [Reported]:** Baird to **$200 from $340** (Outperform kept), BofA to **$265 from $310** (Buy kept), DA Davidson to **$125 from $250** (Neutral kept). At least seven analysts cut targets after the Q3 report ([Yahoo Finance](https://finance.yahoo.com/markets/stocks/articles/nebius-sinks-13-baird-bofa-160453625.html), [Motley Fool](https://www.fool.com/investing/2026/11/13/why-nebius-group-stock-plunged-again-today/)).
- **Microsoft [Reported, Bloomberg via Motley Fool]:** Microsoft did not renew a cloud deal with Oracle and is reviewing its neocloud contracts to use fewer vendors and favour its own data centers. Nebius has a **$17.4B Microsoft contract running through 2031** ([Motley Fool](https://www.fool.com/investing/2026/11/13/microsoft-just-piled-onto-the-bad-news-for-neoclouds/)). I have not read the Bloomberg original.
- **Form 144 [Confirmed], filed after the close (21:24 UTC):** a trust of director John Boynton plans to sell 4,502 shares (~$579K) under a 10b5-1 plan adopted in March ([144](https://www.sec.gov/Archives/edgar/data/1513845/000195004726011076/xsl144X01/primary_doc.xml)). Minor.

**CRWV**
- **Microsoft [Reported]:** same report as above. Microsoft was **36% of CoreWeave's Q2 revenue**, which makes this the most important item for CRWV today ([Motley Fool](https://www.fool.com/investing/2026/11/13/microsoft-just-piled-onto-the-bad-news-for-neoclouds/)).
- No SEC filing today. The $4B+ loan reported on Nov 11 has not been announced.

**MRVL**
- Three Form 3 filings [Confirmed] for the directors who joined on Nov 12 ([example](https://www.sec.gov/Archives/edgar/data/1835632/000162828026073725/xslF345X06/wk-form3_1794598327.xml)). Routine. No other company news; the drop followed the chip sector.

**MU**
- **No material news** and no SEC filing today. The move was sector read-through from NVIDIA [Reported] ([Motley Fool](https://www.fool.com/investing/2026/11/13/why-micron-stock-was-sliding-today/)).

**KTOS**
- **Form 144 [Confirmed]:** officer Steven Fendley plans to sell 14,000 shares (~$486.5K) ([144](https://www.sec.gov/Archives/edgar/data/1069258/000195917326007996/xsl144X01/primary_doc.xml)). Minor.

**LUNR**
- 10-Q for Q3 filed late on Nov 12 (22:33 UTC) [Confirmed] ([10-Q](https://www.sec.gov/Archives/edgar/data/1844452/000162828026073512/lunr-20260930.htm)). I have not reviewed it for changes vs. the earnings release.

**RDW**
- No filing today. Commentary today covers a roughly **$40M NASA award** for a lunar power system that Redwire disclosed on Tuesday Nov 10 [Reported] ([Zacks](https://www.zacks.com/stock/news/3029636/can-redwire-s-40m-nasa-deal-boost-lunar-power-capabilities)). This was not in the morning brief.

**OUST**
- **No material news.** No filing and no headline explains the 8.5% drop. Opinion: with no catalyst, it looks like a high-beta name giving back part of a 43% run (Nov 5 low $28.16 to Nov 10 high $40.38) in a weak tape.

**RKLB, BKSY, ASTS, VELO, CRDO:** **No material news.** No 8-K, Form 4, S-3 or ATM filing on EDGAR for any of them on Nov 12–13 (checked at 21:40 UTC). Space names fell with the sector ([TIKR](https://www.tikr.com/blog/ast-spacemobile-sinks-6-rocket-lab-down-5-as-space-stocks-give-back-a-stellar-week)).

---

### 4. Technical update (daily, includes today's provisional close)

| Ticker | Close | 20 DMA | 50 DMA | 100 DMA | 200 DMA | RSI(14) | MACD line / signal | MACD histogram (prev) |
|---|---|---|---|---|---|---|---|---|
| SPY | 754.27 | 759.02 ↓ | 764.43 ↓ | 760.28 ↓ | 731.92 ↑ | 47.0 | -4.13 / -4.09 | -0.04 (-0.29) |
| QQQ | 679.90 | 695.45 ↓ | 717.87 ↓ | 714.45 ↓ | 682.24 ↓ | 42.8 | -12.92 / -12.83 | -0.09 (-0.54) |
| SMH | 486.60 | 518.13 ↓ | 559.80 ↓ | 567.58 ↓ | 523.89 ↓ | 40.1 | -22.75 / -21.90 | -0.85 (-1.29) |
| RKLB | 61.53 | 55.78 ↑ | 62.47 ↓ | 68.86 ↓ | 78.28 ↓ | 52.9 | -0.22 / -1.90 | +1.68 (+1.81) |
| BKSY | 23.80 | 19.45 ↑ | 20.56 ↑ | 22.98 ↑ | 27.01 ↓ | 63.6 | 0.90 / 0.08 | +0.82 (+0.86) |
| RDW | 7.74 | 8.16 ↓ | 9.56 ↓ | 10.16 ↓ | 10.87 ↓ | 43.0 | -0.48 / -0.56 | +0.08 (+0.09) |
| ASTS | 32.59 | 37.81 ↓ | 49.70 ↓ | 58.25 ↓ | 73.62 ↓ | 36.8 | -4.58 / -4.87 | +0.30 (+0.35) |
| MRVL | 156.75 | 194.75 ↓ | 229.21 ↓ | 225.51 ↓ | 187.00 ↓ | 35.2 | -24.27 / -21.88 | -2.39 (-3.38) |
| MU | 778.11 | 837.99 ↓ | 943.77 ↓ | 943.00 ↓ | 765.61 ↑ | 42.4 | -55.05 / -53.63 | -1.42 (-4.27) |
| VELO | 4.16 | 6.04 ↓ | 8.41 ↓ | 10.67 ↓ | 12.86 ↓ | 29.3 | -1.06 / -1.01 | -0.04 (-0.00) |
| NBIS | 115.84 | 151.12 ↓ | 194.60 ↓ | 204.14 ↓ | 179.35 ↓ | 35.8 | -19.05 / -18.37 | -0.68 (+0.19) |
| CRWV | 53.11 | 54.99 ↓ | 72.60 ↓ | 79.20 ↓ | 88.99 ↓ | 43.1 | -5.70 / -7.00 | +1.30 (+1.26) |
| OUST | 33.48 | 32.28 ↑ | 35.61 ↓ | 38.48 ↓ | 32.87 ↑ | 48.3 | 0.22 / -0.56 | +0.78 (+1.10) |
| CRDO | 131.56 | 149.05 ↓ | 172.28 ↓ | 202.22 ↓ | 180.86 ↓ | 40.5 | -14.42 / -14.51 | +0.10 (-0.16) |
| LUNR | 13.00 | 11.03 ↑ | 12.91 ↑ | 14.49 ↓ | 19.30 ↓ | 57.0 | -0.16 / -0.61 | +0.45 (+0.41) |
| KTOS | 33.91 | 38.34 ↓ | 42.11 ↓ | 47.21 ↓ | 60.11 ↓ | 35.3 | -2.09 / -1.84 | -0.24 (-0.17) |

↑ = close above the average, ↓ = close below. Volume confirmation is pending for every item below (see data notes).

**Breakouts / breakdowns and levels that changed**
- **QQQ: closed below the 200 DMA** ($679.90 vs. $682.24) after two closes above it. Low $671.71. After-hours $674.57. Next support is the Nov 5 low at $647. Resistance $688.7, then the 20 DMA at $695.5.
- **SMH:** -3.0% and still under its 200 DMA ($523.89). Low $473.32. The Nov 5 low at $445.6 is the level that matters below.
- **NBIS: breakdown continues.** MACD crossed back below its signal line. It lost yesterday's $118.81 low and briefly the Nov 5 low ($113.30). New support **$109.00**. Resistance $118.8, then **$123.9** (today's high), then $132.7.
- **OUST: failed breakout retest.** Closed under the 50 DMA ($35.61) and the $33.7 breakout level. It still holds the 200 DMA ($32.87) and 20 DMA ($32.28); today's low of $32.43 sat between them. Resistance $33.9, then $35.6–36.25.
- **MU: 200 DMA pierced intraday, defended at the close.** Low $750.35 vs. the 200 DMA at $765.61. New support **$750.35**; below that $745, then $700. Resistance $783.9–796.0, then $827.6. The after-hours print ($763.63) is below the 200 DMA.
- **RKLB: lost the 50 DMA** ($62.47). Support $59.80, then $58–59 (Nov 9 gap). Resistance $62.5, then $64.2.
- **CRWV: lost the 20 DMA** ($54.99) and undercut the gap support. New support **$49.25**, then $48.7. Resistance $53.7–55.0, then $56.4.
- **MRVL:** broke yesterday's low. New support **$149.19**, then $147.8. Resistance $158.1, then $163.9. MACD histogram still negative but improving.
- **CRDO:** MACD histogram turned slightly positive (+0.10). Support $126.4. Resistance $132.6, then $140.9.
- **ASTS:** broke the $31.96 support (low $31.34). Next support is the 52-week low at $27.58.
- **VELO:** new low for the move at $4.01. Twelve Data shows $4.01 as the 52-week low; my Massive history shows an older $3.75 low, so the sources conflict. RSI 29.
- **BKSY:** the only name above its 20, 50 and 100 DMA. Resistance $24.27, then **$24.92**. Support $22.2–23.0.
- **LUNR:** retest of the $12.0–12.6 breakout area held, with a close back above the 50 DMA ($12.91). Resistance $13.45, then $14.62.
- **RDW:** below every average. Support $7.46, then $7.0–7.2. **KTOS:** MACD histogram worsening; support $33.36, then $31.57.
- **No watchlist name broke out to the upside today.**

---

### 5. Plan for Monday, Nov 16

Levels are opinion. "Open" means the morning setup triggered today on paper; I do not know whether you took it.

| Ticker | Signal | Entry zone / trigger | Stop | Targets | Note |
|---|---|---|---|---|---|
| **MU** | 🟡 **SETUP OPEN, needs Monday to hold** | No new entries unless Monday holds above **$750.35** and reclaims $766 (200 DMA) on an hourly close. Then $755–780. | $735 | $855 / $945 | After-hours is under the 200 DMA. A daily close below $763 cancels the morning confirmation. Do not add before NVDA (Tue). |
| **LUNR** | 🟡 **SETUP OPEN** | $12.0–12.6 on a pullback; no chase above $13.5 | $10.9 | $14.6 / $16.2 | Best-behaved extra candidate today. |
| **BKSY** | ⏳ **WAIT FOR RETEST** | $21–22, or a daily close above $24.92 on 1.5× volume | $19.6 | $24.9 / $28.3 | Strongest chart on the list. |
| **RKLB** | ⏳ **WAIT: in zone, unconfirmed** | $59.5–62.5, only after an hourly close above ~$62.5 with $59.80 holding | $56.5 | $68.3 / $78 | A close below $59.5 points to the $58–59 gap. |
| **CRWV** | ⏳ **WAIT: unconfirmed** | $51–54, only after a daily close above $55.0 (20 DMA) or an hourly higher low above $49.25 | $47 | $62 / $73 | Half size at most. The Microsoft report is a real risk to the thesis, not only to the chart. |
| **CRDO** | ⏳ **WAIT (downgraded from Potential Buy)** | $128–134, only if Monday's low stays above $126.4 | $119.5 | $151 / $175 | Confirmation level broke today; moves with SMH. |
| **MRVL** | 👀 **HOLD / MONITOR** | $150–156 while $147.8 holds | $141 | $174.5 / $188 | Marginal trigger today. Earnings Dec 1; Lumentum deal overhang. |
| **OUST** | 👀 **HOLD / MONITOR (downgraded from Potential Buy)** | Either a daily close back above $35.6, or a reversal candle at $32.3–32.9 (20/200 DMA) | $31.4 | $38.4 / $40.4 | Today's drop had no news behind it. A close below $32.3 breaks the structure. |
| **RDW** | 👀 **HOLD / MONITOR** | Daily close above $8.75 | n/a | $9.45 | Leaning avoid. |
| **KTOS** | 👀 **HOLD / MONITOR** | A sweep below $31.57 that reclaims it; zone $31.6–33.0 | $29.9 | $38.1 / $44.1 | Drifting toward the trigger. |
| **NBIS** | ⛔ **AVOID / HIGH RISK** | No entry. First sign of repair: 2–3 sessions holding $109 and a daily close above $123.9 | n/a | Resistance $118.8 / $123.9 / $132.7 | A daily close below $109 opens a new leg down. |
| **ASTS** | ⛔ **AVOID / HIGH RISK** | Daily close above $38.2, or a sweep below $27.6 that reverses the same day | n/a | n/a | Lost $31.96 support. |
| **VELO** | ⛔ **AVOID / HIGH RISK** | None | n/a | n/a | Revisit only after a base above $4.0 and a reclaim of $5.4. |

**Key events**
- **Mon Nov 16:** I found no confirmed high-impact US release or watchlist earnings for Monday. One calendar lists a single high-impact event without naming it ([Thrive in Markets](https://thriveinmarkets.com/calendar/2026-11-16/)). Fed speakers for Monday: not verified.
- **Tue Nov 17, 8:30 am ET (15:30 Bucharest): October retail sales** [Reported]; consensus about +0.2% m/m [Est.].
- **Tue Nov 17, after the close: NVIDIA Q3 FY27 results** [Confirmed date]. Guidance was $108.0B ±2%; consensus is about $109B revenue and $2.47–2.49 EPS [Est.]. First report under the interim CEO, so the outlook and commentary matter more than the quarter.
- **Wed Nov 18, 2:00 pm ET (21:00 Bucharest): FOMC minutes** from the October meeting [Reported].
- **Wed Nov 18: Anthropic IPO pricing, Nasdaq ticker ANT** [Reported, from week-ahead previews; date not confirmed by a filing I read] ([Kitco/Reuters](https://www.kitco.com/news/off-the-wire/2026-11-13/wall-st-week-ahead-nvidia-results-anthropic-ipo-pose-tests-tumultuous)).
- **Thu Nov 19:** Walmart earnings [Reported, single source].
- **Still pending:** CoreWeave's reported $4B+ loan launch; MRVL earnings Dec 1; FOMC Dec 9.

**Stance (opinion):** no new size on Monday. QQQ is back under its 200-day average, SMH never reclaimed its own, the after-hours tape is soft, and NVIDIA reports the next evening. The two open setups (MU, LUNR) are worth holding only while MU stays above $750 and LUNR above $12.0. Among the names waiting for confirmation, BKSY and LUNR are showing relative strength; the neoclouds (NBIS, CRWV) now carry a customer-concentration question on top of the rate problem.

---

*Sources are linked inline. Today's prices are provisional Twelve Data values; history is from Massive. Facts are labeled; levels, signals and the stance are opinion, not personalised investment advice.*
