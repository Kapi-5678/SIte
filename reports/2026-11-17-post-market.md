## 🌙 Post-Market Briefing: Tuesday, November 17, 2026

**Data notes (please read first)**
- **Retrieved:** 2026-11-17, 21:32–21:55 UTC (23:32–23:55 Bucharest; 16:32–16:55 ET).
- **Today's prices.** Massive (Polygon) still refuses same-day data on this plan: `/v1/open-close`, minute bars and the snapshot endpoint for today all returned "not authorized". Today's open/high/low/close and volume therefore come from the **Stock Analysis** daily history pages, read about 16:45 ET. Every close was cross-checked against the **Twelve Data** quote; the largest gap is 21 cents (ALAB $211.60 vs $211.81), most are under 5 cents.
- **History:** daily candles through Nov 16 are from Massive. % change is vs. the Nov 16 close; "5D" is vs. the Nov 10 close.
- **Relative volume** = today's Stock Analysis volume ÷ the 20-day average from Massive. It was read within an hour of the close and may be revised slightly. Twelve Data's volume figures were unusable again (e.g. 0.43M shares for RKLB, 2.96B for NVDA).
- **After-hours:** the Twelve Data extended quote with its own timestamp. These are **early prints taken before Nvidia's 17:00 ET conference call**, so they can move a lot before the 20:00 ET close of the after-hours session. Where the timestamp is 15:59 ET there was no post-close print.
- **Indicators** are computed by me from the candles and include today's close: SMA 20/50/100/200, RSI(14, Wilder), MACD(12,26,9), ATR(14). Intraday checks use Twelve Data 30-minute regular-session bars.
- **Morning brief:** setups are checked against `reports/2026-11-17-market-intelligence.md` on branch `claude/pensive-clarke-thwkwi` (not on this branch). Its three extra candidates are **KRMN, ALAB, SYM**.
- **Filings:** checked through the SEC EDGAR submissions API at about 21:50 UTC for every watchlist company, for filings dated Nov 16–17. Documents were read directly from EDGAR.
- **Labels:** **[Confirmed]** = SEC filing or company release. **[Reported]** = media. **[Est.]** = unconfirmed. **Opinion** = my analysis. Not personalised financial advice.

---

### 🧭 The day in three lines
1. **Nvidia beat and raised.** Q3 FY27 revenue was **$115.8B** vs. a $108B ±2% guide, and the Q4 guide is **$130B ±3%** (incl. an extra week, no China data-center compute) **[Confirmed]**. Gross margin is guided down to 71–72% from 74.8%. The early after-hours reaction was **muted: NVDA +2.4% to $159.16 at 16:40 ET**. AI names led after hours: **NBIS +5.3%, ALAB +4.9%, CRWV +4.4%, MRVL +3.6%, MU +1.9%, SMH +2.0%**.
2. **The regular session was a "test of the lows and a bounce".** SMH (low $445.32) and QQQ (low $646.64) both **undercut their Nov 5 lows intraday** (morning alert levels $445.6 / $647), then closed back above them. **SPY closed $732.44, just $0.10 above its 200-day SMA ($732.34).** The Dow fell 1.64%, S&P 500 −1.03%, Nasdaq −0.74%; VIX 25.5 **[Reported]**. Media tied part of the slide to a reported outage of a classified NSA network, which the NSA called "temporary degradation" during maintenance **[Reported]**.
3. **Morning setups: 2 entries triggered (BKSY, KRMN pullback zones filled), 1 conditional (MU hammer in zone), none stopped out, no targets hit.** Space names stayed weak: ASTS closed $0.01 above its 52-week-low reference after issuing **10M shares to Firefly** (filed today), VELO made a new low.

---

### 1. Session recap

