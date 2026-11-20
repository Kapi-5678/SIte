## 🌙 Post-Market Briefing: Friday, November 20, 2026

**Data notes (please read first)**
- **Retrieved:** 2026-11-20, about 21:32–22:10 UTC (23:32–00:10 Bucharest; 16:32–17:10 ET). After-hours runs until 20:00 ET, so **the after-hours prices below are early prints only**.
- **Today's prices.** Massive (Polygon) refused same-day data on this plan (`/v1/open-close` → "NOT_AUTHORIZED … before end of day"). Today's open, high, low, close and volume therefore come from the **Twelve Data** quote endpoint. They were cross-checked against press reports where available:
  - CNBC (via StockTitan) has MU −13.86% and the Fool has MU at $594.51; Twelve Data matches.
  - CNBC has SPY $690.42 (−3.56%) vs Twelve Data $689.81 (−3.64%), and NVDA −13.65% vs Twelve Data −14.01%. These small gaps are probably closing-print timing. I used Twelve Data throughout.
- **History:** daily candles through Nov 19 come from Massive. % change is vs. the Nov 19 close; "5D" is vs. the Nov 13 close. Hourly bars are Twelve Data (regular session, ET).
- **Relative volume** = Twelve Data consolidated day volume ÷ the 20-day Massive average. For **QQQ, SMH, RKLB, VELO and SYM**, Twelve Data returned only a single-venue volume (3–9% of normal), so their RVOL is shown as **n/a**. I did not estimate it.
- **After-hours:** Twelve Data extended quotes, each with its ET timestamp. "No AH print" means the last trade was at 15:59 ET.
- **Indicators** are computed by me from the candles and include today's close: SMA 20/50/100/200, RSI(14, Wilder), MACD(12,26,9), ATR(14).
- **Morning brief:** the setups are checked against `reports/2026-11-20-market-intelligence.md` on branch `claude/pensive-clarke-xs555c`; it is not on this branch. Its three extra candidates are **CRDO, KTOS and SYM**.
- **Filings:** I checked the SEC EDGAR submissions API at about 21:50 UTC for every watchlist company and the three candidates. The window covered filings dated Nov 19–20.
- **Labels:** **[Confirmed]** = SEC filing or exchange/company data. **[Reported]** = media. **[Est.]** = unconfirmed. **Opinion** = my analysis. This is not personalised financial advice.

---

