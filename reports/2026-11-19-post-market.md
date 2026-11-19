## 🌙 Post-Market Briefing: Thursday, November 19, 2026

**Data notes (please read first)**
- **Retrieved:** 2026-11-19, about 21:32–21:45 UTC (23:32–23:45 Bucharest; 16:32–16:45 ET). The after-hours session runs until 20:00 ET, so **the after-hours prices below are early prints only**.
- **Today's prices.** Massive (Polygon) again refused same-day data on this plan: `/v1/open-close` returned "NOT_AUTHORIZED … before end of day", and same-day minute bars were not available. Today's open/high/low/close and volume therefore come from the **Stock Analysis** daily history pages. Every close was cross-checked against the **Twelve Data** quote and matched within 15 cents. The largest gaps were MRVL $138.47 vs $138.36, CRDO $117.76 vs $117.57 and SPY $715.87 vs $715.78.
- **History:** daily candles through Nov 18 come from Massive. % change is vs. the Nov 18 close, and "5D" is vs. the Nov 12 close. The hourly bars used for the confirmation checks are Twelve Data (regular session, ET).
- **Relative volume** = today's Stock Analysis volume ÷ the 20-day average from Massive. It was read within about 45 minutes of the close and may be revised slightly. Twelve Data's own daily volume figure was inconsistent across tickers and was not used.
- **After-hours:** Twelve Data extended quotes, each with its own ET timestamp. "No AH print" means the last trade was at 15:59 ET.
- **Indicators** are computed by me from the candles and include today's close: SMA 20/50/100/200, RSI(14, Wilder), MACD(12,26,9), ATR(14).
- **Morning brief:** setups are checked against `reports/2026-11-19-market-intelligence.md` on branch `claude/pensive-clarke-x3xp8f`. It is not on this branch. Its three extra candidates are **CRDO, KTOS and PL**.
- **Filings:** I checked the SEC EDGAR submissions API at about 21:40 UTC for every watchlist company, the three candidates and NVDA. The window was filings dated Nov 18–19, including after-hours on the 18th.
- **Labels:** **[Confirmed]** = SEC filing or company release. **[Reported]** = media. **[Est.]** = unconfirmed. **Opinion** = my analysis. This is not personalised financial advice.

---

### 🧭 The day in three lines
1. **A broad reversal day, and the market's "cut exposure" rule fired.** Futures and the open were green. SPY traded up to $739.90 (above its 200-day SMA) and SMH reached +4.4%. Then the tape rolled over from about 11:30 ET, around the time Anthropic began trading, and **nearly every name closed in the bottom 8% of its daily range**. Closes:
   - **SPY $715.87 (−1.96%)**, a **6th straight loss**, its second close under the 200-day ($732.69), and **below the $726.8 "cut exposure" level**.
   - QQQ −2.19%, SMH −2.62% to $447.48, only **$2 above the $445.3 crash-low line**.
   - Index closes **[Reported]**: S&P 500 −2.02%, Nasdaq −2.25%, Dow −2.19% (back below 50,000), Russell 2000 −2.18%. **VIX 28.44 (+15.8%)**; the 10-year yield was roughly flat at 5.05%.
2. **AI infrastructure led the decline.**
   - **NBIS −9.4%** broke below $100 on 1.30× volume, so the morning's bearish trigger fired.
   - **CRWV −6.1%**, **MRVL −4.9%**, **MU −2.1%** after trading as high as $760.
   - **NVDA −3.3% to $145.98**, a new 52-week low, with RSI at 19.6.
   - **BKSY −9.0%** closed below $19.10, which **invalidates the morning's top-ranked setup**.
3. **No setup triggered. One was invalidated (BKSY), and NBIS hit its bearish trigger.**
   - RKLB and OUST traded inside their buy zones but closed at the lows with no confirmation.
   - MRVL missed its zone by 35 cents. In early after-hours MRVL ($137.24) and PL ($11.50) are inside their zones, and MU ($680.55) and CRWV ($44.28) are approaching theirs.
   - Nothing was stopped out and no targets were hit.

