## 🌙 Post-Market Briefing: Wednesday, November 18, 2026

**Data notes (please read first)**
- **Retrieved:** 2026-11-18, about 21:35–22:20 UTC (23:35–00:20 Bucharest; 16:35–17:20 ET).
- **Today's prices.** Massive (Polygon) still refuses same-day data on this plan: `/v1/open-close` for today returned "NOT_AUTHORIZED … before end of day". Today's open/high/low/close and volume therefore come from the **Stock Analysis** daily history pages. Every close was cross-checked against the **Twelve Data** quote, and all matched within 5 cents (largest gaps: BKSY $20.65 vs $20.61, SPY $730.20 vs $730.33, MU $705.27 vs $705.00).
- **History:** daily candles through Nov 17 come from Massive (status DELAYED). % change is vs. the Nov 17 close, and "5D" is vs. the Nov 11 close.
- **Relative volume** = today's Stock Analysis volume ÷ the 20-day average from Massive. It was read within about an hour of the close and may be revised slightly.
- **After-hours:** these are Twelve Data extended quotes with their own ET timestamps. "No AH print" means the last trade was at 15:59 ET. After-hours was very quiet tonight: no name moved more than 0.3%.
- **Indicators** are computed by me from the candles and include today's close: SMA 20/50/100/200, RSI(14, Wilder), MACD(12,26,9), ATR(14).
- **Morning brief:** setups are checked against `reports/2026-11-18-market-intelligence.md` on branch `claude/pensive-clarke-1zvayf`. It is not on this branch. Its three extra candidates are **CRDO, KTOS and PL**.
- **Filings:** I checked the SEC EDGAR submissions API at about 21:45 UTC for every watchlist company and for NVDA, for filings dated Nov 17–18. The documents were read on EDGAR.
- **Labels:** **[Confirmed]** = SEC filing or company release. **[Reported]** = media. **[Est.]** = unconfirmed. **Opinion** = my analysis. This is not personalised financial advice.

---

### 🧭 The day in three lines
1. **Nvidia's beat was sold.** Last night's after-hours gap disappeared before the open, and the rest of the move faded during the session. **NVDA closed −2.9% at $150.96** on 1.44× volume, its 5th straight loss, with RSI at 21. AI names that had been +4–11% in last night's after-hours all closed red or flat: **MU −1.0%, MRVL −2.2%, CRWV −4.1%, NBIS +0.9%**. Media reasons given **[Reported]**:
   - uncertainty over leadership after Huang's exit;
   - a federal export-control probe involving the customer Megaspeed;
   - about $118B of financial guarantees;
   - the 10-Q coming "in the coming weeks" rather than with the results. EDGAR shows no NT 10-Q, so it is **not late**.
2. **SPY closed below its 200-day SMA:** $730.20 vs. $732.55. That is the **first close below it in my data window (since at least mid-2026)**. The intraday low of $726.80 undercut the morning's $727 "cut exposure" level, but the **close was above it**, so the rule did not fire. The index tape was mixed:
   - Dow −1.11%, S&P 500 −0.23%, Nasdaq +0.42%, Russell 2000 +0.46%.
   - 10-year yield 5.07%, VIX 24.56.
   - **The October FOMC minutes pointed to further hikes**, and a near-certain 25 bp December hike is priced in **[Reported]**.
3. **Morning setups: zone fills, few confirmations.**
   - **Zones filled with no extra condition required (3):** CRDO, PL, and MU's pullback leg.
   - **In the zone but confirmation failed or is missing (4):** RKLB, BKSY, OUST, CRWV. CRWV broke its higher-low pivot.
   - Nothing stopped out and no targets were hit.
   - **ASTS (−7.6%) and KTOS (−2.6%) made new 52-week lows.** ASTS filed a second share issuance in two days.

---

### 1. Session recap

