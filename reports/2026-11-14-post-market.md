## 🌙 Post-Market Briefing: Saturday, November 14, 2026 (weekend edition)

**Data notes (please read first)**
- **US markets were closed today (Saturday).** There was no session, so nothing could trigger, stop out or hit a target. This report instead (a) replaces Friday's *provisional* numbers with **official Nov 13 data**, (b) adds the **final after-hours prints** from Friday evening, and (c) covers what was published since Friday's close.
- **Retrieved:** 2026-11-14, 21:35–22:10 UTC (23:35–00:10 Bucharest).
- **Source:** Massive (Polygon) daily bars, 1-minute bars incl. extended hours, `/v1/open-close` and `/v2/reference/news`. Twelve Data was not needed. Massive marks the data "DELAYED" (end-of-day), which is fine for a closed market.
- **After-hours** = last 1-minute bar of Friday's extended session, which ends 20:00 ET (03:00 Bucharest Saturday). After-hours volume is thin, so treat those prints as indications, not levels.
- **Relative volume** = Friday's full-day volume ÷ the prior 20-day average.
- **Indicators** are computed by me from the daily candles: SMA 20/50/100/200, RSI(14, Wilder), MACD(12,26,9).
- **Morning brief:** setups are checked against `reports/2026-11-14-market-intelligence.md` on branch `claude/pensive-clarke-6a2ros` (not on this branch). Its three extra candidates are **KRMN, CRDO, FLY**.
- **Labels:** **[Confirmed]** = price data, SEC filing or company release. **[Reported]** = media. **[Est.]** = unconfirmed. **Opinion** = my analysis. Not personalised financial advice.

---

### 🧭 Three takeaways
1. **Friday's after-hours session finished weaker than the close, across the whole list.** Every ticker ended extended trading 1.4–3.0% below its 16:00 close (SPY −0.6%, QQQ −0.8%). **MU's last print, $761.20, is back below its 200-day average ($765.61)** and **OUST's, $32.62, is below its own ($32.87)**. I found no headline behind the drift.
2. **Friday's selling came on below-average volume**, apart from NBIS (1.80×). QQQ's close under its 200-day average happened on 0.83× volume. Opinion: that is weak-demand drift, not capitulation, so it neither confirms a breakdown nor shows buyers stepping in.
3. **Rocket Lab flew its 100th Electron on Saturday, successfully** [Confirmed, company release]. It is the only company-specific positive on the list this weekend. The week ahead is dominated by **NVIDIA results on Tuesday after the close**.

---

### 1. Session recap (official Friday Nov 13 data)

| Ticker | Close | % chg | Week | Open | High | Low (time ET) | Rel. vol | After-hours (Fri 19:59 ET unless noted) | AH vs close |
|---|---|---|---|---|---|---|---|---|---|
| **SPY** | 754.37 | −0.36% | +2.6% | 760.07 | 760.12 | 747.88 (10:21) | 0.80 | 749.60 | −0.63% |
| **QQQ** | 679.89 | −1.20% | +3.6% | 688.54 | 688.75 | 671.68 (11:22) | 0.83 | 674.25 | −0.83% |
| **SMH** | 486.75 | −2.99% | +4.9% | 499.93 | 500.27 | 473.26 (11:05) | 1.03 | 481.53 | −1.07% |
| RKLB | 61.53 | −3.96% | +15.9% | 63.70 | 64.46 | 59.76 (11:05) | 0.68 | 59.87 | −2.69% |
| BKSY | 23.80 | +2.41% | +11.6% | 23.25 | 24.26 | 22.33 (09:45) | 1.18 | 23.46 @ 19:15 | −1.43% |
| RDW | 7.73 | −3.74% | +7.2% | 7.86 | 8.05 | 7.45 (13:17) | 0.84 | 7.56 @ 19:58 | −2.20% |
| ASTS | 32.60 | −5.51% | +0.8% | 33.91 | 34.50 | 31.34 (10:03) | 0.85 | 31.70 | −2.76% |
| MRVL | 156.76 | −4.68% | +11.0% | 161.60 | 163.89 | 149.17 (10:26) | 0.79 | 152.59 | −2.66% |
| MU | 778.31 | −2.52% | +12.8% | 782.68 | 796.18 | 750.25 (11:16) | 0.91 | 761.20 | −2.20% |
| VELO | 4.15 | −5.90% | −25.6% | 4.41 | 4.44 | 4.01 (11:06) | 0.85 | 4.07 | −2.03% |
| NBIS | 115.88 | −9.92% | −10.5% | 123.55 | 123.97 | 109.00 (10:23) | **1.80** | 112.80 | −2.66% |
| CRWV | 53.13 | −6.13% | +14.5% | 56.05 | 56.36 | 49.24 (10:36) | 1.08 | 51.75 | −2.60% |
| OUST | 33.48 | −8.52% | −3.8% | 36.23 | 36.51 | 32.40 (10:14) | 0.92 | 32.62 | −2.57% |
| KRMN | 40.66 | +0.40% | −10.9% | 39.85 | 40.70 | 37.33 (10:48) | 1.25 | 39.00 @ 18:32 (≈1K shares, not meaningful) | −4.08% |
| CRDO | 131.51 | −5.94% | +9.1% | 138.95 | 141.00 | 126.26 (10:36) | 0.77 | 128.04 | −2.64% |
| FLY | 25.21 | −0.40% | +21.4% | 25.00 | 25.95 | 23.27 (10:37) | 0.84 | 24.45 | −3.01% |

