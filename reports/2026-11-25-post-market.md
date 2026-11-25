## 🌙 Post-Market Briefing: Wednesday, November 25, 2026

**Prepared:** ~23:45 EET (21:30–22:00 UTC), after the US close. The morning plan being graded is [reports/2026-11-25-market-intelligence.md](https://github.com/kapi-5678/site/blob/claude/pensive-clarke-8omlha/reports/2026-11-25-market-intelligence.md), which sits on branch `claude/pensive-clarke-8omlha`.

**Price data:**
- **Today's OHLC and 1h bars** come from Twelve Data, retrieved 21:35–21:45 UTC.
  - Massive (Polygon) returned `NOT_AUTHORIZED` for today's `/v1/open-close` and same-day minute bars. Its plan has no same-day data.
  - **Caveat:** Twelve Data's "close" is the last regular-session trade it received. It can differ from the official closing-auction print. Example: MU shows **$604.16** here, but Motley Fool shows **$601.25**. Treat closes as accurate to within about ±0.5%.
- **History through Tue Nov 24** comes from Massive daily candles.
- SMA 20/50/100/200, RSI(14, Wilder), MACD(12,26,9) and ATR(14) are computed in-house on that history plus today's close.

**Data gaps:**
- **After-hours prices are unavailable tonight.**
  - Massive blocks same-day data.
  - Twelve Data's extended-hours data needs a higher plan (HTTP 403: "Pre-market and post-market data are available on the Pro plan").
  - No AH price is shown, rather than inventing one.
  - None of the 13 tickers had an earnings release or 8-K after the bell (see §3).
- **Relative volume** is shown only where the feed's volume looks consolidated.
  - It is n/a for QQQ (1.5M), SMH (0.6M), RKLB (0.5M), BKSY (0.06M) and VELO, where the feed volume is clearly partial.
  - It is also n/a for SPY (217M, 3.5× average). That is implausible for this feed, and the same reading was flagged yesterday.

**Labels:** **[FACT]** = sourced or computed from data · **[EST]** = estimate or unconfirmed · **[VIEW]** = my analysis or opinion. Not personalised financial advice.

---

### 🧭 What happened today

- **[FACT] There was a gap-down washout, then a near-complete intraday reversal.**
  - **Nasdaq Composite:** fell as much as **−4.6%** intraday, then closed **−0.6% at 23,585.80**.
  - **SOX chip index:** fell as much as **−8.0%**, then closed **−0.7%** after recovering about 92% of the drop.
  - **S&P 500:** −0.3%, after a −3.2% low.
  - **Dow:** +0.3%, after a −2.2% low.
  - **10-year yield:** ~4.87%, down from ~4.90%.
  - Source: [TECHi close recap](https://www.techi.com/chip-stocks-recover-early-slide-nasdaq-close-november-25/).
- **[FACT] Drivers cited for the early slide:**
  - **Tariff risk:** Reuters reported that findings from a trade investigation into **16 economies including Taiwan and South Korea** were about to be released, with new tariffs expected. Nothing had been posted by the close.
  - **Hot inflation:** **October PCE was +3.8% y/y.**
  - **Follow-through selling from Tuesday.**
  - AI credit-risk worries (CDS widening) were also cited **[EST, secondary sources]** ([Finexus](https://api.finexus.net/api/news/earnings/129662/html)).
- **[FACT] Memory-specific pressure:**
  - **TrendForce** said Chinese cloud providers have **cut 2027 memory orders** and warned of NAND oversupply and a downward pricing cycle.
  - MU fell as much as about 13% intraday. It recovered to about −4% to −4.5%.
  - TrendForce still expects DRAM to stay undersupplied in 2027.
  - Source: [Motley Fool](https://www.fool.com/investing/2026/11/25/why-micron-stock-just-dropped-again/).
- **[FACT] The Nov 20 lows held for SPY and QQQ:**
  - **SPY:** low $695.47 vs. the $686.75 line.
  - **QQQ:** low $607.81 vs. the $606.23 line, a $1.58 margin.
  - **SMH undercut** its Nov 20 low ($393.88 vs. $396.85), then closed at **99% of its daily range**.
- **[VIEW] This is the first constructive daily candle of the drawdown.** It is a broad-based hammer or failed breakdown: the indices made a lower open and a higher close, and SMH reclaimed the Nov 20 low.
  - **It is not a trend change.** Every index is still below its 20-, 50- and 200-day SMAs, and MACD is negative.
  - A reversal candle **needs follow-through.** Friday is a thin half-day and Thursday is closed, so the real test is **Mon Nov 30 and MRVL earnings on Dec 1**.

---

### 1️⃣ Session recap

| Ticker | Close | % chg | Open | High | Low | Close in range | AH price | RVOL |
|---|---|---|---|---|---|---|---|---|
| **SPY** | 716.76 | −0.28% | 703.20 | 718.43 | **695.47** | 93% | n/a (feed) | n/a |
| **QQQ** | 633.92 | −0.66% | 617.09 | 634.85 | **607.81** | 97% | n/a | n/a |
| **SMH** | 422.60 | −0.97% | 402.63 | 422.88 | **393.88** | **99%** | n/a | n/a |
| RKLB | 47.02 | **+2.26%** | 43.78 | 48.14 | 42.14 | 81% | n/a | n/a |
| BKSY | 15.95 | −2.80% | 15.46 | 16.64 | **14.65** ⚠️ 52-wk low | 65% | n/a | n/a |
| RDW | 5.88 | −0.25% | 5.61 | 6.08 | 5.39 | 72% | n/a | 1.56 |
| **ASTS** | **26.00** | **+10.19%** | 22.68 | 26.66 | **22.50** ⚠️ 52-wk low | 84% | n/a | 1.20 |
| MRVL | 130.90 | −0.51% | 122.63 | 130.99 | 117.80 | 99% | n/a | 0.74 |
| **MU** | 604.16* | −4.07%* | 574.92 | 604.78 | **548.13** | 99% | n/a | 1.37 |
| VELO | 3.16 | +5.33% | 2.88 | 3.27 | **2.755** ⚠️ 52-wk low | 78% | n/a | n/a |
| NBIS | 84.97 | −2.68% | 80.50 | 87.28 | 75.60 | 80% | n/a | 1.19 |
| CRWV | 42.54 | −0.15% | 39.13 | 43.02 | **37.40** ⚠️ 52-wk low | 91% | n/a | 1.10 |
| OUST | 25.75 | **+3.02%** | 23.36 | 26.54 | 22.25 | 81% | n/a | 0.88 |
| **KTOS** | **28.95** | **+2.62%** | 27.31 | 29.35 | 26.83 | 84% | n/a | 0.73 |
| CRDO | 106.77 | +0.29% | 99.00 | 106.77 | 93.28 | 100% | n/a | 0.86 |
| PL | 10.62 | −0.23% | 10.17 | 10.89 | **9.71** ⚠️ 52-wk low | 77% | n/a | 0.81 |

**Notes:**
- \* MU's official close is reported as **$601.25 (−4.53%)** by Motley Fool. The Twelve Data value is the last 15:59 print.
- All other values are [FACT] from Twelve Data. % change is measured against the Massive Nov 24 close.
- RVOL is today's feed volume divided by the 20-day Massive average, and is **unverified**.
- **[VIEW]** Five names printed **new 52-week lows intraday and then reversed**: BKSY, ASTS, VELO, CRWV and PL. That pattern looks like capitulation. **ASTS (+10% on 1.2× volume)** and **RKLB, OUST and KTOS** (green on a red index day) showed the best relative strength.

---

### 2️⃣ Morning setups: scorecard

| Ticker | Morning plan | What happened (1h bars) | Status |
|---|---|---|---|
| **MU** | Buy $590–615 **only** on a 4H reversal that holds above $585. Stop **$555**. Plan cancelled on a close below $585. | Gapped to $574.92, below the zone. The low was **$548.13, below the $555 stop**. Rallied to close at about $601–604, inside the zone. | **INVALIDATED.** The stop level traded before any confirmation. A buy at the open was not possible because price opened under the $585 condition. The close above $585 does not revive the original plan. |
| **OUST** | Buy $23.60–25.00 after a 4H higher low above $23.60 and a 1H close above $25.20. Stop **$22.30**. | Opened $23.36 below support. The low was **$22.25, $0.05 below the stop**. The first 1H close above $25.20 came at 12:30 ($25.38). Closed $25.75. | **INVALIDATED.** The stop traded by 5 cents before the higher low formed. The later VWAP reclaim was not a valid entry under the plan. |
| **BKSY** | Buy $15.50–16.40 on a reversal **holding above $15.07**. Stop $14.40. | **New 52-week low $14.65.** The $15.07 hold failed. The stop was not hit (by $0.25). Bounced to $16.64, then faded to $15.95. | **NOT TRIGGERED.** The confirmation condition failed. The stop held, so the idea survives with new levels (see §5). |
| **KTOS** | Confirmation is a daily close above **$29.75**. Zone $26.60–28.20. Stop $25.40. | Low $26.83 **held above $26.60**, forming a higher low. High $29.35, close $28.95. | **NOT TRIGGERED.** The higher-low part is done, but the close above $29.75 is still missing. |
| **RKLB** | Buy $44.00–45.50 on a 4H reversal **and** a hold above $43.89. Stop $41.90. | Opened $43.78. The low was $42.14 (the $43.89 hold failed, but the stop held). Reversed to close at $47.02, above the zone. | **NOT TRIGGERED.** The hold condition failed. The stop was not hit. |
| **NBIS** | Buy $80.70–84 on a higher low above $80.67. Stop $73. | The low was **$75.60**, breaking $80.67. The stop held. Closed $84.97. | **NOT TRIGGERED.** No higher low formed. |
| **MRVL** | No position before Dec 1 earnings. Breakdown watch at $120.56. | Undercut to $117.80, then closed at $130.90 (99% of range). | **No trade (by design).** The $120.56 support was undercut, then reclaimed. |
| **CRDO** | Wait for earnings. Zone $98–104 if the Nov 20 low holds. | The low was $93.28, below $97.92. Closed at the high, $106.77. | **NOT TRIGGERED.** The Nov 20 low failed intraday. |
| **PL** | Buy $10.35–10.80 on a hold of $10.35. Stop $9.70. | **New 52-week low $9.71**, $0.01 above the stop. Closed $10.62. | **NOT TRIGGERED.** The hold failed. The stop survived by one cent. |
| **ASTS** | Avoid. Reclaim trigger is a close above **$27.40**. | New low $22.50, then +10%. High $26.66, close $26.00. | **NOT TRIGGERED.** Still below $27.40. |
| **CRWV** | Avoid. Reclaim above $51.90. Breakdown below $39.28. | **New 52-week low $37.40**, then reclaimed $39.28. Closed $42.54. | **Breakdown alert triggered intraday, then reversed.** No trade. |
| **RDW / VELO** | Avoid. | VELO made a new low of $2.755. RDW held above $5.12. | No trade. |

**Intraday monitoring triggers:**
- **SPY and QQQ held their breakdown lines.**
- **Hit intraday and then reclaimed:** MU < $585, NBIS < $80.67, CRWV < $39.28, BKSY < $15.07, OUST < $23.60.
- **Not hit:** KTOS < $26.60.
- **Not triggered:** the KTOS close above $29.75, the RKLB close above $50.70 and the ASTS close above $27.40.

**[VIEW] Lesson:** today was a stop-hunt day. Every "hold above X" condition failed in the first hour, then price recovered. Morning stops that sat just below an obvious low (OUST at $22.30, MU at $555) were taken out. Tomorrow's plans put stops **below today's washout lows**, not just below the Nov 20 lows.

---

### 3️⃣ News, filings and earnings (today, incl. after-hours)

| Ticker | Item | Type |
|---|---|---|
| **MU** | **[FACT]** TrendForce says Chinese cloud providers cut 2027 memory orders, NAND is oversupplied and pricing is heading down; DRAM stays undersupplied. MU fell as much as about 13% intraday. [Motley Fool](https://www.fool.com/investing/2026/11/25/why-micron-stock-just-dropped-again/). **[FACT]** The DEF 14A proxy and the annual report were filed **Nov 24**. These are routine. [EDGAR](https://www.sec.gov/Archives/edgar/data/723125/000072312526000034/0000723125-26-000034-index.htm) | Industry data, negative |
| **ASTS** | **[FACT] Form 4 (filed Nov 24):** Director **Adriana Cisneros bought 43,564 shares on Nov 20 at about $23.54 (~$1.03M)** on the open market. [EDGAR](https://www.sec.gov/Archives/edgar/data/1780312/000110465926131559/0001104659-26-131559-index.htm). Media tie today's +10% to insider dip-buying plus a rebound from the 52-week low. [24/7 Wall St.](https://247wallst.com/investing/2026/11/25/ast-spacemobile-surges-9-erasing-early-losses-as-space-stocks-diverge-spacex-eases-rocket-lab-holds-steady/), [Unusual Whales](https://unusualwhales.com/news/ast-spacemobile-stock-rebounds-from-52-week-low-2026-11-25). There is still **no confirmed BlueBird 14–16 launch date**. | Insider buy, positive |
| **RKLB** | **[FACT] Five Form 4s (filed Nov 25):** the CFO, COO, President, General Counsel and Controller sold shares on Nov 23 at about $48.9–51.7. The footnotes say these were **"sell-to-cover" sales under a Rule 10b5-1 election** to pay RSU tax withholding, so they are **not discretionary**. Form 144s were also filed. [EDGAR example](https://www.sec.gov/Archives/edgar/data/1819994/000200101126000153/0002001011-26-000153-index.htm) | Insider, neutral |
| **BKSY** | **[FACT] S-8 (filed Nov 24)** registers shares for the inducement grants tied to the EpochGeo acquisition (up to 565K RSUs, previously disclosed). [EDGAR](https://www.sec.gov/Archives/edgar/data/1753539/000175353926000170/0001753539-26-000170-index.htm) | Minor dilution, known |
| **PL** | **[EST]** A Zacks note on European defense expansion is commentary only, not a company release. [Zacks](https://www.zacks.com/stock/news/3034959/pl-expands-european-defense-footprint-a-new-growth-opportunity-ahead) | Commentary |
| **NBIS** | Commentary only ("fell despite 571% revenue growth"). No release. [Motley Fool](https://www.fool.com/investing/2026/11/25/nebius-stock-fell-despite-571-revenue-growth-here-s-why/) | No material news |
| **RDW, VELO, MRVL, CRWV, OUST, KTOS, CRDO** | No 8-K, S-3/ATM, Form 4 or company release dated Nov 25 was found on EDGAR or in the Massive news feed. (MRVL had a Form 4 on Nov 24 and CRDO had one on Nov 23. RDW's Nov 23 Form 4 is the CEO buy already covered this morning.) | **No material news** |
| **After-hours** | No watchlist company reported earnings or filed an 8-K after the bell. The trade findings on Taiwan and Korea (tariffs) **had not been posted** at the close **[FACT, TECHi]**. | — |

---

### 4️⃣ Technical update (daily close vs. moving averages)

| Ticker | Close | SMA20 | SMA50 | SMA100 | SMA200 | RSI(14) | MACD hist (vs prior) | Read **[VIEW]** |
|---|---|---|---|---|---|---|---|---|
| SPY | 716.76 | 740.33 | 757.89 | 758.54 | 733.16 | 39.9 | −2.91 (−3.53) ↑ | Below all MAs; hammer at $695; histogram improving |
| QQQ | 633.92 | 666.73 | 707.05 | 708.46 | 683.50 | 38.6 | −2.50 (−2.81) ↑ | Nov 20 low defended by $1.58 |
| SMH | 422.60 | 476.60 | 541.12 | 553.62 | 525.65 | 37.0 | −3.26 (−3.33) ↑ | Failed breakdown below $396.85; bullish if it holds |
| RKLB | 47.02 | 54.48 | 60.40 | 65.48 | 77.33 | 39.8 | −0.95 (−0.95) → | Outside-day reversal; below all MAs |
| BKSY | 15.95 | 19.90 | 20.19 | 22.34 | 26.86 | 36.7 | −0.66 (−0.58) ↓ | New 52-week low; weak close; MACD still falling |
| RDW | 5.88 | 7.30 | 8.86 | 9.77 | 10.72 | 35.4 | −0.10 (−0.11) → | Inside range; no signal |
| ASTS | 26.00 | 31.79 | 44.04 | 53.92 | 70.50 | 36.2 | −0.08 (−0.32) ↑ | **Bullish reversal on volume from a new low**; MACD near a bull cross |
| MRVL | 130.90 | 154.96 | 215.01 | 215.38 | 189.41 | 35.1 | **+0.23 (−0.07)** | **MACD bullish cross**; hammer |
| MU | 604.16 | 742.95 | 895.53 | 910.87 | 776.49 | 35.8 | −7.58 (−6.09) ↓ | Hammer, but momentum still falling; below the 200-day |
| VELO | 3.16 | 4.66 | 7.23 | 9.63 | 12.46 | 30.8 | −0.02 (−0.05) ↑ | Oversold bounce from a new low |
| NBIS | 84.97 | 122.68 | 174.12 | 192.95 | 179.74 | 33.1 | −1.76 (−2.03) ↑ | Undercut $80.67, then reclaimed |
| CRWV | 42.54 | 49.58 | 65.72 | 75.58 | 87.26 | 38.9 | +0.13 (+0.17) | New low $37.40, then reclaimed |
| OUST | 25.75 | 31.23 | 34.42 | 36.66 | 33.18 | 39.9 | −0.78 (−0.82) ↑ | Shakeout to $22.25, then closed above Nov 24 close and VWAP |
| KTOS | 28.95 | 34.26 | 39.23 | 45.53 | 57.45 | 32.7 | −0.42 (−0.58) ↑ | **Higher low ($26.83 > $26.60)**; resistance $29.35–29.75 |
| CRDO | 106.77 | 128.64 | 164.87 | 191.07 | 180.86 | 38.1 | −0.48 (−0.51) ↑ | Closed at the high of the day |
| PL | 10.62 | 12.67 | 14.53 | 18.07 | 25.58 | 33.7 | −0.17 (−0.17) → | New low $9.71, then recovered |

**Breakouts and breakdowns:** No ticker closed above a moving average. There were no closing breakdowns: every intraday break of support (MU $585, NBIS $80.67, CRWV $39.28, BKSY $15.07, OUST $23.60, CRDO $97.92, PL $10.35, SMH $396.85) **closed back above** the level.

**Levels that changed:**
- **New washout lows (key support from now on):**
  - Indices: SPY **$695.47** · QQQ **$607.81** · SMH **$393.88**.
  - Watchlist: MU **$548.13** · NBIS **$75.60** · CRWV **$37.40** · OUST **$22.25** · BKSY **$14.65** · ASTS **$22.50** · RKLB **$42.14** · MRVL **$117.80** · CRDO **$93.28** · KTOS **$26.83** · PL **$9.71** · VELO **$2.755**.
- **Confirmation highs to beat:** SPY $720.93 / QQQ $648.00 / SMH $442.88 (the Nov 24 highs).

---

### 5️⃣ Plan for tomorrow (next session: **Fri Nov 27, half-day, 1:00 PM ET close**)

> **[VIEW] General stance: WAIT and keep sizes small.** One reversal candle before a holiday, on thin volume, is not confirmation. Friday's half-session is a poor venue for new entries. Use it to see whether today's lows hold. The decisive sessions are **Mon Nov 30 and the MRVL print on Dec 1**. If Friday closes **below today's lows** (SPY $695 / QQQ $607.8), the reversal has failed and you should stand aside.

| Ticker | Signal | Entry zone / trigger | Stop | T1 / T2 | R/R (from) |
|---|---|---|---|---|---|
| **KTOS** | **POTENTIAL BUY** ⬆ (best structure) | **Trigger:** daily close above **$29.75**, then buy pullbacks into **$27.80–28.80** | $26.40 | $31.70 / $34.25 | 1.8 / 3.1 (from $28.30) |
| **OUST** | **POTENTIAL BUY** (reset) | **$23.80–24.80**, on a retest that holds above $23.60. Or a daily close above $26.54 | $22.00 | $28.75 / $31.20 | 1.9 / 3.0 (from $24.30) |
| **BKSY** | **POTENTIAL BUY** (conditional) | **$15.20–16.00**, only after a **daily close above $16.64** confirms the $14.65 low | $14.40 | $18.75 / $19.90 | 2.1 / 2.9 (from $15.80) |
| **ASTS** | HOLD / MONITOR ⬆ (from Avoid) | Close above **$27.40** on above-average volume. A confirmed launch date would add conviction | $24.40 | $31.80 / $35.00 | 1.3 / 2.3 (from $27.60) |
| **RKLB** | HOLD / MONITOR | **$44.50–46.00** pullback holding above $44; add on a close above $48.14 | $41.90 | $50.70 / $54.50 | 1.6 / 2.8 (from $45.25) |
| **MU** | HOLD / MONITOR ⬇ (from Potential Buy) | No entry until the TrendForce NAND news is absorbed. Watch **$585–610** holding above $585 into Dec 17 earnings | $545 | $672 / $707 | 1.3 / 1.9 (from $600), **poor** |
| **MRVL** | HOLD / MONITOR | **No position before Dec 1 earnings (after close).** After earnings: $121–128 if $117.80 holds | $113 | $145 / $155 | 1.7 / 2.5 (from $125) |
| **NBIS** | HOLD / MONITOR | $80–84 on a higher low above $75.60; use half size | $74.50 | $95 / $110 | 1.7 / 3.7 (from $82) |
| **CRDO** | HOLD / MONITOR | Wait for earnings (early Dec **[EST]**). After earnings: $98–104 | $91.50 | $118 / $128.60 | 1.8 / 2.9 (from $101) |
| **PL** | HOLD / MONITOR | Wait for Dec 10 earnings. Any entry needs a hold of $10.00–10.35 | $9.55 | $11.70 / $12.10 | 1.9 / 2.4 (from $10.30) |
| **CRWV** | AVOID / HIGH RISK | Re-evaluate on a close above $47 (first step) and above $51.90 (full) | — | — | — |
| **RDW** | AVOID / HIGH RISK | Re-evaluate on a close above $6.62 with RVOL above 1.5 | — | — | — |
| **VELO** | AVOID / HIGH RISK | No structure; a new 52-week low today | — | — | — |

R/R and percentage figures are **[EST]** calculations from the stated reference prices, not forecasts.

**Key events:**
- **Thu Nov 26:** US markets **closed** (Thanksgiving).
- **Fri Nov 27:** **1:00 PM ET early close** (bond market 2:00 PM ET). Liquidity will be thin.
  - No major US data releases are scheduled **[EST]**.
  - The **Fed pre-meeting blackout** for the Dec 8–9 FOMC starts **Sat Nov 28**, so few Fed speakers are expected **[EST]**.
- **Over the holiday (wildcard):** findings from the **trade investigation into 16 economies (incl. Taiwan and South Korea)** could post at any time, along with any tariff announcement. This matters most for SMH, MU, MRVL and CRDO.
  - **Nvidia governance:** Treasury's 10-day window for answers from Nvidia's board expired today with no public response.
  - Source: [TECHi](https://www.techi.com/chip-stocks-recover-early-slide-nasdaq-close-november-25/).
- **Next week:**
  - **MRVL earnings on Tue Dec 1, after the close [FACT].**
  - CRDO earnings in early December **[EST]**.
  - Jobs report on Fri Dec 4 **[EST]**.
  - **FOMC decision on Dec 9**, with a ~95% chance of a 25 bp hike priced in **[FACT per yesterday's sources]**.

---

*Data limitations:*
- Today's prices are Twelve Data snapshots and may differ slightly from official closing prints.
- After-hours data was unavailable from both feeds.
- Some news items come from secondary aggregators.
- Nothing here is personalised investment advice.