| Ticker | Close | % chg | 5D | Open | High | Low | Rel. vol | After-hours (ET) | AH vs close |
|---|---|---|---|---|---|---|---|---|---|
| **SPY** | 730.20 | −0.31% | −3.9% | 733.37 | 735.06 | 726.80 | 1.00× | 730.74 @ 16:27 | +0.1% |
| **QQQ** | 659.51 | +0.39% | −4.5% | 661.03 | 662.80 | 653.05 | 0.82× | 659.41 @ 16:09 | 0.0% |
| **SMH** | 459.54 | −0.12% | −9.4% | 467.98 | 469.50 | 452.85 | 0.58× | 459.45 @ 16:11 | 0.0% |
| RKLB | 53.07 | −3.60% | −19.8% | 55.98 | 56.36 | 52.89 | 0.71× | 53.20 @ 16:19 | +0.3% |
| BKSY | 20.65 | −5.71% | −14.3% | 22.23 | 22.35 | 20.56 | 0.87× | no AH print | n/a |
| RDW | 6.82 | +0.59% | −18.8% | 6.97 | 7.20 | 6.73 | 0.80× | no AH print | n/a |
| ASTS | 25.49 | **−7.61%** | **−30.4%** | 28.10 | 28.10 | **25.16** | **1.29×** | no AH print | n/a |
| MRVL | 145.54 | −2.15% | −13.8% | 151.91 | 152.39 | 142.62 | 0.62× | 145.55 @ 16:34 | 0.0% |
| MU | 705.27 | −1.00% | −13.1% | 718.50 | 722.96 | 687.33 | 0.86× | 704.24 @ 16:33 | −0.1% |
| VELO | 3.48 | **+6.75%** | −29.0% | 3.34 | 3.54 | 3.18 | 1.21× | no AH print | n/a |
| NBIS | 106.96 | +0.87% | −30.9% | 109.83 | 110.22 | **100.80** | 0.91× | 107.00 @ 16:02 | 0.0% |
| CRWV | 47.83 | −4.13% | −21.3% | 51.07 | 51.07 | 46.21 | 0.86× | 47.99 @ 16:30 | +0.3% |
| OUST | 29.30 | −3.87% | −23.3% | 31.10 | 31.59 | 29.13 | 0.60× | no AH print | n/a |
| CRDO | 122.94 | −0.81% | −13.1% | 127.34 | 128.12 | 119.18 | 0.57× | no AH print | n/a |
| KTOS | 30.24 | −2.64% | −17.6% | 31.01 | 31.69 | **29.98** | 0.96× | no AH print | n/a |
| PL | 12.05 | −3.52% | −16.0% | 12.79 | 12.89 | 12.03 | 0.67× | no AH print | n/a |
| *NVDA (context)* | 150.96 | −2.89% | −13.1% | 159.19 | 159.70 | 150.40 | **1.44×** | 150.92 @ 16:33 | 0.0% |

- **Overnight gap vs. actual open (fact):**

  | Ticker | Last night's AH (per morning brief) | Today's open | Close |
  |---|---|---|---|
  | MU | $745.80 | $718.50 | $705.27 |
  | MRVL | $157.24 | $151.91 | $145.54 |
  | NBIS | $117.99 | $109.83 | $106.96 |
  | CRWV | $54.39 | $51.07 | $47.83 |
  | RKLB | $57.75 | $55.98 | $53.07 |

  **Every name closed below its open.** The morning's "do not chase the gap" call was correct.