---

### 1. Session recap

| Ticker | Close | % chg | 5D | Open | High | Low | Rel. vol | After-hours (ET) | AH vs close |
|---|---|---|---|---|---|---|---|---|---|
| **SPY** | 715.87 | −1.96% | −5.4% | 737.46 | 739.90 | **715.65** | **1.49×** | 716.38 @ 16:33 | +0.1% |
| **QQQ** | 645.04 | −2.19% | −6.3% | 671.09 | 676.49 | 644.34 | 1.35× | 643.42 @ 16:29 | −0.3% |
| **SMH** | 447.48 | −2.62% | −10.8% | 473.05 | 479.96 | 447.20 | 0.85× | 445.69 @ 16:32 | −0.4% |
| RKLB | 50.99 | −3.92% | −20.4% | 55.21 | 56.83 | 50.45 | 0.82× | 50.81 @ 16:32 | −0.4% |
| BKSY | 18.79 | **−9.01%** | −19.1% | 20.95 | 21.60 | 18.61 | 0.85× | no AH print | n/a |
| RDW | 6.51 | −4.55% | −18.9% | 7.00 | 7.24 | 6.46 | 0.94× | 6.50 @ 16:16 | −0.2% |
| ASTS | 25.55 | +0.24% | −25.9% | 27.62 | 28.47 | 25.39 | 0.95× | no AH print | n/a |
| MRVL | 138.47 | −4.86% | −15.8% | 151.32 | 154.51 | 138.35 | 0.94× | 137.24 @ 16:33 | −0.9% |
| MU | 690.44 | −2.10% | −13.5% | 740.33 | 760.01 | 689.28 | 1.10× | 680.55 @ 16:34 | −1.4% |
| VELO | 3.39 | −2.59% | −23.1% | 3.63 | 3.85 | 3.39 | 1.07× | no AH print | n/a |
| NBIS | 96.92 | **−9.39%** | −24.7% | 111.59 | 115.18 | **96.54** | **1.30×** | 95.50 @ 16:31 | −1.5% |
| CRWV | 44.91 | **−6.10%** | −20.7% | 50.01 | 52.86 | 44.36 | 1.13× | 44.28 @ 16:30 | −1.4% |
| OUST | 28.16 | −3.89% | −23.1% | 30.85 | 31.41 | 28.10 | 0.97× | 28.18 @ 16:00 | +0.1% |
| CRDO | 117.76 | −4.21% | −15.8% | 128.83 | 131.15 | 117.21 | 0.66× | 117.07 @ 16:24 | −0.6% |
| KTOS | 29.65 | −1.95% | −14.7% | 30.56 | 31.37 | **29.29** | 1.24× | no AH print | n/a |
| PL | 11.63 | −3.49% | −16.3% | 12.68 | 13.11 | 11.60 | **1.31×** | 11.50 @ 16:03 | −1.1% |
| *NVDA (context)* | 145.98 | −3.30% | −12.2% | 152.92 | 158.13 | **145.71** | 1.26× | 144.41 @ 16:35 | −1.1% |

- **Shape of the day (fact, from the daily and hourly candles):** this was the **second gap-up-then-fade day in a row**.
  - Every name except ASTS and VELO opened above Wednesday's close, and most also traded above Wednesday's high.
  - Every name then closed in the **bottom 8% of its range**. KTOS (17%) was the only exception.
  - The hourly bars show the break came in the **11:30 ET bar**. SPY fell from $731.7 to $717.5 in that hour, and SMH from $468.3 to $448.0.
  - Opinion: a high-to-close reversal on rising index volume (SPY 1.49×) looks like distribution. It does not look like a washed-out low.