| Ticker | Close | % chg | 5D | Open | High | Low | Rel. vol | After-hours (ET) | AH vs close |
|---|---|---|---|---|---|---|---|---|---|
| **SPY** | 732.44 | −1.01% | −2.3% | 738.39 | 739.76 | 727.00 | **1.42×** | 734.08 @ 16:20 | +0.2% |
| **QQQ** | 656.95 | −0.73% | −2.6% | 663.05 | 663.36 | 646.64 | 1.05× | 660.88 @ 16:40 | +0.6% |
| **SMH** | 460.10 | −0.39% | −4.9% | 466.43 | 466.43 | 445.32 | 0.99× | 469.25 @ 16:38 | +2.0% |
| RKLB | 55.05 | −4.04% | −12.2% | 57.44 | 58.60 | 53.42 | 0.72× | 56.30 @ 16:31 | +2.3% |
| BKSY | 21.90 | −5.40% | −8.1% | 23.25 | 23.66 | 21.35 | 0.97× | no post-close print | n/a |
| RDW | 6.78 | −3.83% | −16.6% | 7.07 | 7.20 | 6.63 | 0.84× | no post-close print | n/a |
| ASTS | 27.59 | −3.46% | −18.1% | 28.51 | 29.23 | **27.01** | 1.10× | 28.29 @ 16:35 | +2.5% |
| MRVL | 148.74 | **+2.33%** | −3.7% | 150.20 | 150.95 | 140.90 | 0.85× | 154.10 @ 16:34 | +3.6% |
| MU | 712.42 | −0.92% | −1.8% | 726.20 | 726.99 | **666.88** | 1.03× | 726.14 @ 16:38 | +1.9% |
| VELO | 3.26 | −8.04% | −46.0% | 3.60 | 3.74 | **3.16** | **1.46×** | no post-close print | n/a |
| NBIS | 106.04 | −1.02% | −20.9% | 108.87 | 111.90 | 102.25 | 1.00× | 111.70 @ 16:38 | **+5.3%** |
| CRWV | 49.89 | +0.02% | +2.4% | 49.70 | 50.79 | 46.84 | 0.71× | 52.10 @ 16:35 | +4.4% |
| OUST | 30.48 | −2.40% | −20.3% | 31.78 | 31.99 | 29.19 | 0.67× | no post-close print | n/a |
| KRMN | 35.55 | −5.17% | −19.0% | 36.64 | 38.34 | 34.85 | 0.48× | no post-close print | n/a |
| ALAB | 211.60 | **+4.58%** | −2.1% | 207.63 | 212.03 | 190.75 | 1.00× | 221.88 @ 16:35 | +4.9% |
| SYM | 33.06 | −3.56% | −12.1% | 34.22 | 34.60 | **32.43** | 1.16× | no post-close print | n/a |
| *NVDA (context)* | 155.46 | −0.44% | −8.0% | 156.90 | 158.19 | 150.33 | **1.64×** | 159.16 @ 16:40 | +2.4% |

- **Shape of the day (from 30-minute bars):** a small opening bounce, then a flush. **Every name on the list made its low in the 10:30–11:00 ET bar** (SYM at 11:30). After that, AI/semis recovered: MU rallied from $666.88 to $712.42, with a +2% jump in the final 30 minutes (high $721.55); ALAB closed at the high of the day; MRVL recovered from $140.90 to $148.74. Space and small caps did not bounce.
- **Leaders vs. laggards:** semis/AI infrastructure outperformed (MRVL +2.3%, ALAB +4.6%, CRWV flat, MU −0.9%), space and small caps lagged (BKSY −5.4%, KRMN −5.2%, VELO −8.0%, RKLB −4.0%).
- **Macro [Reported, Yahoo Finance live blog]:** Dow 50,759.42 (−1.64%), S&P 500 7,340.53 (−1.03%), Nasdaq 24,328.38 (−0.74%), Russell 2000 2,701.87 (−1.50%). 10-year yield 5.10%. VIX 25.46 (+11%). October retail sales +0.2% m/m vs. +0.1% expected; September revised up to +0.8%. St. Louis Fed's Musalem called for hikes "sooner" ([Yahoo Finance](https://finance.yahoo.com/markets/live/stock-market-today-tuesday-november-17-dow-sp-500-nasdaq-nvidia-earnings-retail-sales-143848454.html)).