- **Shape of the day (from the daily candles):** nearly every name opened near its high and closed in the lower part of its range. BKSY, OUST, PL, KTOS and NVDA all closed within a few cents of the day's low. The exceptions were VELO (+6.8%, a bounce off its 52-week low) and the small rebounds in NBIS and RDW.
- **Volume:** below average almost everywhere (0.57–0.91×). The exceptions were **ASTS (1.29×)**, **VELO (1.21×)** and NVDA (1.44×). Opinion: on most names this looks like a lack of buyers rather than capitulation.
- **Macro [Reported]:**
  - Index closes: Dow 50,198.17 (−1.11%), S&P 500 7,323.63 (−0.23%), Nasdaq 24,429.89 (+0.42%), Russell 2000 2,714.31 (+0.46%). 10-year yield 5.07% (−4 bp). VIX 24.56 (−3.5%) ([Yahoo Finance live blog](https://finance.yahoo.com/markets/live/stock-market-today-wednesday-november-18-dow-sp-500-nasdaq-nvidia-earnings-anthropic-ipo-143530588.html)).
  - The October FOMC minutes saw a "need for further rate hikes", with a few members favouring 50 bp ([Rallies.ai](https://rallies.ai/news/wall-street-ends-mixed-after-nvidia-earnings-and-fed-minutes-a6392108f1de9ae9)).
  - Gov. Waller said a December hike could be 50 bp if the Fed does not signal a January move (Yahoo).
  - Housing starts beat expectations ([Zacks](https://www.zacks.com/stock/news/3031915/housing-starts-increased-more-than-expected)).
  - Benzinga headlined a 19-month high in the dollar ([headline](https://www.tradingview.com/news/benzinga:cf58745d6094b:0-dow-drops-as-nvidia-slips-after-earnings-dollar-hits-19-month-high-stock-market-today/)). I did not verify the level.

---

### 2. Morning setups: what happened

| Ticker | Morning plan | Result | Detail |
|---|---|---|---|
| **CRDO** | Buy $112–122 holding $110.8. Stop $104. T1 $148, T2 $170 | ✅ **TRIGGERED (zone filled)** | Low $119.18, close $122.94, $110.8 held. Mid-zone fill (~$120) is +2.4%. Light volume (0.57×). Earnings 12/1 [Est.], so size down. |
| **PL** | Buy $11.2–12.2 holding $11.0. Stop $10.4. T1 $14.9, T2 $17.2 | ✅ **TRIGGERED (zone top filled)** | Low $12.03, close $12.05. Only the top of the zone traded, and it **closed at the day's low** (opinion: weak candle). $11.0 intact. |
| **MU** | (a) Pullback $670–700 holding $650, stop: close below $626; or (b) close above $770 on ≥1.3× volume | ⚠️ **(a) TRIGGERED on the plan's terms; (b) not triggered** | Low $687.33 (in the zone), close $705.27; $650 held. **But** the morning signal was HOLD/MONITOR, the candle is red after a gap fade, and from $705 the R/R to T1 is poor (see section 5). |
| **RKLB** | Entry $50.5–53.5. Confirmation: a 4h higher low **and** a daily close above $56.3. Stop $47.8 | ⏸ **NOT TRIGGERED: in the zone, no confirmation** | Low $52.89, close $53.07, both in the zone. The close is below the 20-day SMA ($56.26). Stop not hit. |
| **BKSY** | Entry $20.2–21.0. Confirmation: a daily hold above $20 on lighter volume **plus** a 4h bullish reversal candle. Stop $18.4 | ⏸ **NOT TRIGGERED: in the zone, partial confirmation** | Low $20.56, close $20.65, both in the zone. It held $20 on 0.87× volume (✓), but **closed at the low with no reversal (✗)**. Stop not hit. |
| **OUST** | Entry $28.3–30.0. Confirmation: a daily bullish reversal above the triple bottom. Stop $26.4 | ⏸ **NOT TRIGGERED: in the zone, no confirmation** | Low $29.13, close $29.30, near the low. The daily MACD histogram flipped negative (−0.16 from +0.10). The triple bottom ($27.35–28.16) is intact. |
| **CRWV** | Entry $47–50.5. Confirmation: **the 4h higher low ($46.84–47.06) holds**, then a close above $53.8. Stop $44 | ❌ **CONFIRMATION FAILED, setup weakened** | Low **$46.21 undercut the higher-low pivot**, close $47.83 in the zone. Stop $44 not hit. Opinion: the higher-low thesis is broken; see section 5. |
| **MRVL** | Buy $135–142 holding $132.5. Stop $128 | ⏸ **NOT REACHED** | Low $142.62, 62 cents above the zone. Close $145.54. |
| **KTOS** | Trigger: a daily close above $35, then buy the $33–35 retest. Stop $30.2 | ⏸ **NOT TRIGGERED** | Close $30.24. **New 52-week low $29.98**, below the plan's $30.2 stop level (no position existed). |
| **ASTS** | AVOID. Base needs a close above $32.6 | 🛑 **AVOID stands** | **New 52-week low $25.16**, close $25.49 on 1.29× volume. A second issuance filing (section 3). |
| **RDW** | AVOID. A close below $6.06 opens a new leg down | 🛑 **AVOID stands** | Low $6.73, close $6.82. $6.06 not tested. |
| **VELO** | AVOID | 🛑 **AVOID stands** | A +6.8% bounce from $3.18 (above yesterday's $3.16 low). One day does not make a base. |
| **NBIS** | AVOID. Re-assess after a close above $130 | 🛑 **AVOID stands** | Opened $109.83, nowhere near $113–118. Low $100.80 is a new 20-day low; closed $106.96. |

**Summary:**
- Triggered: **2** (CRDO, PL), plus MU's pullback leg on the plan's terms.
- In the zone without confirmation: **3** (RKLB, BKSY, OUST).
- Confirmation failed: **1** (CRWV).
- Not reached: **2** (MRVL, KTOS).
- Stopped out: **0**. Targets hit: **0**.

**Morning market rules:**
- SPY close above $740 (add risk): **no**.
- SPY close below $727 (cut exposure): **no** on a closing basis ($730.20), but the intraday low was $726.80, **and SPY closed below its 200-day SMA**.

---

### 3. Earnings, filings and material news (Nov 18, incl. after-hours)

**Watchlist filings on EDGAR (Nov 17–18)**
- **ASTS: 424B5, Nov 18 [Confirmed]** ([filing](https://www.sec.gov/Archives/edgar/data/1780312/000149315226053004/form424b5.htm)):
  - A registered direct issue of **780,052 Class A shares to Ligado Networks and One Dot Six**.
  - ASTS receives **no cash proceeds**. The shares are issued under the Ligado agreements and were to be delivered on or about Nov 18.
- **ASTS: 8-K, Nov 17 after the close [Confirmed]** ([filing](https://www.sec.gov/Archives/edgar/data/1780312/000149315226052865/form8-k.htm)):
  - It covers the **10,000,000 shares issued to Firefly Aerospace** under the Nov 6 IP license agreement (prospectus supplement under S-3 No. 333-281939). Yesterday's post-market brief flagged this.
  - Together, the two filings add **~10.8M new shares in two days**. Opinion: that is a supply overhang on a stock already at 52-week lows.
- **RKLB: Form 4, filed Nov 18 [Confirmed]** ([filing](https://www.sec.gov/Archives/edgar/data/1819994/000200101126000147/xslF345X06/edgardoc.xml)). VP A. Ricupati received a **grant of 5,373 RSUs**; there was no open-market sale. Not material.
- **VELO: Form 4, filed Nov 18 [Confirmed]** ([filing](https://www.sec.gov/Archives/edgar/data/1825079/000119312526466758/xslF345X06/ownership.xml)). CEO/director A. Jeldi had **3,145 RSUs vest** on 11/15. The reporting person's affiliate Arrayed holds 12.74M shares indirectly. There was no sale. Not material.
- **RDW (Form 4, 11/17), MRVL (two Form 4s, 11/17), NBIS (Form 4, 11/17):** these were filed before this morning's brief. They are routine insider forms and I found nothing material in them on a scan.
- **MU, BKSY, CRWV, OUST, CRDO, KTOS, PL:** no filings dated Nov 17–18.
- **NVDA:** the only recent filing is the 8-K results release (11/17). There is **no NT 10-Q**. Media say the 10-Q is due "in the coming weeks" and is not late **[Reported]** ([Motley Fool](https://www.fool.com/investing/2026/11/18/nvidia-just-demolished-earnings-but-the-stock-is-still-plunging-the-reason-is-obvious/)).

**News by ticker**
- **RKLB, BKSY, RDW, MRVL, MU, VELO, NBIS, CRWV, OUST, CRDO, KTOS, PL:** **No material news.** The Massive news feed for Nov 17 21:00 UTC onwards held only commentary and opinion pieces (Motley Fool, Zacks): Redwire Paragon MOU and Kratos offshore-launch "can X" explainers, and CoreWeave/Nebius "buy the dip" pieces. None was a company release.
- **ASTS:** only the filings above. Media coverage was commentary only.
- **Sector driver, NVDA [Reported]:** the stock fell despite the beat. The Motley Fool cites four reasons:
  - Leadership: the board "does not intend to reinstate Jensen as CEO".
  - A federal probe into possible export-control breaches involving the customer Megaspeed.
  - About $118B of financial guarantees, including credit support for a data-center campus.
  - The timing of the 10-Q.
  I did not independently verify these beyond that source.
- **Market event, Anthropic IPO [Reported, single source]:** Yahoo, citing Bloomberg, reports the IPO **priced at $83**, above the $70–78 range, with a larger deal size, and that **ANT starts trading on Nasdaq Thursday**. The $70–78 range and Thursday listing are corroborated elsewhere ([TNW](https://thenextweb.com/news/anthropic-ipo-terms-1-4-trillion-valuation)); the $83 price is not yet. Opinion: a deal of up to roughly $60B+ can pull money out of other AI names in the short term.
- **Earnings after the close:** none on the watchlist.

---

### 4. Technical update (daily, includes today's close)

| Ticker | Close | SMA20 | SMA50 | SMA100 | SMA200 | RSI(14) | MACD hist (prev) | ATR % | Position / change |
|---|---|---|---|---|---|---|---|---|---|
| SPY | 730.20 | 753.72 | 762.51 | 760.27 | **732.55** | 36.6 | −2.15 (−1.60) | 1.5% | **Below all four; first close under the 200d** |
| QQQ | 659.51 | 686.30 | 714.36 | 712.76 | 682.81 | 37.7 | −1.48 (−1.46) | 2.4% | Below all; 8 closes under the 200d |
| SMH | 459.54 | 504.64 | 553.13 | 562.59 | 524.75 | 35.2 | −2.38 (−2.38) | 5.1% | Below all; held $445.3 (11/17 low) |
| RKLB | 53.07 | 56.26 | 61.91 | 67.88 | 77.93 | 43.1 | +0.35 (+0.79) | 9.0% | Lost the 20d; histogram fading |
| BKSY | 20.65 | 20.17 | 20.59 | 22.86 | 27.00 | 49.2 | +0.29 (+0.52) | 8.0% | **Sitting on the 20d/50d**; above both by cents |
| RDW | 6.82 | 7.92 | 9.32 | 10.04 | 10.81 | 37.2 | −0.03 (−0.01) | 9.9% | Below all |
| ASTS | 25.49 | 35.70 | 47.52 | 56.83 | 72.37 | **29.7** | −0.35 (−0.15) | 15.2% | **Breakdown on volume**; 29% below the 20d |
| MRVL | 145.54 | 180.61 | 224.32 | 221.65 | 188.03 | 33.3 | −1.00 (−1.50) | 10.9% | Below all; histogram improving; mid-range $132.5–174.5 |
| MU | 705.27 | 809.10 | 925.62 | 929.45 | **769.93** | 37.0 | −3.69 (−3.50) | 8.2% | Below all; 200d now $770 |
| VELO | 3.48 | 5.54 | 7.93 | 10.25 | 12.71 | 28.0 | −0.13 (−0.13) | 19.2% | Oversold bounce; below all |
| NBIS | 106.96 | 141.47 | 186.79 | 199.76 | 179.64 | 34.1 | −1.87 (−1.96) | 15.7% | Below all; new 20d low $100.80 |
| CRWV | 47.83 | 53.12 | 69.87 | 77.77 | 88.36 | 38.8 | +0.80 (+0.99) | 12.8% | Below all; **lost its higher-low pivot** |
| OUST | 29.30 | 32.39 | 35.22 | 38.01 | 33.02 | 41.1 | **−0.16 (+0.10)** | 10.2% | Below all; **MACD histogram turned negative** |
| CRDO | 122.94 | 141.09 | 169.51 | 198.38 | 180.92 | 38.5 | −0.05 (−0.20) | 11.9% | Below all; histogram nearly flat |
| KTOS | 30.24 | 37.15 | 41.12 | 46.73 | 59.06 | **29.0** | −0.57 (−0.50) | 7.5% | **New 52-week low**; below all |
| PL | 12.05 | 13.39 | 15.07 | 19.08 | 25.87 | 37.4 | +0.03 (+0.10) | 8.0% | Below all; histogram almost negative |
| NVDA | 150.96 | 189.04 | 210.30 | 211.05 | 203.72 | **21.1** | −3.82 (−4.00) | 6.4% | Deeply oversold; 52-week low $148.80 nearby |

**Breakouts and breakdowns on volume**
- **ASTS:** breakdown to a new 52-week low on 1.29× volume. It is the only clear volume breakdown on the list today.
- **KTOS:** new 52-week low on average volume (0.96×).
- **SPY:** closed below its 200-day SMA on average volume (1.00×). Opinion: a single close is not yet a confirmed break. Two closes below it, or a close below $726.8, would confirm.
- **No breakouts.** No name closed above its 20-day SMA after being below it this morning.

**Levels that changed**
- **ASTS:** new support reference is $25.16 (52-week low). Resistance is $28.1 (today's open/high), then $29.2.
- **KTOS:** new low at $29.98. The $30.2 level is gone; resistance is $31.7, then $35.
- **NBIS:** $100.80 is the new near-term support. Resistance is $110.2, then $113.3.
- **CRWV:** $46.21 replaces $46.84 as the near-term low. Resistance is $51.1 (today's open/high), then $53.1 (20-day).
- **RKLB:** $52.89 is the new short-term low. The 20-day ($56.26) is now resistance.
- **MU:** the 200-day dropped to ~$770. Today's low ($687.33) is the first support above $666.88 / $650.
- **SPY:** the 200-day ($732.55) flips to first resistance. Support is $726.80–727.00 (the 11/17–11/18 lows).

---

### 5. Plan for tomorrow (Thu Nov 19)

**General stance (opinion):** **Defensive. Wait.**
- The market just ignored a strong Nvidia beat, SPY is under its 200-day, and the Fed is guiding to hikes. Under those conditions, buy only inside zones, at **half size**.
- **Add risk only if SPY reclaims $735 (today's high) and holds above its 200-day.**
- **Cut exposure on a SPY close below $726.8.**
- Anthropic's debut (if it trades Thursday) is a liquidity and sentiment wildcard for AI names in both directions.

| Ticker | Signal | Entry zone | Confirmation | Stop | Targets | Notes |
|---|---|---|---|---|---|---|
| **BKSY** | WAIT FOR CONFIRMATION | $20.2–21.0 (live) | Daily close back above $21.4, or a 4h bullish reversal while holding $20 | $18.4 | T1 $24.9, T2 $27.0 | Strongest relative strength; on the 20/50d. **A close below $20 cancels it; then wait for $18.4–19.** R/R from $20.6: 2.0 / 2.9 |
| **CRDO** | POTENTIAL BUY (triggered) | $112–122 | Hold $110.8 | $104 | T1 $148, T2 $170 | Earnings 12/1 [Est.]: half size, trim before the print. R/R from $120: 1.8 / 3.1 (lower than the morning's 2.4 because the fill was at the top of the zone) |
| **PL** | POTENTIAL BUY (triggered) | $11.2–12.2 | Hold $11.0; add on a close above $12.9 | $10.4 | T1 $14.9, T2 $17.2 | Closed at the low; expect a test of $11.0–11.5 first (opinion) |
| **OUST** | POTENTIAL BUY (on reversal only) | $28.3–30.0 | A reversal candle above $28.2, or a reclaim of $32.4 (20d) | $26.4 | T1 $33.5, T2 $39.5 | MACD histogram turned negative. A close below $27.35 breaks the triple bottom |
| **RKLB** | POTENTIAL BUY (on confirmation) | $50.5–53.5 | A 4h higher low, then a close above $56.3 | $47.8 | T1 $61.5, T2 $68 | A break of $52.89 likely tests $49.3–50.7 (opinion) |
| **MU** | HOLD / MONITOR | Prefer **$670–690** to a fill at $705 | A reversal candle; hold $650 | Daily close below $626 | T1 $768, T2 $827 | From $705: −11% vs. +9%, so **R/R < 1. Don't chase.** Breakout trigger: close above $770 on ≥1.3× volume |
| **CRWV** | **Downgraded to HOLD / MONITOR** (was POTENTIAL BUY) | $44.5–47 | Hold $46.2, **and** a close above $51.1 | $44.0 (existing) | T1 $53.1, T2 $62 | The higher-low pivot failed; there is a debt overhang. A close below $44 invalidates it. |
| **MRVL** | HOLD / MONITOR | $135–142 | Hold $132.5 plus a 4h reversal | $128 | T1 $174, T2 $187 | Earnings ~11/26–12/1 [Est., verify on IR] |
| **KTOS** | HOLD / MONITOR → leaning AVOID | none until a close above $35 | Close above $35, then a retest at $33–35 | $30.2 → **re-set to $29.5** once triggered | T1 $41.5, T2 $44 | New low; no base |
| **NBIS** | AVOID | — | Close above $113.3, then above $130 | — | — | $100.80 is the next support |
| **ASTS** | AVOID / HIGH RISK | — | Close above $29.2, then a 4h higher low | — | — | Dilution (≈10.8M shares in 2 days) plus a volume breakdown |
| **RDW** | AVOID | — | Reclaim $7.9–8.0 | — | — | $6.06 is the line |
| **VELO** | AVOID | — | — | — | — | Bounce at RSI 28; no base. Dilution risk (2028 cash-flow target) |

**Key events Thu Nov 19 (ET)**
- **08:30: Initial and continuing jobless claims** ([Financecalendar](https://www.financecalendar.com/events/2026-11-19/)). Also the **Philadelphia Fed manufacturing index**, plus the Kansas City Fed index and October Leading Index at 10:00 or later **[Est., from a secondary calendar]**.
- **Fed speakers [Est., times not time-zone-verified]:** Hammack (opening remarks), Goolsbee (Economic Club of Indiana), Barr (AI-related appearance), Barkin (fireside chat) ([Newsquawk weekly](https://www.newsquawk.com/headlines/newsquawk-weekly-economic-release-16th---20th-november-2026), TD calendar). Opinion: after the hawkish minutes, any comment endorsing a 50 bp December hike is a downside risk for high-beta names.
- **Anthropic (ANT) Nasdaq debut [Reported]:** expected Thursday.
- **Earnings:** none on the watchlist. Walmart is listed for 11/19 by one calendar, but the date is **unconfirmed**.
- **Watchlist dates still ahead:**
  - MRVL FQ3 ~11/26 or 12/1 [Est.]
  - CRDO 12/1 [Est.]
  - PL early December (12/3, 12/8 or 12/10 cited) [Est.]
  - MU ~12/16 [Est.]

---

*Prices: Stock Analysis (OHLCV), Twelve Data (closes, after-hours), Massive (history). News: Massive news feed, Yahoo Finance, Motley Fool, Zacks, Rallies.ai. Filings: SEC EDGAR. Facts, estimates and opinions are labelled. This is not personalised investment advice.*