All figures [Confirmed, Massive]. "Week" is vs. the Nov 6 close.

- **How the after-hours session went:** most of the drop came in the first hour after the close and prices then drifted lower without recovering. MU went $778.31 → $770.15 by 17:00 → $761.20 by 20:00. QQQ went $679.89 → $677.23 → $674.25. Volume after 17:00 was thin (MU about 244K shares in three hours).
- **Corrections to Friday's provisional report:**
  - Official closes differ from Friday's Twelve Data values by a few cents (MU $778.31, not $778.11; NBIS $115.88, not $115.84).
  - **CRWV volume was 80.2M shares (1.08×)**, not the 121.7M Twelve Data showed. There was no unusual volume.
  - After-hours ended lower than the early prints quoted on Friday (e.g. MU $761.20 vs. $763.63; NBIS $112.80 vs. $113.76; OUST $32.62 vs. $33.34).
  - VELO: $4.01 is the low since the August 2025 uplisting week. The only lower print in my history is $2.81 on its first listing day (2025-08-19).

---

### 2. This morning's setups: status

**No US session today, so every setup is NOT TRIGGERED by definition.** The table shows where Friday's last after-hours print sits against each plan. These plans were written this morning from Friday's close; Monday's open is the first real test.

| Ticker | Morning plan (Nov 14 brief) | Status | Where the last print sits |
|---|---|---|---|
| **OUST** | Buy $31.80–33.00; confirm a daily close holding the 200 DMA (~$32.9) and a 1h reclaim of $34.70; stop $30.10 | ⏸ **NOT TRIGGERED** (market closed) | AH $32.62: **inside the zone**, but below the 200 DMA. Confirmation not possible before Monday's close. |
| **KRMN** | Buy $38.00–40.00; confirm Monday holds above $37.33 and the 4h reclaims $41; stop $35.30 | ⏸ **NOT TRIGGERED** | Close $40.66, just above the zone. The $39.00 after-hours print was about 1,000 shares; ignore it. |
| **RKLB** | Buy $57.50–60.00, or a daily close above $68.30 on >1.3× volume; stop $53.40 | ⏸ **NOT TRIGGERED** | AH $59.87: at the **top edge of the zone**. Friday's low was $59.76. |
| **CRWV** | Buy $49.50–51.50; confirm $49.24 holds and the 4h reclaims $54.80; stop $44.80 | ⏸ **NOT TRIGGERED** | AH $51.75: 25 cents above the zone. |
| **MU** | Buy $735–760; confirm a daily close above $800, or a 4h higher low holding the 200 DMA after NVDA; stop $695 | ⏸ **NOT TRIGGERED** | AH $761.20: $1.20 above the zone and **$4.41 below the 200 DMA**. |
| **BKSY** | Retest $21.80–22.50, or a daily close above $24.95 with volume above 1.6M; stop $19.90 | ⏸ **NOT TRIGGERED** | AH $23.46, between the two triggers. |
| **FLY** | Retest $21.00–22.50; stop $19.20 | ⏸ **NOT TRIGGERED** | AH $24.45, about 9% above the zone. |
| **CRDO** | $112–122, or a daily close above $148.20; stop $108 | ⏸ **NOT TRIGGERED** | AH $128.04, about 5% above the zone. |
| **MRVL** | No trade; speculative $133–142 only with a daily reversal candle | ⏸ **NOT TRIGGERED** | AH $152.59. |
| **RDW** | No trade; reconsider on a daily close above $8.75 | ⏸ **NOT TRIGGERED** | AH $7.56. |
| **ASTS** | No trade; reconsider above $38.20 or on a double bottom at $27.5–29 | ⏸ **NOT TRIGGERED** | AH $31.70. |
| **NBIS** | No trade; valid only if $109 holds and price closes back above $123.50 | 🛑 **AVOID stands** | AH $112.80, below the Nov 5 low ($113.30) and $3.80 above Friday's $109.00 low. |
| **VELO** | No trade | 🛑 **AVOID stands** | AH $4.07. |