---

### 2. Morning setups: what happened

| Ticker | Morning plan | Result | Detail |
|---|---|---|---|
| **BKSY** | (A) Pullback buy $21.30–22.20, or (B) close above $24.95 on ≥1.5× volume. Stop $20.30. T1 $27.20–27.70, T2 $30 | ✅ **TRIGGERED (A: pullback zone filled)** | Low $21.35, close $21.90, both inside the zone. A mid-zone fill (~$21.75) is +0.7%. Stop not hit. **Caution (opinion):** it lost the $22.2 flag low and closed in the bottom quarter of its range on 0.97× volume, heavier than the flag's 0.6×. The pullback was the plan, but the candle is not a reversal. |
| **KRMN** | Buy $34.50–36.00. Invalidation: close below $32. T1 $42, T2 $47.50 | ✅ **TRIGGERED (zone filled)** | Low $34.85, close $35.55, both in the zone. Volume very light (0.48×). Note: it spiked to $38.34 first and was rejected, closing near the low. Invalidation not hit. |
| **MU** | Buy $655–690 **with a reversal candle**. Stop $620. T1 $767, T2 $828 | ⚠️ **TRIGGERED, conditionally** | Reached the zone (low $666.88 at ~10:30 ET) and closed $712.42 with a **hammer**: lower shadow $45.5, upper shadow $0.6, small red body. That meets "reversal candle", but the candle was only complete at the close, **above** the zone. At $712 the original stop/target math no longer works (see section 5). Stop not hit. |
| **RKLB** | Zone $53.50–56.00. Confirmation: close above $58.50 **or** a 1h higher low in the zone **after** Nvidia. Stop $49.80 | ⏸ **NOT TRIGGERED: in zone, no confirmation** | Low $53.42 (8 cents under the zone), close $55.05 in the zone. Intraday higher lows formed after 10:30 ET, but before the Nvidia print, so they do not count. AH $56.30. Stop not hit. |
| **OUST** | Buy $28.50–29.50 on a reversal candle or a reclaim of $32.50. Stop $26.80 | ⏸ **NOT TRIGGERED: zone touched, no confirmation** | Low $29.19 in the zone, close $30.48. Red candle with a modest lower wick; not a reversal. Light volume (0.67×). |
| **MRVL** | Buy $133–138 on a reversal candle that holds $132.5. Stop $124 | ⏸ **NOT TRIGGERED** | Low $140.90, $2.90 above the zone. It did print a **hammer-style reversal** (closed $148.74, +2.3%) and AH $154.10. $132.5 support intact. |
| **CRWV** | Buy $44–46.5 on a reversal candle. Stop $40 | ⏸ **NOT TRIGGERED** | Low $46.84, 34 cents above the zone. Closed flat at $49.89. AH $52.10. |
| **ALAB** | Buy $180–190 on a reversal, **after** Nvidia. Invalidation close below $168 | ⏸ **NOT TRIGGERED** | Low $190.75, 75 cents above the zone, before the print. Closed at the high ($211.60, +4.6%), a strong reversal. AH $221.88. |
| **SYM** | No trade before Nov 23 earnings. Invalidation: close below $32.50 | ⏸ **NOT TRIGGERED; level warning** | New 52-week low intraday at $32.43, but closed $33.06, above $32.50. The $33.20–34.00 "hold" area for after earnings already failed on a closing basis. |
| **ASTS** | AVOID. Alert: close below $27.58 | 🛑 **AVOID stands; alert missed by 1 cent** | New 52-week low intraday at $27.01; closed **$27.59**. Dilution filing today (section 3). |
| **RDW** | AVOID. Watch for a double bottom at $6.06–6.20 | 🛑 **AVOID stands** | Low $6.63, close $6.78. Not yet at the $6.06–6.20 test. |
| **VELO** | AVOID | 🛑 **AVOID stands** | New 52-week low at $3.16 on 1.46× volume, closed $3.26. |
| **NBIS** | AVOID | 🛑 **AVOID stands** | New 60-day low at $102.25, closed $106.04. AH +5.3% after Nvidia. |