### 🧭 The day in three lines
1. **An AI-trade crash day: the indexes entered correction and chips had their worst week since 9/11 [Reported].**
   - **SPY $689.81 (−3.64%) on 2.59× volume**, its **7th straight loss**. It is now 5.9% below its 200-day ($732.76), with RSI 24.9.
   - **QQQ −5.47%**, **SMH −10.55% to $400.28**, **NVDA −14.0% to $125.53**, a new 52-week low with RSI 15.0.
   - Index closes **[Reported]**: S&P 500 6,910.39 (−3.70%), Nasdaq 22,617.73 (−5.28%, erasing its 2026 gains), Dow 48,147.33 (−1.93%), Russell 2000 −2.76%. **VIX 35.89 (+26%)**. The 10-year yield fell about 14bp to ~4.91%, while gold (−4.4%) and bitcoin (−4.5%) also fell. Sources: [Yahoo live blog](https://finance.yahoo.com/markets/live/stock-market-today-friday-november-19-dow-sp-500-nasdaq-anthropic-nvidia-141644188.html), [StockTitan/CNBC](https://www.stocktitan.net/articles/stock-market-today-live-november-20-2026).
2. **Every watchlist name fell between 6% and 16%, and almost all closed in the bottom 15% of the day's range.**
   - The worst were **NBIS −16.1%**, **OUST −15.5%**, **CRDO −15.2%**, **MU −13.9%**, **RDW −13.2%**, **BKSY −12.9%**, **VELO −12.4%**, **CRWV −12.0%**, **MRVL −11.7%** and **RKLB −10.8%**.
   - New 52-week lows: ASTS, VELO, CRWV, KTOS, SYM and NVDA.
3. **No setup triggered. Three were invalidated: MU, OUST and SYM (pre-earnings). Five bearish triggers fired: RDW, CRWV, QQQ, SMH and MRVL's support.**
   - **RKLB** traded inside its buy zone, and its key $43.89 low held. **BKSY** tested its $16.1 double bottom intraday and closed 27¢ above it.
   - **Opinion:** the tape shows capitulation-style readings (VIX near 36, SPY RSI below 25, NVDA RSI 15, 2–2.6× volume in the leaders). A reflex bounce is likely within days, but **no reversal has printed yet**. Early after-hours prices are only +0.5% to +3%.

---

### 1. Session recap

| Ticker | Close | % chg | 5D | Open | High | Low | Rel. vol | After-hours (ET) | AH vs close |
|---|---|---|---|---|---|---|---|---|---|
| **SPY** | 689.81 | −3.64% | −8.6% | 713.56 | 718.29 | 686.75 | **2.59×** | 693.29 @ 16:31 | +0.5% |
| **QQQ** | 609.75 | **−5.47%** | −10.3% | 638.55 | 643.23 | 606.27 | n/a | 613.21 @ 16:31 | +0.6% |
| **SMH** | 400.28 | **−10.55%** | −17.8% | 437.98 | 438.42 | 396.89 | n/a | 405.29 @ 16:24 | +1.3% |
| RKLB | 45.47 | −10.83% | −26.1% | 49.70 | 50.67 | 45.12 | n/a | 46.80 @ 16:25 | +2.9% |
| BKSY | 16.37 | −12.88% | −31.2% | 18.29 | 18.50 | 16.10 | 1.30× | no AH print | n/a |
| RDW | 5.65 | −13.21% | −26.9% | 6.32 | 6.43 | 5.59 | 1.48× | 5.71 @ 16:02 | +1.1% |
| ASTS | 23.27 | −8.92% | −28.6% | 24.96 | 25.95 | **22.72** | 1.33× | 23.76 @ 16:25 | +2.1% |
| MRVL | 122.28 | −11.69% | −22.0% | 132.74 | 134.18 | 120.56 | 1.26× | 124.74 @ 16:34 | +2.0% |
| MU | 594.51 | **−13.89%** | −23.6% | 665.62 | 668.99 | 585.25 | **1.83×** | 603.38 @ 16:35 | +1.5% |
| VELO | 2.97 | −12.39% | −28.4% | 3.25 | 3.33 | **2.85** | n/a | 3.04 @ 16:07 | +2.4% |
| NBIS | 81.31 | **−16.11%** | −29.8% | 93.69 | 93.97 | 80.67 | **1.67×** | 83.10 @ 16:32 | +2.2% |
| CRWV | 39.51 | −12.02% | −25.6% | 43.21 | 43.21 | **39.28** | 1.10× | 39.98 @ 16:30 | +1.2% |
| OUST | 23.80 | **−15.48%** | −28.9% | 27.10 | 27.48 | 23.60 | **1.50×** | no AH print | n/a |
| CRDO | 99.86 | **−15.20%** | −24.1% | 114.01 | 114.01 | 97.92 | **1.58×** | 99.00 @ 16:00 | −0.9% |
| KTOS | 26.89 | −9.31% | −20.7% | 28.92 | 29.41 | **26.60** | 1.35× | no AH print | n/a |
| SYM | 31.15 | −6.06% | −10.6% | 32.10 | 32.62 | **30.35** | n/a | no AH print | n/a |
| *NVDA (context)* | 125.53 | −14.01% | −22.9% | 143.57 | 143.73 | **124.50** | **2.34×** | 128.00 @ 16:34 | +2.0% |

**Bold low** = new 52-week low.

- **Shape of the day (fact, from hourly bars):** this was a gap-down and grind-lower session. It was not a flush and recovery.
  - Every name opened below Thursday's close and made lower hourly closes almost all day. SPY went $710.5 → $705.6 → $700.9 → $700.0 → $694.8 → $692.7 → $690.6.
  - SMH's sharpest leg came in the 13:30 and 15:30 bars.
  - Only **ASTS (+1.8% in the last hour) and SYM (+2.1% in the last hour)** bounced into the close. Opinion: no buyers stepped in at the bell elsewhere.
- **Volume:** the heaviest was in SPY (2.59×), NVDA (2.34×), MU (1.83×), NBIS (1.67×), CRDO (1.58×) and OUST (1.50×). Opinion: this looks like real liquidation, not a thin-tape drift.
- **Market drivers [Reported]:**
  - **Memory:** TrendForce flagged weaker NAND demand, with Chinese cloud providers cutting enterprise-SSD orders and NAND spot prices down about 20%. Sandisk fell about 16% ([Motley Fool](https://www.fool.com/investing/2026/11/20/why-micron-stock-crashed-today/)).
  - **AI-returns doubts and the Anthropic IPO:** ANT fell about 8–10% on day 2, back near its $83 IPO price.
  - **Fed:** **Governor Lisa Cook** said waiting longer to raise rates "risks getting behind the curve" and that she had preferred a hike in October. CME FedWatch shows about **92–97.5%** odds of a +25bp hike in December.
  - **Asia:** SoftBank fell about 16% in Tokyo and EWT (Taiwan) fell 10.9%.
  - **Data:** UMich final November sentiment was 51.5 (vs 51.6 expected, 48.0 prior).
  - Strategists were split: BNP Paribas called it "panic selling", while Deutsche Bank called the market "very oversold".
  - Sources: [Yahoo live blog](https://finance.yahoo.com/markets/live/stock-market-today-friday-november-19-dow-sp-500-nasdaq-anthropic-nvidia-141644188.html), [StockTitan](https://www.stocktitan.net/articles/stock-market-today-live-november-20-2026), [Yahoo: "Chips are crashing like it's 2008"](https://finance.yahoo.com/markets/article/chips-are-crashing-like-its-2008-as-the-nasdaq-100-nears-a-bear-market-192805534.html).

---

### 2. Morning setups: what happened

| Ticker | Morning plan | Result | Detail |
|---|---|---|---|
| **MU** (top pick) | POTENTIAL BUY. Zone $655–675. Confirmation: a 4H reversal with RVOL above 1.2, **or** a close above $712. Stop $615. Invalidation: close below $650 | ❌ **INVALIDATED** | It opened **in the zone ($665.62)**, but no reversal formed. The first hourly close was $626.17, already below the $650 shelf. **Close $594.51 < $650.** The $615 stop level was also breached (low $585.25). No confirmation occurred, so under the plan **no position was opened**. |
| **OUST** | POTENTIAL BUY. Zone $27.4–28.6. Confirmation: support holds on a close, then a reclaim of $29.3. Stop $25.90 | ❌ **INVALIDATED** | It gapped **below** the zone (open $27.10) and closed **$23.80**, well under the $27.35 triple support, on 1.50× volume. The stop level was breached. No entry was possible on the plan's terms. |
| **BKSY** | POTENTIAL BUY. Zone $16.6–17.4. Confirmation: double bottom holds on a 4H close, then reclaims $18.6. Stop $15.40 | ⏸ **NOT TRIGGERED: traded through the zone, no confirmation** | Low **$16.10**, an exact retest of the 10/23 low of $16.13. Close $16.37 (below the zone, above $16.1). Every hourly close was below $17.6, so $18.6 was never reclaimed. **Stop not hit.** |
| **RKLB** | POTENTIAL BUY. Zone $44.0–46.5, only if the 11/05 low ($43.89) holds. Confirmation: close above $49.25. Stop $41.40 | ⏸ **NOT TRIGGERED: in the zone, no confirmation** | Low $45.12, close $45.47 (in the zone). **$43.89 is intact.** The close was well below $49.25. Stop not hit. |
| **MRVL** | HOLD / MONITOR. No trade before earnings. Support $132.5 | ⚠️ **Support broken** | Close $122.28. **$132.5 is now resistance.** |
| **CRDO** | POTENTIAL BUY, **post-earnings only** (Dec 1). Zone $108–114. Invalidation $99 | ⚠️ **Not active. The invalidation level was breached intraday** | Low $97.92, close $99.86. The pre-earnings structure is broken; the zone needs rebuilding after the print. |
| **KTOS** | HOLD / MONITOR. Buy only on a close above $31.6 | ⏸ **NOT TRIGGERED** | New 52-week low $26.60, close $26.89. |
| **SYM** | HOLD / MONITOR into Mon earnings. Post-earnings zone $34–35.5, stop $31.5 | ❌ **INVALIDATED pre-earnings** | Close $31.15, **below the $31.5 stop** and a new 52-week low ($30.35). The setup must be rebuilt (see §5). |
| **CRWV** | AVOID. Bearish trigger: close below $40.58 | 🔻 **Bearish trigger FIRED** | Close $39.51, a new 52-week low ($39.28). |
| **RDW** | AVOID. A break below $6.06 opens $4.9–5.5 | 🔻 **Bearish trigger FIRED** | Close $5.65. |
| **NBIS / ASTS / VELO** | AVOID | ✔️ Avoid call was right | −16.1% / −8.9% / −12.4%. ASTS and VELO made new 52-week lows. |
| **SMH / QQQ** | Bearish: close below $445.6 / $644 | 🔻 **Both FIRED** | $400.28 / $609.75. |

**Scorecard:** 0 triggered, 3 invalidated (MU, OUST, SYM), 2 untriggered and still alive (RKLB, BKSY), 5 bearish triggers fired. No stops were hit on live positions, because none were opened, and no targets were hit. The morning's **"WAIT / reduce exposure"** stance was the correct call.

---

### 3. Earnings, filings and news (Nov 19 after-hours through Nov 20 after-hours)

**SEC filings [Confirmed, EDGAR]:**
- **CRWV: two Form 144s, accepted 16:36 ET today.** These are notices of proposed sales dated 11/20:
  - **CEO Michael Intrator:** 13,753 shares (~$581.5K; implied ~$42.28/share), [filing](https://www.sec.gov/Archives/edgar/data/1769628/000195004726011401/).
  - **Officer Kristen McVeety:** 4,173 shares (~$176.4K), [filing](https://www.sec.gov/Archives/edgar/data/1769628/000195004726011397/).
  - Both are acquired as "Restricted Stock" and are small relative to 465.8M shares outstanding. *Opinion:* these look like RSU sell-to-cover sales rather than discretionary selling. That remains unconfirmed until the Form 4s are filed.
- **ASTS:** a Form 4 was accepted 11/19 at 00:54 UTC, which is the Nov 18 evening ET and was already in the prior window. **KTOS:** the same applies, a Form 4 accepted 11/19 at 00:46 UTC.
- **None found** for RKLB, BKSY, RDW, MRVL, MU, VELO, NBIS, OUST, CRDO or SYM: no 8-K, S-3/ATM, 424B or Form 4 dated Nov 19–20.

**News (Massive `/v2/reference/news` plus web search):**
- **MU:** no company-specific news. The decline was attributed to TrendForce's NAND outlook: China cloud enterprise-SSD order cuts, NAND spot prices −20%, and a forecast of falling prices into 2027. About 26% of Micron's revenue is NAND [Reported] ([Motley Fool](https://www.fool.com/investing/2026/11/20/why-micron-stock-crashed-today/)). The confirmed catalysts are unchanged: buybacks step up from ~Dec 9 and earnings are on **Dec 17**.
- **ASTS:** Firefly Aerospace fell after JPMorgan cut its target to $32 (still Overweight). The Fool details the AST–Firefly deal: $1.3B for 36 engines, of which **≥$400M is payable in AST stock** and $500M has an unclear payment form [Reported] ([Motley Fool](https://www.fool.com/investing/2026/11/20/why-firefly-aerospace-stock-dropped-on-friday/)). *Opinion:* this reinforces the dilution overhang.
- **RKLB, RDW, MRVL, CRDO, NBIS, CRWV:** only opinion and comparison pieces from Motley Fool and Zacks. **No material news.**
- **BKSY, VELO, OUST, KTOS, SYM:** **No material news.**
- **Earnings today:** none on the watchlist. **SYM reports Mon Nov 23 after the close** [Confirmed earlier, [Finviz](https://finviz.com/news/411991/symbotic-announces-date-for-reporting-fourth-quarter-and-fiscal-year-2026-financial-results)].

---

### 4. Technical update (daily close vs. SMAs, RSI, MACD)

| Ticker | Close | 20-SMA | 50-SMA | 100-SMA | 200-SMA | RSI | MACD hist (prev) | ATR | Status change |
|---|---|---|---|---|---|---|---|---|---|
| SPY | 689.81 | 747.81 | 760.18 | 759.40 | 732.76 | **24.9** | −5.38 (−3.25) | 13.6 | **Breakdown on 2.6× volume**: −5.9% vs the 200-day; correction confirmed |
| QQQ | 609.75 | 678.60 | 710.98 | 710.69 | 683.07 | 26.8 | −4.68 (−2.22) | 18.8 | Lost the $644–647 Nov low; at Jan '26 low $607 |
| SMH | 400.28 | 494.50 | 547.51 | 558.31 | 525.17 | 26.2 | −5.72 (−2.81) | 26.1 | **Lost $445.6** (−10.6% day); next pivot $374 (Feb–Mar '26) |
| RKLB | 45.47 | 55.89 | 61.34 | 66.83 | 77.72 | 35.7 | −0.67 (−0.07) | 4.97 | Below all; $43.89 held; MACD widening lower |
| BKSY | 16.37 | 20.21 | 20.46 | 22.65 | 26.96 | 36.0 | **−0.33 (+0.01) flipped negative** | 1.82 | At the $16.1–16.3 double/triple bottom |
| RDW | 5.65 | 7.70 | 9.14 | 9.92 | 10.77 | 30.2 | −0.12 (−0.06) | 0.70 | **Broke $6.06**; next $4.87 (52-week low) |
| ASTS | 23.27 | 34.21 | 46.10 | 55.57 | 71.63 | 27.6 | −0.51 (−0.40) | 3.77 | New 52-week low; no structure below |
| MRVL | 122.28 | 171.05 | 220.27 | 218.56 | 188.60 | 27.9 | −1.57 (−0.87) | 16.1 | **Broke $132.5** on 1.26×; next pivots $100 (Apr low) / $85–87 |
| MU | 594.51 | 786.65 | 912.26 | 920.44 | 772.54 | 29.5 | −9.67 (−4.05) | 61.8 | **Broke the $650 shelf** on 1.83×; −23% vs 200-day; May '26 base ~$510 |
| VELO | 2.97 | 5.20 | 7.64 | 9.98 | 12.61 | 25.6 | −0.11 (−0.11) | 0.65 | New 52-week low $2.85 |
| NBIS | 81.31 | 134.48 | 181.30 | 196.49 | 179.75 | 28.5 | −3.05 (−2.17) | 16.9 | Closed at the low; pivots $78.2 / $75.3 / $73.5 (52-week low) |
| CRWV | 39.51 | 51.85 | 67.99 | 76.76 | 88.00 | 32.6 | **0.00 (+0.50) bear cross** | 6.26 | **New 52-week low; MACD crossed down** |
| OUST | 23.80 | 32.11 | 34.85 | 37.31 | 33.09 | 33.0 | −0.78 (−0.39) | 3.13 | **Broke $27.35 triple support** on 1.5×; sitting on $23.5–23.6 (Jan/May '26 lows) |
| CRDO | 99.86 | 136.47 | 167.40 | 195.25 | 181.03 | 31.6 | −1.22 (−0.16) | 14.9 | Broke the $110.8 Nov low; next $92.6–94.2 |
| KTOS | 26.89 | 36.13 | 40.37 | 46.27 | 58.46 | **24.0** | −0.75 (−0.60) | 2.31 | New 52-week low; no base |
| SYM | 31.15 | 36.18 | 39.66 | 40.78 | 46.31 | 29.0 | −0.39 (−0.28) | 2.11 | New 52-week low $30.35 into earnings |
| NVDA | 125.53 | 181.46 | 207.00 | 209.79 | 203.35 | **15.0** | −4.63 (−3.71) | 10.7 | Extreme oversold; −48% from its 52-week high |

- **Every ticker is below all four SMAs.** Every MACD histogram is negative or crossing negative. No bullish divergences are visible on the daily charts. Opinion: the only constructive facts are RKLB holding $43.89 and BKSY holding $16.1, both by a margin of less than 1 ATR.
- **Breakdowns on volume:** MU (shelf), OUST (triple support), MRVL ($132.5), CRDO ($110.8), RDW ($6.06), CRWV ($40.58), SMH ($445.6), QQQ ($644).
- **No breakouts.**

---

### 5. Plan for the next session (Mon Nov 23)

**Stance: STAY DEFENSIVE. No new full-size longs.** *Opinion:*
- Positioning is stretched enough for a sharp short-covering bounce (VIX 35.9, SPY RSI 24.9, NVDA RSI 15).
- Buy only **after** a reversal day prints: an index close above the prior day's high on expanding volume.
- Even then, use half size until SPY reclaims **$715.9** (Thursday's close).
- Key SPY levels: support **$676–680** (Jan–Feb '26 lows); resistance $705, then $715.9 and $732.8 (200-day).
- SMH: support $374, resistance $437–447.

| Ticker | Signal | Entry zone / trigger | Stop | Targets | Notes |
|---|---|---|---|---|---|
| **RKLB** | **POTENTIAL BUY (conditional)**, unchanged | $44.0–46.5. Confirmation: **close above $49.25** on RVOL above 1.0 | $41.40 | T1 $56.0, T2 $61.5 | Still the only intact morning setup. A close below $43.89 voids it. AH $46.80 |
| **BKSY** | **HOLD / MONITOR** (downgraded) | Only on a reclaim of **$17.4**, then $18.6, while $16.1 holds | $15.40 | T1 $20.2 (20-day), T2 $23.8 | The MACD flip and −31% over 5 days argue for waiting. **A close below $16.1 = breakdown** toward $12.4 |
| **MU** | **HOLD / MONITOR** (downgraded) | No zone. Reassess on a **close above $626** (Friday's first-hour close) with RVOL above 1.2 | n/a | n/a | No chart support until about $510 (May base). The fundamental anchors are unchanged: buybacks ~Dec 9, earnings Dec 17. *Opinion:* the risk is that NAND weakness spreads to DRAM pricing |
| **OUST** | **AVOID** (downgraded) | Reassess only on a reclaim of $27.35 | n/a | n/a | Watch $23.5: a close below it opens $21.0 |
| **MRVL** | **AVOID until earnings** (~Dec 1, *unverified*) | After the print: hold $120.5 and reclaim $132.5 | n/a | n/a | $132.5 is now resistance |
| **CRDO** | **HOLD / MONITOR**, post-earnings only (Dec 1, *secondary-sourced*) | Rebuild after the print: a hold of $92.6–94.2 and a reclaim of $110.8 | n/a | n/a | The old $108–114 zone is void |
| **SYM** | **HOLD / MONITOR**: earnings **Mon AMC** | Post-print gap that **holds above $33.2** (Thursday's close); zone $33.2–34.5 | $30.20 | T1 $36.2 (20-day), T2 $39.7 (50-day) | A close below $30.35 after the print → avoid |
| **KTOS** | **HOLD / MONITOR** | Close above $29.4 (Friday's high), then $31.6 | n/a | n/a | No base yet |
| **NBIS** | **AVOID / HIGH RISK** | — | — | — | Pivots $78.2, $75.3, $73.5 |
| **CRWV** | **AVOID / HIGH RISK** | — | — | — | New lows; insider 144s (likely sell-to-cover) |
| **ASTS** | **AVOID / HIGH RISK** | — | — | — | No floor; the stock-paid Firefly deal adds dilution |
| **RDW** | **AVOID / HIGH RISK** | — | — | — | Target zone $4.9–5.5 now in play |
| **VELO** | **AVOID / HIGH RISK** | — | — | — | New lows; cash burn |

**Key events ahead**
- **Mon Nov 23:** **SYM FQ4 earnings after the close (webcast 5 PM ET) [Confirmed].** I found no confirmed 2026 macro releases or Fed-speaker schedule for Monday; verify on the [Fed calendar](https://www.federalreserve.gov/newsevents/calendar.htm).
- **Wed Nov 25:** Q3 GDP (2nd estimate) and October PCE [scheduled per the morning brief; *unverified*]. This is a key input for the December hike odds.
- **Thu Nov 26:** US markets **closed** (Thanksgiving). **Fri Nov 27:** early 1 PM ET close [*Est.*, standard NYSE holiday schedule].
- **Dec 1:** MRVL and CRDO earnings (*press-reported*). **Dec 2:** House briefing deadline on Nvidia. **Dec 8–9:** FOMC, with a hike about 92–97% priced. **~Dec 9:** MU buyback step-up. **Dec 17:** MU earnings [Confirmed].

**Alert levels for Monday**

| Ticker | Bullish (actionable) | Bearish (informational) |
|---|---|---|
| SPY / QQQ / SMH | Close above $705 / $630 / $420 (reversal-day confirmation) | Close below $676 / $593 / $374 |
| RKLB | Close above $49.25 | Close below $43.89 |
| BKSY | Reclaim of $17.4 → $18.6 | Close below $16.1 |
| MU | Close above $626 on RVOL above 1.2 | Close below $585 |
| OUST | Reclaim of $27.35 | Close below $23.5 |
| SYM | Post-earnings hold above $33.2 | Close below $30.35 |
| NVDA (sector tell) | Close above $135.8 | Close below $124.5 |

*Sources not linked inline: price, volume and indicator data are from api.massive.com (history) and api.twelvedata.com (today and after-hours); filings are from SEC EDGAR.*