- **Volume:** heavier at the index level (SPY 1.49×, QQQ 1.35×) and in NBIS (1.30×), PL (1.31×), NVDA (1.26×) and KTOS (1.24×). The space small caps and CRDO were **lighter** (0.66–0.95×).
- **Macro and market drivers [Reported]** (from the [Yahoo Finance live blog](https://finance.yahoo.com/markets/live/stock-market-today-thursday-november-19-dow-sp-500-nasdaq-anthropic-ipo-live-141306032.html)):
  - **Anthropic (ANT) debut:** priced at $83 and opened at **$111.50**. It fell about 13% from the first trade within 30 minutes, which Yahoo called "the worst start for a big IPO since 2008". It closed **+15–17%**, roughly $95–97; the figures in the report conflict, so I have not used an exact close.
  - The live blog says chip stocks "erased gains" once ANT began trading, and that retail investors sold single stocks to fund ANT buying.
  - **AMD fell about 8–9%** after Hunterbrook disclosed a short position citing China and export concerns. Motley Fool covered the same story ([Motley Fool](https://www.fool.com/investing/2026/11/19/first-nvidia-now-amd-a-short-seller-just-put-its-china-business-under-the-microscope/)).
  - Initial jobless claims were about **203K** vs about 197K expected; the figure comes from the calendar widget on the page. The Philly Fed result was not available in my sources.
  - Walmart beat and raised guidance; healthcare (UNH −5%) was also weak.
  - Benzinga headlined the S&P 500's sixth straight loss and Anthropic's jump ([Benzinga](https://www.benzinga.com/markets/equities/26/11/63446162/stock-market-today-anthropic-ipo-debut-sp-500-sixth-loss-november-19); the page returned 403, so this is the headline only).
  - Fed speakers were on the calendar: Hammack, Goolsbee, Barr, Barkin and Paulson ([TD calendar](https://economics.td.com/domains/economics.td.com/documents/reports/bottom-line/tables/2026-11-13/upcoming.htm)). I found **no readout** of their remarks in my sources.

---

### 2. Morning setups: what happened

| Ticker | Morning plan | Result | Detail |
|---|---|---|---|
| **BKSY** | POTENTIAL BUY. Zone $19.30–20.30. Confirmation: close above $19.10 **and** a 4H close above $21. Stop $18.30 | ❌ **INVALIDATED** | It traded through the zone and touched $21.60 in the first minutes. The first hourly bar closed at $19.62, so there was no 4H close above $21. **Close $18.79 < $19.10**, which hits the bearish trigger. The $18.30 stop was **not** hit (low $18.61). |
| **RKLB** | Zone $49.50–51.00. Confirmation: a 4H reversal plus a 1H close above the 1H 20-EMA. Stop $45.80 | ⏸ **NOT TRIGGERED: in the zone, no confirmation** | Low $50.45, close $50.99 (top of the zone). Every hourly close was below the 1H 20-EMA, which was ~$53.7 at the close. Stop not hit. |
| **OUST** | Zone $27.40–28.40. Confirmation: a 4H higher low plus a 1H close above the 20-EMA. Stop $25.60 | ⏸ **NOT TRIGGERED: in the zone, no confirmation** | Low $28.10, close $28.16 (in the zone, at the low). The hourly 20-EMA (~$29.9) was never reclaimed. **$27.35 is intact.** |
| **MRVL** | Zone $133–138. Confirmation: a higher low above $132.5. Stop $124 | ⏸ **NOT REACHED (by 35 cents)** | Low $138.35, close $138.47. **After-hours $137.24 is inside the zone.** |
| **MU** | Zone $650–670. Confirmation: a 4H bullish engulfing candle that holds $650. Stop $610 | ⏸ **NOT REACHED** | High $760 then low $689.28. After-hours **$680.55** is $10 from the zone. |
| **CRWV** | Zone $41.00–43.50. Confirmation: a reversal with RVOL > 1.3. Stop $38.40 | ⏸ **NOT REACHED** | Low $44.36, close $44.91. After-hours $44.28. The 5 Nov low of $40.58 is intact. |
| **RDW** | Zone $6.05–6.35. Confirmation: a reversal candle. Stop $5.60 | ⏸ **NOT REACHED** | Low $6.46, close $6.51. |
| **CRDO** | Zone $111–116. Stop $103 | ⏸ **NOT REACHED** | Low $117.21, close $117.76. |
| **PL** | Zone $11.00–11.50. Stop $10.30 | ⏸ **NOT REACHED in the session** | Low $11.60. **After-hours $11.50 is at the top of the zone.** |
| **KTOS** | Trigger: reclaim $32.00–32.50 after a higher low. Stop $28.90 | ⏸ **NOT TRIGGERED** | High $31.37. **New 52-week low of $29.29.** The $28.90 invalidation level is intact. |
| **ASTS** | AVOID. Reassess on a close above $28.10 on volume | 🛑 **AVOID stands** | High $28.47 intraday, but the close was $25.55. Low $25.39 held above Wednesday's $25.16 low. |
| **NBIS** | AVOID. Bearish alert on a close below $100 | 🛑 **BEARISH TRIGGER FIRED** | **Close $96.92 on 1.30× volume.** After-hours $95.50. |
| **VELO** | AVOID. Needs a close above $4.15 | 🛑 **AVOID stands** | Closed at its low of $3.39. The $3.16 52-week low is intact. |

**Summary:**
- Triggered: **0**.
- In the zone without confirmation: **2** (RKLB, OUST).
- Invalidated: **1** (BKSY).
- Not reached: **6** (MRVL, MU, CRWV, RDW, CRDO, PL). Four of them are at or near their zones in after-hours.
- Bearish trigger hit: **NBIS**.
- Stopped out: **0**. Targets hit: **0**.

**Market rules from the morning and the prior evening:**
- SPY reclaim of $733 / $735: **intraday yes (high $739.90), but it failed**. It closed $24 lower.
- **SPY close below $726.8 (cut exposure): YES. It fired at $715.87.**
- SMH hold of $445: **held on the close ($447.48)**, but after-hours is $445.69, which is right on the line.

---

### 3. Earnings, filings and material news (Nov 19, incl. after-hours)

**Filings on EDGAR (Nov 18 after-hours through Nov 19)**
- **ASTS: 8-K, filed Nov 18 at 16:35 ET [Confirmed]** ([filing](https://www.sec.gov/Archives/edgar/data/1780312/000149315226053080/form8-k.htm)). This is Item 8.01 paperwork for the **780,052 Class A shares that ASTS may issue to Ligado and One Dot Six** in place of payments under the spectrum agreements, plus legal opinions. It is the same issuance as Wednesday's 424B5, so it adds **no new dilution beyond what was already reported**. Not new information.
- **KTOS: Form 4, filed Nov 18 at 20:04 ET [Confirmed]** ([filing](https://www.sec.gov/Archives/edgar/data/1069258/000150940926000013/primary_doc.xml)). Phillip D. Carrai, President of the STC Division, **sold 6,500 shares on Nov 16** at $31.92–32.96, about $0.21M. He holds 162,770 shares directly afterwards. Opinion: the sale is small relative to his holding and not material.
- **No filings dated Nov 19** (8-K, Form 4, S-3, 424B or ATM) for RKLB, BKSY, RDW, ASTS, MRVL, MU, VELO, NBIS, CRWV, OUST, CRDO, KTOS, PL or NVDA as of about 21:40 UTC. Late filings may still appear tonight.
- **Earnings released today:** none on the watchlist.

**News by ticker**
- **RKLB, BKSY, RDW, ASTS, MRVL, MU, VELO, NBIS, CRWV, OUST, CRDO, KTOS, PL:** **No material news.** The Massive news feed from Nov 18 21:00 UTC onward held only commentary and opinion pieces, and no company releases. Examples:
  - Motley Fool on Rocket Lab's Neutron order book ([link](https://www.fool.com/investing/2026/11/19/rocket-lab-sold-out-neutron-through-the-2030s-before-it-ever-flew-heres-why-the-stock-fell-after-earnings-anyway/)).
  - Motley Fool on CoreWeave's debt ([link](https://www.fool.com/investing/2026/11/19/will-coreweave-stock-investors-get-swallowed-by-its-debt/)).
  - Zacks on MRVL custom silicon ([link](https://www.zacks.com/stock/news/3032572/can-mrvl-s-custom-silicon-business-drive-its-next-growth-phase)).
  - Motley Fool on the PL–Stoke Space launch deal. That deal was announced Nov 9 ([SatNews](https://satnews.com/2026/11/09/planet-contracts-stoke-space-for-multi-launch-agreement-across-nova-rocket-fleet/)), so it is not new.
- **Sector drivers [Reported]:** Anthropic's debut pulled liquidity from AI names, and the AMD short report weighed on chips. Both are detailed in section 1. Opinion: neither changes any watchlist company's fundamentals. Both are flow and sentiment effects that can persist for a few sessions.

---

### 4. Technical update (daily, includes today's close)

| Ticker | Close | SMA20 | SMA50 | SMA100 | SMA200 | RSI(14) | MACD hist (prev) | ATR % | Position / change |
|---|---|---|---|---|---|---|---|---|---|
| SPY | 715.87 | 751.32 | 761.67 | 759.96 | **732.69** | 31.6 | −3.25 (−2.15) | 2.1% | Below all; **2nd close under the 200d, now 2.3% below it** |
| QQQ | 645.04 | 683.33 | 713.09 | 711.85 | 683.00 | 33.9 | −2.22 (−1.48) | 3.1% | Below all; **broke its 20-day low ($646.6)** |
| SMH | 447.48 | 500.85 | 550.88 | 560.51 | 525.08 | 33.0 | −2.81 (−2.38) | 6.1% | Below all; **$445.3 line holding by $2** |
| RKLB | 50.99 | 56.24 | 61.69 | 67.37 | 77.82 | 40.9 | **−0.07 (+0.35)** | 10.7% | **MACD histogram turned negative** |
| BKSY | 18.79 | 20.27 | 20.55 | 22.77 | 26.99 | 42.7 | +0.01 (+0.29) | 10.3% | **Lost the 20d and 50d**; histogram near zero |
| RDW | 6.51 | 7.84 | 9.24 | 9.98 | 10.79 | 35.1 | −0.06 (−0.03) | 11.4% | Below all; $6.06 is 7% away |
| ASTS | 25.55 | 35.03 | 46.83 | 56.20 | 71.98 | **29.8** | −0.40 (−0.35) | 15.7% | Below all; held above $25.16 |
| MRVL | 138.47 | 176.36 | 222.55 | 220.06 | 188.35 | 31.6 | −0.87 (−1.00) | 11.4% | Below all; at the top of the $132.5–138 support |
| MU | 690.44 | 800.80 | 919.88 | 924.81 | 771.48 | 35.9 | −4.05 (−3.69) | 9.5% | Below all; rejected from $760 |
| VELO | 3.39 | 5.39 | 7.79 | 10.11 | 12.66 | **27.6** | −0.11 (−0.13) | 20.3% | Below all; closed at the low |
| NBIS | 96.92 | 138.35 | 184.16 | 197.97 | 179.71 | 31.8 | −2.17 (−1.87) | 18.0% | **Breakdown below $100 on volume** |
| CRWV | 44.91 | 52.58 | 68.98 | 77.22 | 88.18 | 36.5 | +0.50 (+0.80) | 14.4% | Below all; histogram fading toward zero |
| OUST | 28.16 | 32.40 | 35.08 | 37.67 | 33.06 | 39.2 | **−0.39 (−0.16)** | 11.9% | Below all; 3% above the triple bottom |
| CRDO | 117.76 | 138.84 | 168.66 | 196.84 | 181.02 | 36.8 | −0.16 (−0.05) | 12.5% | Below all |
| KTOS | 29.65 | 36.72 | 40.77 | 46.53 | 58.75 | **28.0** | −0.60 (−0.57) | 8.2% | **New 52-week low ($29.29)** |
| PL | 11.63 | 13.32 | 14.97 | 18.87 | 25.81 | 35.4 | **−0.03 (+0.03)** | 9.1% | **Histogram turned negative**; near the $11.01 low |
| NVDA | 145.98 | 185.73 | 208.86 | 210.51 | 203.58 | **19.6** | −3.71 (−3.82) | 8.2% | **New 52-week low $145.71**; extremely oversold |

**Breakouts and breakdowns on volume**
- **NBIS:** breakdown below $100 on 1.30× volume. Its next historical support is the **March 2026 lows at $86.5–89.7**.
- **SPY:** a second close under the 200-day, on 1.49× volume and through the $726.8 lows. Opinion: last night I said two closes below it would confirm the break; **it is now confirmed**. The next support is the **late-April 2026 lows at $708–712**.
- **QQQ:** closed below its 20-day low. The next support is the April lows at $642, then $620.
- **KTOS and NVDA:** new 52-week lows, on 1.24× and 1.26× volume respectively.
- **BKSY:** lost its MA cluster ($20.3–20.6) and the $19.1 breakout level on below-average volume (0.85×). It is a failed retest, not yet a volume breakdown.
- **No breakouts.**

**Levels that changed**
- **SPY:** resistance is now $726.8, then $732.7 (200d). Support is $708–712.
- **SMH:** the $445.3 crash low is the line. Below it, the April lows sit at $433.6–435.2.
- **BKSY:** $19.1–19.5 flips to resistance. Support is the **$16.2–17.0 late-October base** (Oct 30–Nov 4 lows), then the $16.13 higher low.
- **NBIS:** $100 flips to resistance. Support is $86.5–89.7.
- **KTOS:** new low reference $29.29. No support below in my data window.
- **RKLB:** the $50.45 low now sits inside the zone, and $49.5 is the zone floor.
- **MU:** the $760 intraday high is a new lower-high reference. Support is $666.9, then $650.

---

### 5. Plan for tomorrow (Fri Nov 20)

**General stance (opinion): DEFENSIVE.**
- The SPY "cut exposure" rule fired, SPY's break of its 200-day is confirmed, VIX is above 28, and two days in a row strong opens were sold.
- **No new full-size entries.** Use quarter- to half-size positions only, and only at the predefined zones **with** confirmation.
- **Re-enable normal risk only after SPY closes back above $726.8.**
- **Sector stop:** an SMH close below $445.3 means a sector-wide breakdown. If it happens, stand aside on all AI and semiconductor setups (MU, MRVL, CRWV, CRDO).
- Opinion: RSI near 30 on SPY, QQQ and SMH, and below 20 on NVDA, makes a sharp relief bounce possible. But the last two such bounces were sold at the open, so **wait for a close, not an opening gap**.

| Ticker | Signal | Entry zone | Confirmation | Stop | Targets | Notes |
|---|---|---|---|---|---|---|
| **MU** | HOLD / MONITOR (sector bellwether) | **$650–670** | A 4H bullish engulfing candle or hammer that holds $650 | $610 | T1 $795, T2 $860 | After-hours $680.55, so the zone may be tested Friday. From $660: +20% / +30% vs −7.6%, **R/R 2.7 / 4.0**. Earnings ~Dec 16 [Est.] |
| **MRVL** | HOLD / MONITOR | $133–138 (after-hours price is in the zone) | A daily higher low above $132.5 with RVOL > 1 | $124 | T1 $165, T2 $176 (20d) | Earnings **Dec 1 [Confirmed]**: half size at most. From $135.5: R/R 2.5 / 3.4. A close below $132.5 voids it |
| **RKLB** | HOLD / MONITOR | $49.50–51.00 (live) | A 4H reversal **and** a 1H close above the 1H 20-EMA (~$53.7 now, falling) | $45.80 | T1 $56.2 (20d), T2 $61.7 (50d) | MACD histogram turned negative. From $50.25: +12% / +23% vs −8.9%, R/R 1.3 / 2.6 |
| **OUST** | HOLD / MONITOR | $27.40–28.40 (live) | A 4H higher low above $27.35 plus a 1H close above the 20-EMA (~$29.9) | $25.60 | T1 $32.40, T2 $35.10 | A close below $27.35 breaks the triple bottom. From $27.9: R/R 1.9 / 3.1 |
| **CRWV** | HOLD / MONITOR (high risk) | $41.00–43.50 | A daily reversal candle with RVOL > 1.3 | $38.40 | T1 $52.6 (20d), T2 $60.8 | After-hours $44.28. Rate- and debt-sensitive. From $42.25: R/R 2.4 / 4.4 |
| **PL** | HOLD / MONITOR | $11.00–11.50 (after-hours price at the top of the zone) | Hold $11.0 plus a reversal candle | $10.30 | T1 $13.3 (20d), T2 $15.0 | MACD histogram just turned negative. From $11.25: R/R 2.2 / 3.9. Earnings ~Dec 3 [Est.] |
| **CRDO** | HOLD / MONITOR (was POTENTIAL BUY) | $111–116 | Hold $110.8 plus a 4H reversal | $103 | T1 $138.8 (20d), T2 $160 | Earnings **Dec 1** [Confirmed per the morning brief]. Downgraded because the morning's 4H MACD upturn reversed and closed at the low (opinion). From $113.5: R/R 2.4 / 4.4 |
| **BKSY** | **Downgraded to HOLD / MONITOR** (was POTENTIAL BUY) | **New zone $16.40–17.20** (the late-October base) | A daily reversal candle while holding $16.13, **or** a daily close back above $19.50 | $15.60 | T1 $19.50, T2 $21.60 | The morning setup was invalidated. From $16.8: +16% / +29% vs −7.1%, R/R 2.3 / 4.0. Anyone who bought in the zone this morning: the **$18.30 stop stays**; price is $0.49 above it |
| **RDW** | HOLD / MONITOR | $6.05–6.35 | A daily bullish engulfing candle or hammer, RVOL > 1.2 | $5.60 | T1 $7.84, T2 $9.24 | A close below $6.06 opens a path to $4.87. ATM dilution overhang |
| **KTOS** | HOLD / MONITOR → leaning AVOID | none until a reclaim of $32.0–32.5 | A 4H higher low, then a reclaim | $28.90 | T1 $36.7, T2 $40.8 | New 52-week low; no support below. A close below $28.90 = AVOID |
| **NBIS** | **AVOID** | — | Reclaim $100, then a close above $116 | — | — | Breakdown on volume. Next support $86.5–89.7 |
| **ASTS** | AVOID / HIGH RISK | — | A close above $28.47 (today's high) on volume, then a higher low | — | — | Dilution overhang (≈10.8M shares in a week). Watch for a SpaceX launch date for BlueBirds 14–16 [Est.] |
| **VELO** | AVOID | — | A close above $4.15, then a higher low | — | — | Closed at the low; the $3.16 52-week low is the line |

**Key events Fri Nov 20 (ET)**
- **08:25: Fed Governor Waller, welcoming remarks** ([TD calendar](https://economics.td.com/domains/economics.td.com/documents/reports/bottom-line/tables/2026-11-13/upcoming.htm)). Opinion: this is the highest-risk headline of the day. Waller has floated a 50 bp December hike **[Reported]**.
- **12:15: Fed Governor Cook on the US economy** (same TD calendar).
- **US data:** the TD calendar lists **no US releases** for Friday. A flash PMI date for Nov 20 is **unconfirmed**; I found only conflicting calendars.
- **Earnings:** none on the watchlist.
- **Anthropic (ANT) day 2:** a flow wildcard for AI names in either direction. **[Opinion]**
- **Watchlist dates ahead:**
  - **MRVL Dec 1 [Confirmed]** and **CRDO Dec 1** (after the close).
  - **PL ~Dec 3 [Est.]**.
  - **FOMC Dec 8–9**: a 25 bp hike is ~90% priced **[Reported]**.
  - **MU ~Dec 16 [Est.]**.
  - **OUST at the Northland conference, Dec 16**.

---

*Prices: Stock Analysis (OHLCV), Twelve Data (close cross-check, hourly bars, after-hours), Massive (daily history, news feed). News: Massive news feed, Yahoo Finance live blog, Motley Fool, Zacks, SatNews. Filings: SEC EDGAR. Facts, estimates and opinions are labelled. This is not personalised investment advice.*