**Summary: triggered 2 (BKSY, KRMN), conditionally triggered 1 (MU), zone touched without confirmation 2 (RKLB, OUST), not reached 3 (MRVL, CRWV, ALAB), stopped out 0, targets hit 0.**

**Morning alert levels:** SMH below $445.6 / QQQ below $647 → **breached intraday only, both closed back above** (not a closing breakdown). MRVL $132.5 intact. ASTS $27.58 → held on a closing basis by 1 cent. BKSY breakout level $24.95 not reached.

---

### 3. Earnings, filings and material news (Nov 17, incl. after-hours)

**Sector driver: Nvidia Q3 FY27 [Confirmed]** ([release via StockTitan](https://www.stocktitan.net/news/NVDA/nvidia-announces-financial-results-for-third-quarter-fiscal-fpx9dw5egxqa.html), 16:20 ET)
- Revenue $115.8B (+103% y/y, +20% q/q). Data Center $107.6B (+110% y/y).
- GAAP EPS $2.70, non-GAAP $2.68 (about $2.48 expected **[Reported]**). GAAP gross margin 74.8%.
- **Q4 guide: $130.0B ±3%**, including an extra week, and **no Data Center compute revenue from China**. Consensus was about $124.7B **[Reported]**. Gross margin guide **71–72%**, a step down.
- $28.1B returned to shareholders in the quarter; about $227.3B left on the buyback authorization (the $150B increase was approved in September, not today).
- Early reaction: +2–3% after hours, smaller than the ~8% move options implied **[Reported]** ([CBS News](https://www.cbsnews.com/news/nvidia-earnings-jensen-huang-colette-kress/), [Benzinga](https://www.benzinga.com/markets/earnings/26/11/63372441/nvidia-stock-jumps-on-q3-double-beat-strong-outlook-explosive-demand-for-vera-rubin), [InvestingLive](https://investinglive.com/stocks/nvidia-price-up-tops-forecasts-by-7-billion-as-kress-steers-first-report-since-huang-exit/)). The call (17:00 ET) was still to come when prices were read.

**Watchlist**

- **ASTS: material dilution filing [Confirmed].** A [424B5 prospectus supplement](https://www.sec.gov/Archives/edgar/data/1780312/000149315226052716/form424b5.htm) (filed 08:30 ET) and an [8-K](https://www.sec.gov/Archives/edgar/data/1780312/000149315226052865/form8-k.htm) (filed 16:35 ET) register **10,000,000 new Class A shares issued to Firefly Aerospace**. They are payment for a perpetual license to build Firefly's Miranda and Vira engines for AST's own planned 20-ton rocket ("Blacklift"). Total consideration under the Nov 6 agreement is **$400M in cash plus an estimated 10–14M shares**; up to ~4M more shares could follow. AST receives no cash from the issuance, and part of the shares are locked up. Opinion: this adds supply and a large cash commitment to a balance sheet already carrying $4.08B of long-term debt. An analyst called the 2-year rocket plan "totally unrealistic" **[Reported]** ([Stocktwits/TradingView](https://www.tradingview.com/news/stocktwits:6ea5e629d094b:0-why-catching-spacex-is-getting-harder-analyst-calls-ast-s-2-year-rocket-plan-totally-unrealistic-rocket-lab-is-still-building-one/)).
- **MRVL: Form 4 (routine) [Confirmed].** An officer (Justin Scarpulla) had 393 shares withheld for taxes at $156.76 on Nov 15 on RSU vesting ([Form 4](https://www.sec.gov/Archives/edgar/data/1835632/000162828026074462/xslF345X06/wk-form4_1794947404.xml)). Not a discretionary sale. Three more Form 4s and the 10b5-1 Form 144 were filed Nov 16 (covered this morning).
- **NBIS: Form 4 (small) [Confirmed].** Director John Boynton sold 4,502 shares on Nov 13 at $109.79–118.00, leaving about 398,687 ([Form 4](https://www.sec.gov/Archives/edgar/data/1513845/000151384526000151/xslF345X06/form4.xml)). Immaterial in size.
- **RKLB:** No material news. Only opinion pieces (Motley Fool).
- **BKSY:** No material news. It presented at the Craig-Hallum conference today; no release found.
- **RDW:** No material news.
- **MU:** No company news. Intraday, the stock fell toward $670 on sector selling, opposition to data-center expansion and weaker Kioxia guidance **[Reported]** ([FX Leaders](https://www.fxleaders.com/news/2026/11/17/micron-stock-tests-support-below-700-as-big-tech-attack-weighs-on-chip-companies/)). It reversed after midday and gained after hours on Nvidia.
- **VELO, CRWV, OUST, KRMN, ALAB, SYM:** No material news. No 8-K, Form 4, S-3 or ATM filings dated Nov 16–17 on EDGAR for these names, or for RKLB, BKSY, RDW, MU.

No watchlist company reported earnings today.

---

### 4. Technical update (daily close vs. key averages)

| Ticker | Close | SMA20 | SMA50 | SMA100 | SMA200 | RSI | MACD hist (prev) | ATR % | Change in structure |
|---|---|---|---|---|---|---|---|---|---|
| SPY | 732.44 | 755.86 | 763.15 | 760.37 | **732.34** | 37.5 | −1.60 (−0.75) | 1.6% | **On** the 200-day ($0.10 above). Below all others. Distribution volume 1.42× for a second day. |
| QQQ | 656.95 | 689.58 | 715.49 | 713.41 | 682.59 | 36.5 | −1.46 (−0.84) | 2.5% | Undercut the Nov 5 low ($647.05) intraday, closed back above. |
| SMH | 460.10 | 509.50 | 555.43 | 564.32 | 524.44 | 35.3 | −2.38 (−1.90) | 5.2% | Undercut the Nov 5 low ($445.59) by $0.27, then closed +$15 off the low. AH +2%. |
| RKLB | 55.05 | 56.29 | 62.11 | 68.33 | 78.07 | 45.2 | +0.79 (+1.26) | 8.9% | **Lost the 20-day** (first close below since Nov 6). Histogram fading. Light volume. |
| BKSY | 21.90 | 20.00 | 20.61 | 22.94 | 27.01 | 54.4 | +0.52 (+0.71) | 7.5% | **Lost the 100-day** and the $22.2 flag low. Still above 20/50-day. Uptrend intact while above $20.3. |
| RDW | 6.78 | 8.01 | 9.40 | 10.08 | 10.83 | 36.7 | −0.01 (+0.03) | 10.2% | Below all MAs; histogram turned negative. |
| ASTS | 27.59 | 36.47 | 48.26 | 57.44 | 72.82 | 31.7 | −0.15 (+0.03) | 14.3% | New 52-week low at $27.01; histogram turned negative. |
| MRVL | 148.74 | 185.58 | 226.11 | 222.97 | 187.68 | 34.2 | −1.50 (−2.17) | 11.0% | Hammer above $132.5 support; histogram improving. Still under AVWAP $150.8 (AH $154.10 is above it). |
| MU | 712.42 | 819.52 | 932.07 | 933.85 | 768.50 | 37.5 | −3.50 (−2.83) | 8.3% | **Hammer** off $666.88, defending the $650–690 base. Below 200-day. |
| VELO | 3.26 | 5.71 | 8.08 | 10.40 | 12.77 | 25.3 | −0.13 (−0.10) | 21% | New low on 1.46× volume; no base. |
| NBIS | 106.04 | 144.70 | 189.46 | 201.30 | 179.55 | 33.7 | −1.96 (−1.58) | 16.3% | New 60-day low $102.25; closed slightly under the AVWAP ($107.56). |
| CRWV | 49.89 | 53.82 | 70.81 | 78.24 | 88.58 | 40.6 | +0.99 (+1.11) | 12.5% | Range $40.6–62 intact; held above $46.5. |
| OUST | 30.48 | 32.44 | 35.36 | 38.26 | 32.97 | 43.1 | +0.10 (+0.40) | 10.0% | Second close below 200-day; histogram near zero. |
| KRMN | 35.55 | 39.00 | 35.88 | 43.22 | 59.69 | 44.9 | −0.34 (+0.04) | 9.8% | **Closed below the 50-day** ($35.88); histogram turned negative. Gap base $34.18 is next. |
| ALAB | 211.60 | 239.09 | 290.56 | 309.47 | 258.02 | 39.0 | +0.26 (−0.35) | 11.2% | **Bullish reversal** (low $190.75 → close at high); histogram turned positive; reclaimed AVWAP ($205.6). |
| SYM | 33.06 | 37.34 | 40.21 | 41.12 | 46.64 | 31.8 | −0.29 (−0.20) | 6.3% | New 52-week low $32.43. |

No watchlist name broke out on volume today. **Breakdowns of note:** VELO (new low, 1.46×), ASTS (new 52-week low intraday, 1.10×), SYM (new 52-week low, 1.16×). **Reversals:** MU, MRVL, ALAB (all on roughly average volume, so not yet confirmed).

---

### 5. Plan for tomorrow (Wednesday, Nov 18)

**Posture (opinion): cautious, selective.** Nvidia removed the binary event with a beat and a raised guide, but the reaction is small so far, and the macro backdrop (10-year 5.1%, hike talk from Fed speakers, VIX 25) is unchanged. Treat a gap up in AI names as something to confirm, not to chase. If SMH holds above $460 and closes above $470, today's undercut-and-reclaim of the Nov 5 lows becomes a valid higher-low test; a close back under $445 cancels that view.

| Ticker | Signal | Entry plan | Stop | Targets | R/R |
|---|---|---|---|---|---|
| **BKSY** | **POTENTIAL BUY: position open from the zone** | Hold the zone fill. Add only on a close back above $23.70 (today's high area) | **$20.30** | T1 $27.20, T2 $30.00 | From $21.90: 3.3 / 5.1 |
| **KRMN** | **POTENTIAL BUY: position open, weaker** | Hold; no adds below the 50-day ($35.88) | Close below **$32.00**; tighter option $34.10 (below the gap base) | T1 $42, T2 $47.50 | From $35.55: 1.8 / 3.4 (with $32 stop) |
| **MU** | **POTENTIAL BUY on a pullback** (upgraded from Hold) | Don't chase the AH $726. Buy $690–705 if the hammer low holds | **$660** (below the $666.88 hammer low) | T1 $767 (200-day), T2 $828 | From $697: 1.9 / 3.5 |
| **ALAB** | **HOLD / MONITOR → potential buy** | Pullback to $205–212 (AVWAP/today's close) that holds after the AH gap | **$189** (below today's low) | T1 $230, T2 $258 | From $209: 1.05 / 2.45 (T2 is the trade) |
| **MRVL** | **HOLD / MONITOR** | Buy only on a **daily close above $151** (AVWAP) — AH suggests it may open there | **$139.50** (below today's low) | T1 $165, T2 $187 | From $151: 1.2 / 3.1. Earnings Dec 1 = gap risk |
| **RKLB** | **POTENTIAL BUY (confirmation required)** | Zone $53.50–56.00 unchanged. Confirmation: daily close above **$58.50**, or a 1h higher low inside the zone **tomorrow** | **$49.80** | T1 $64, T2 $68 | From $55: 1.7 / 2.5 |
| **CRWV** | **HOLD / MONITOR** | Zone $44–46.5 on a reversal, **or** a close above $54 (20-day / AVWAP $51.89 reclaimed) | $40.00 (zone) / $48.50 (breakout) | T1 $54.50, T2 $62 | Zone from $45.5: 1.6 / 3.0 |
| **OUST** | **POTENTIAL BUY (confirmation required)** | Zone $28.50–29.50 with a reversal candle, or a reclaim of $32.50 | $26.80 | T1 $34.80, T2 $38.50 | From $29: 2.6 / 4.3 |
| **SYM** | **HOLD / MONITOR until Nov 23 earnings** | Post-earnings: reclaim of $34.60 with a bullish reaction, or $37.70 (20-day) | Close below **$32.40** (today's low) | T1 $40.40, T2 $45.60 | Wait |
| **NBIS** | **AVOID / HIGH RISK** | AH +5.3% is a reaction, not a base. Revisit only on a close above $120 | — | — | — |
| **ASTS** | **AVOID / HIGH RISK** | New share issuance plus $400M cash commitment. A close below $27.01 leaves no chart support | — | — | — |
| **RDW** | **AVOID / HIGH RISK** | Watch for a double bottom at $6.06–6.20, then a reclaim of $7.45 | — | — | — |
| **VELO** | **AVOID / HIGH RISK** | No base | — | — | — |

R/R = (target − entry) ÷ (entry − stop). Entry zones, stops, targets and signals are **opinions**.

**Key events tomorrow (all times ET)** ([Kiplinger calendar](https://www.kiplinger.com/investing/economy/this-weeks-economic-calendar), [Newsquawk week ahead](https://www.newsquawk.com/headlines/week-in-focus--16-20th-november-2026-highlights-include-us-retail-sales-fomc-minutes-chinese-activity-data-pboc-lpr-rba-minutes-uk-inflation-and-uk-jobs), [StockTitan earnings calendar](https://www.stocktitan.net/articles/earnings-calendar-week-of-november-16-2026))
- **08:30:** October housing starts and building permits (consensus 1.23–1.27M; sources differ **[Est.]**).
- **10:00:** October pending home sales.
- **13:35:** Fed Governor Michael Barr speaks. **14:30:** NY Fed President John Williams speaks.
- **14:00: FOMC minutes** (Oct 27–28 meeting, held at 3.75–4.00%). Futures price a Dec 9 hike at about 89% (per this morning's brief).
- **Earnings (pre-market):** TJX, Lowe's, Target, Williams-Sonoma, PDD. **After the close:** Palo Alto Networks. No watchlist company reports.
- **Watchlist events:** MU TomorrowX fireside chat (confirmed in this morning's brief). BKSY Needham virtual event is **Nov 19**.
- **Overnight:** Nvidia's call commentary (China, gross margin, customer financing) may move AH prices well beyond the early prints above.

---

**Sources:** Massive/Polygon daily aggregates; Twelve Data quotes and 30-minute bars; Stock Analysis daily history pages; SEC EDGAR (ASTS [424B5](https://www.sec.gov/Archives/edgar/data/1780312/000149315226052716/form424b5.htm) and [8-K](https://www.sec.gov/Archives/edgar/data/1780312/000149315226052865/form8-k.htm), MRVL and NBIS Form 4s linked above); [Nvidia release](https://www.stocktitan.net/news/NVDA/nvidia-announces-financial-results-for-third-quarter-fiscal-fpx9dw5egxqa.html); [Yahoo Finance live blog](https://finance.yahoo.com/markets/live/stock-market-today-tuesday-november-17-dow-sp-500-nasdaq-nvidia-earnings-retail-sales-143848454.html); [CBS News](https://www.cbsnews.com/news/nvidia-earnings-jensen-huang-colette-kress/); [Benzinga](https://www.benzinga.com/markets/earnings/26/11/63372441/nvidia-stock-jumps-on-q3-double-beat-strong-outlook-explosive-demand-for-vera-rubin); [InvestingLive](https://investinglive.com/stocks/nvidia-price-up-tops-forecasts-by-7-billion-as-kress-steers-first-report-since-huang-exit/); [NBC News on the NSA network](https://www.nbcnews.com/politics/national-security/classified-nsa-network-went-no-indication-was-attack-sources-say-rcna609859); [Kiplinger](https://www.kiplinger.com/investing/stocks/dow-dives-848-points-as-nsa-outage-wrecks-tech-stock-market-today); [FX Leaders on MU](https://www.fxleaders.com/news/2026/11/17/micron-stock-tests-support-below-700-as-big-tech-attack-weighs-on-chip-companies/).