**No setup was invalidated and no stop or target was hit.** Opinion: if Monday opens near the after-hours prints, OUST, RKLB, CRWV and MU will all open in or right next to their entry zones at the same time. Being in the zone is not the signal. Each plan needs its confirmation, and none of them can be confirmed at the open.

---

### 3. Earnings, filings and material news (Friday after the close through Saturday)

Filings were checked on SEC EDGAR for all 13 names (plus NVDA) at about 21:50 UTC on Nov 14. **No 8-K, S-3, 424B (ATM/offering) or 10-Q was filed for any of the 13 tickers on Nov 13–14, and none reported earnings.**

**RKLB**
- **100th Electron launch, successful** [Confirmed, company release]. "The Mountain God Rises" lifted off Saturday Nov 14 at 12:30 am EST and deployed iQPS's YAMATSUMI-II satellite. It was the 11th iQPS mission. The company says the next 100 Electron launches are already booked ([GlobeNewswire](https://www.globenewswire.com/news-release/2026/11/14/3403041/0/en/rocket-lab-hits-100-electron-launches-fastest-commercial-rocket-to-reach-the-milestone.html)). No SEC filing.

**NBIS**
- **Form 4 [Confirmed], accepted Fri 16:48 ET:** Chief Revenue Officer Marc Boroditsky exercised 7,000 options at $40 and sold the 7,000 shares at an average of $147.97 on Nov 11, under a 10b5-1 plan adopted in June ([Form 4](https://www.sec.gov/Archives/edgar/data/1513845/000151384526000149/xslF345X06/form4.xml)). Small and pre-planned, though it was sold the day before the Q3 report.
- No other new item. Friday's analyst cuts and the Microsoft vendor report are in Friday's briefing.

**CRWV**
- **Form 4 [Confirmed], accepted Fri 16:41 ET:** director Glenn Hutchins had 1,440 RSUs vest on Nov 10. No sale ([Form 4](https://www.sec.gov/Archives/edgar/data/1769628/000176962826000466/xslF345X06/form4.xml)). Routine.
- **Loan talks [Reported]:** Friday's drop is attributed to AI-cloud selling and reported talks for a roughly $4B loan ([Motley Fool](https://www.fool.com/coverage/stock-market-today/2026/11/13/stock-market-today-nov-13-coreweave-falls-over-6-on-ai-cloud-selling-and-reported-usd4-billion-loan-talks/)). No company announcement.
- **Barclays [Reported, date unclear]:** target cut to $85 from $105, Equal Weight. The article is dated Nov 13 but seems to describe Thursday ([Defense World](https://www.defenseworld.net/2026/11/13/coreweave-nasdaqcrwv-stock-price-down-6-9-on-analyst-downgrade.html)).

**MRVL**
- **No material news.** **Earnings date is now confirmed: Tue Dec 1**, call at 1:30 pm PT [Confirmed, company IR] ([release](https://investor.marvell.com/news-events/press-releases/detail/1041/marvell-technology-inc-announces-conference-call-to-review-third-quarter-of-fiscal-year-2027-financial-results)). This settles the Dec 1 vs. Nov 26 conflict in this morning's brief.

**CRDO**
- **No material news.** Earnings **Tue Dec 1 after the close**, the same afternoon as MRVL [Reported, company release via StockTitan] ([link](https://www.stocktitan.net/news/CRDO/credo-schedules-second-quarter-fiscal-year-2027-financial-results-vchn8hvl39pc.html)).

**MU**
- **No material news** and no filing after Nov 12. The next earnings date is **not announced**; one calendar lists Dec 23, unconfirmed [Est.] ([Wall Street Horizon](https://www.wallstreethorizon.com/micron-earnings-calendar)). This morning's brief used ~Dec 16 [Est.]; treat both as guesses.
- [Reported] Micron is named among the buyers in a private placement alongside the Anthropic IPO ([Motley Fool](https://www.fool.com/investing/2026/11/14/nvidia-alphabet-microsoft-and-micron-are-buying-anthropic-ipo/)). I have not read the prospectus.

**BKSY, RDW, ASTS, VELO, OUST, KRMN, FLY:** **No material news** and no SEC filing on Nov 13–14.

**Market-wide**
- **NVIDIA CEO change is confirmed** [Confirmed, 8-K filed Nov 12]. The board accepted Jensen Huang's resignation as President, CEO and director on Nov 11. CFO Colette Kress is interim CEO and remains CFO ([8-K](https://www.sec.gov/Archives/edgar/data/1045810/000104581026000082/nvda-20261111.htm)). This morning's brief had this as unverified.
- [Reported] The board says it is still selecting a search firm; the FT reported an approach to Arm's CEO ([CNBC](https://www.cnbc.com/2026/11/13/nvidia-huang-ceo-replacement-search.html)).
- **Anthropic IPO [Reported]:** range $70–78 on 825M shares, up to about $64.4B; pricing expected Wed Nov 18 evening, first trade Thu Nov 19 as "ANT" ([CNBC](https://www.cnbc.com/2026/11/13/stock-market-next-week-outlook-for-nov-16-20-2026.html)).
- I found no Saturday headline that explains Friday's after-hours drift.

---

### 4. Technical update (daily, official Nov 13 close)

| Ticker | Close | 20 DMA | 50 DMA | 100 DMA | 200 DMA | RSI(14) | MACD line / signal | MACD histogram (prev) |
|---|---|---|---|---|---|---|---|---|
| SPY | 754.37 | 759.02 ↓ | 764.43 ↓ | 760.28 ↓ | 731.92 ↑ | 47.1 | −4.12 / −4.09 | −0.03 (−0.29) |
| QQQ | 679.89 | 695.45 ↓ | 717.87 ↓ | 714.45 ↓ | 682.24 ↓ | 42.8 | −12.92 / −12.83 | −0.09 (−0.54) |
| SMH | 486.75 | 518.14 ↓ | 559.80 ↓ | 567.58 ↓ | 523.89 ↓ | 40.1 | −22.74 / −21.90 | −0.84 (−1.29) |
| RKLB | 61.53 | 55.78 ↑ | 62.47 ↓ | 68.86 ↓ | 78.28 ↓ | 52.9 | −0.22 / −1.90 | +1.68 (+1.81) |
| BKSY | 23.80 | 19.45 ↑ | 20.56 ↑ | 22.98 ↑ | 27.01 ↓ | 63.6 | 0.90 / 0.08 | +0.82 (+0.86) |
| RDW | 7.73 | 8.15 ↓ | 9.56 ↓ | 10.16 ↓ | 10.87 ↓ | 43.0 | −0.48 / −0.56 | +0.08 (+0.09) |
| ASTS | 32.60 | 37.81 ↓ | 49.70 ↓ | 58.25 ↓ | 73.62 ↓ | 36.8 | −4.58 / −4.87 | +0.30 (+0.35) |
| MRVL | 156.76 | 194.75 ↓ | 229.21 ↓ | 225.51 ↓ | 187.00 ↓ | 35.2 | −24.27 / −21.88 | −2.39 (−3.38) |
| MU | 778.31 | 838.00 ↓ | 943.78 ↓ | 943.00 ↓ | 765.61 ↑ | 42.5 | −55.03 / −53.62 | −1.41 (−4.27) |
| VELO | 4.15 | 6.04 ↓ | 8.41 ↓ | 10.67 ↓ | 12.86 ↓ | 29.2 | −1.06 / −1.01 | −0.04 (−0.00) |
| NBIS | 115.88 | 151.12 ↓ | 194.60 ↓ | 204.14 ↓ | 179.35 ↓ | 35.8 | −19.05 / −18.37 | −0.68 (+0.19) |
| CRWV | 53.13 | 54.99 ↓ | 72.60 ↓ | 79.20 ↓ | 88.99 ↓ | 43.1 | −5.70 / −7.00 | +1.30 (+1.26) |
| OUST | 33.48 | 32.28 ↑ | 35.61 ↓ | 38.48 ↓ | 32.87 ↑ | 48.3 | 0.22 / −0.56 | +0.78 (+1.10) |
| KRMN | 40.66 | 38.80 ↑ | 36.01 ↑ | 43.41 ↓ | 60.36 ↓ | 53.5 | 1.75 / 1.33 | +0.42 (+0.65) |
| CRDO | 131.51 | 149.05 ↓ | 172.28 ↓ | 202.22 ↓ | 180.86 ↓ | 40.5 | −14.42 / −14.52 | +0.09 (−0.16) |
| FLY | 25.21 | 19.68 ↑ | 20.71 ↑ | 22.05 ↑ | 26.79 ↓ | 62.8 | 1.23 / 0.18 | +1.05 (+1.09) |

↑ = close above the average, ↓ = close below.

**Volume now confirmed: what it changes**
- **No breakdown on Friday was confirmed by volume, except NBIS.** QQQ closed below its 200 DMA on 0.83× volume; RKLB lost its 50 DMA on 0.68×; CRWV lost its 20 DMA on 1.08×; OUST fell 8.5% on 0.92×. These are real closes below the averages, but on ordinary or light volume.
- **NBIS is the exception: −9.9% on 1.80×**, after −16.8% on 2.67× on Thursday. Two heavy-volume down days in a row is distribution. MACD crossed back below its signal line.
- **No breakout on volume either.** BKSY (+2.4%, 1.18×) and KRMN (+0.4%, 1.25×) were the only green names and neither broke out (BKSY stayed under $24.92).

**Levels that changed since this morning's brief** (after-hours only; Opinion)
- **MU:** after-hours low $761.00, below the 200 DMA ($765.61). If Monday opens there, the 200 DMA turns from support into the first resistance. Support is unchanged: $750.25 (Friday's low), then $725–733, then $699.6.
- **QQQ:** after-hours $674.25 is right at the ~$675 level this morning's brief flagged for the weekly close. Friday's official close ($679.89) was above it. Support $671.68 (Friday's low), then $667.05 (Nov 10 low), then $647.05 (Nov 5 low).
- **OUST:** after-hours $32.62 is between the 20 DMA ($32.28) and the 200 DMA ($32.87). A daily close below $32.28 would break the confluence zone the setup depends on.
- **NBIS:** after-hours $112.80 is below the Nov 5 low ($113.30). $109.00 is the only support left before the round $100 level.
- **RKLB:** after-hours $59.87 is just above Friday's $59.76 low. Below that, the 20 DMA is $55.78.
- **ASTS:** after-hours $31.70 is near Friday's $31.34 low. The 52-week low is $27.58.
- All other levels from this morning's brief stand.

---

### 5. Plan for Monday, Nov 16

Levels and signals are opinion. Entry zones, stops and targets are carried over from this morning's brief; only notes and emphasis changed.

| Ticker | Signal | Entry zone / trigger | Stop | Targets | Note for Monday |
|---|---|---|---|---|---|
| **OUST** | 🟡 **POTENTIAL BUY, needs confirmation** | $31.80–33.00; confirm a daily close at or above ~$32.9 and a 1h reclaim of $34.70 | $30.10 | $38.20 / $40.40 | Likely opens inside the zone. Do not buy the open; a close below $32.28 cancels the idea. |
| **KRMN** | 🟡 **POTENTIAL BUY, needs Monday hold** | $38.00–40.00; confirm a hold above $37.33 and a 4h reclaim of $41 | $35.30 | $45.90 / $54.30 | Held up best on Friday (closed at the high on 1.25×). |
| **RKLB** | 🟡 **POTENTIAL BUY (pullback)** | $57.50–60.00 with a 4h higher low and a 1h reclaim of $62; or a daily close above $68.30 on >1.3× volume | $53.40 | $68.00 / $77.50 | 100th Electron success is supportive but small. Watch whether $59.76 holds. |
| **MU** | ⏳ **WAIT for NVDA** | $735–760; confirm a daily close above $800, or a 4h higher low that holds the 200 DMA after NVDA reports | $695 | $828 / $890 | After-hours is under the 200 DMA. NVDA on Tuesday night is binary; no new size before it. |
| **CRWV** | ⏳ **WAIT, speculative** | $49.50–51.50; confirm $49.24 holds and the 4h reclaims $54.80 | $44.80 | $62.00 / $72.50 | Half size at most. Loan talks and the Microsoft vendor review are open risks. |
| **BKSY** | ⏳ **WAIT FOR RETEST** | $21.80–22.50, or a daily close above $24.95 with volume above 1.6M | $19.90 | $27.00 / $30.50 | Strongest chart on the list. |
| **FLY** | ⏳ **WAIT FOR RETEST** | $21.00–22.50 | $19.20 | $27.00 / $31.10 | Extended; no chase. |
| **CRDO** | 👀 **HOLD / MONITOR** | $112–122, or a daily close above $148.20 | $108 | $149 / $172 | Moves with SMH and NVDA. |
| **MRVL** | 👀 **HOLD / MONITOR** | Speculative $133–142 only with a daily reversal candle on rising volume | $127 | $165 / $187 | Support $149.17, then $147.8. |
| **RDW** | ⛔ **AVOID / HIGH RISK** | Reconsider only on a daily close above $8.75 | n/a | $9.45 / $10.15 | Below every average. |
| **ASTS** | ⛔ **AVOID / HIGH RISK** | Daily close above $38.20, or a double bottom at $27.5–29 | n/a | n/a | Drifting toward the 52-week low. |
| **NBIS** | ⛔ **AVOID / HIGH RISK** | No entry. Repair needs $109 to hold and a close back above $123.50 | n/a | Resistance $118.8 / $123.5 / $132 | A daily close below $109 opens a new leg down. |
| **VELO** | ⛔ **AVOID / HIGH RISK** | None | n/a | n/a | New lows, RSI 29, no base. |

**Key events**

All times ET (Bucharest = ET + 7h). Calendar items are [Reported] unless marked.
- **Mon Nov 16:** Empire State Manufacturing, 8:30 am (prior 25.5). Fed speakers per a single source (Finviz): Barr 5:00 am, Williams 9:05 am, **Chair Warsh 12:00 pm**, Barkin 6:10 pm. No watchlist or AI/space/semis earnings.
- **Tue Nov 17:** October retail sales, 8:30 am (consensus 0.0% m/m, ex-autos +0.4%); industrial production, 9:15 am. Fed speakers (same single source): Musalem, Waller, Hammack, Williams. Home Depot before the open. **NVIDIA Q3 FY27 after the close**: consensus revenue about $109B against a $108B guide [Est.]; first report under the interim CEO.
- **Wed Nov 18:** FOMC minutes, 2:00 pm. Anthropic IPO pricing in the evening.
- **Thu Nov 19:** Anthropic first trade on Nasdaq ("ANT").
- **Further out:** MRVL and CRDO earnings, both Dec 1 after the close. FOMC Dec 8–9. MU earnings date not announced.

**Stance (opinion):** unchanged from this morning: wait and be selective, no new size in AI semis or neoclouds before NVIDIA. Friday's after-hours drift means several names may open inside their entry zones on Monday. Treat that as the start of the test, not as the entry. The setups with the cleanest risk definition are still OUST and KRMN; the one that most needs patience is MU.

---

*Prices: Massive (Polygon), official Nov 13 daily bars and Friday extended-hours minute bars. Facts are labeled; levels, signals and the stance are opinion, not personalised investment advice.*
