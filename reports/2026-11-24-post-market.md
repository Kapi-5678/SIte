## 🌙 Post-Market Briefing: Tuesday, November 24, 2026

**Prepared:** ~23:45 EET (21:45 UTC), after the US close. The morning plan being graded is [reports/2026-11-24-market-intelligence.md](https://github.com/kapi-5678/site/blob/claude/pensive-clarke-is2uat/reports/2026-11-24-market-intelligence.md), which sits on branch `claude/pensive-clarke-is2uat`.

**Price data:**
- **Today's OHLC, 1h bars and after-hours (AH) prices** come from Twelve Data. Quotes were retrieved 21:33–21:45 UTC. Massive (Polygon) returned `NOT_AUTHORIZED` for today's `/v1/open-close` and minute bars; its plan has no same-day data.
- **History through Mon Nov 23** comes from Massive daily candles.
- SMA 20/50/100/200, RSI(14, Wilder), MACD(12,26,9) and ATR(14) are computed in-house on that history plus today's close. Session VWAP is approximated from the 1h bars.

**Data gaps:**
- **Relative volume** is shown only where the feed's volume looks consolidated.
  - Twelve Data volume is plainly partial for QQQ (1.1M), SMH (0.5M), RKLB (0.66M) and VELO (0.06M). Those are marked n/a.
  - SPY's 223M (3.6× its average) is implausible on a −0.5% day, so it is also marked n/a.
- **AH timestamps:** where the AH timestamp is 15:59, no after-hours trade reached the feed.

**Labels:** **[FACT]** = sourced or computed from data · **[EST]** = estimate or unconfirmed · **[VIEW]** = my analysis or opinion. Not personalised financial advice.

---

### 🧭 What happened today

- **[FACT]** Monday's chip rally was **half-reversed**, but the broad market held.
  - S&P 500: −0.50% to ~7,201.
  - Nasdaq Composite: −1.48% to ~23,734.
  - Dow: +0.85% to ~50,019.
  - 10-year yield ~4.90%; VIX ~26.4.
  - Source: [Yahoo Finance live](https://finance.yahoo.com/markets/live/stock-market-today-tuesday-november-24-dow-sp-500-nasdaq-chip-stocks-nvidia-140629923.html). The page notes these may not be final prints.
- **[FACT]** NVDA fell about 6% after Monday's +31%. **MU −11.0%**, AMD −8.9%, AVGO −4.0%, and HPE −16.3% after its earnings ([StockTitan](https://www.stocktitan.net/articles/stock-market-today-live-november-24-2026)). Memory names (MU, SK Hynix, SanDisk, WDC, STX) were hit hardest.
- **[FACT] Neocloud financing scare.** On HPE's Q4 call, CEO Antonio Neri said HPE "has not provided financing to neocloud or high-risk customers." CoreWeave fell about 12–13% and Nebius about 11% ([Yahoo Finance](https://finance.yahoo.com/markets/stocks/articles/spacex-falls-4-coreweave-down-185758049.html)).
- **[FACT] Rates.** Traders price about a 95% chance of a 25 bp **hike** on Dec 9, with ~5% odds of 50 bp (Yahoo live page above).
- **[FACT] After the bell, Dell posted a blowout quarter:**
  - Revenue **$54.9B (+103% y/y)** against ~$49.3B expected. Adjusted EPS **$9.45** against $6.59.
  - AI server revenue $22.0B (+291%). AI orders $60.2B; **AI backlog a record $132.3B**.
  - FY27 revenue guidance raised to $202B (from $192B). Q4 guidance of $56.3B vs. ~$53.5B expected. A new $25B buyback.
  - Shares rose about 4% after hours.
  - Sources: [Proactive Investors](https://www.proactiveinvestors.com/companies/news/1102383/dell-shares-rise-after-earnings-beat-as-ai-server-backlog-jumps-619-1102383.html), [mlq.ai](https://mlq.ai/news/dells-revenue-doubles-to-549-billion-as-its-ai-backlog-hits-a-record-1323-billion-full-year-outlook-raised-to-202-billion/), [TipRanks](https://www.tipranks.com/news/dell-stock-rises-after-q3-eps-blows-past-estimates).
- **[VIEW]** Today is the textbook follow-through of a bear-market rally, **not** a new leg down:
  - SPY held Monday's range: low $712.14, close $718.79, and closed at 76% of its daily range.
  - The damage was concentrated in semis and AI-infrastructure names that rallied 15–30% on Monday.
  - The watchlist's AH reaction to Dell was muted: every name moved less than ±0.6% except ASTS (+1.6%).
  - The SMH and QQQ trend structure is unchanged: below every major moving average.

---

### 1️⃣ Session recap

| Ticker | Close | % chg | Open | High | Low | Close in range | ~VWAP | AH price (time ET) | RVOL |
|---|---|---|---|---|---|---|---|---|---|
| **SPY** | 718.79 | −0.48% | 715.14 | 720.93 | 712.14 | 76% | 716.6 | 718.18 (16:26) | n/a |
| **QQQ** | 638.12 | −1.98% | 640.02 | 648.00 | 631.23 | 41% | n/a | 637.60 (16:30) | n/a |
| **SMH** | 427.33 | **−7.14%** | 440.85 | 442.88 | 418.41 | 36% | n/a | 426.91 (16:27) | n/a |
| RKLB | 45.98 | −7.35% | 48.32 | 48.75 | 44.57 | 34% | 45.9 | 46.24 (16:29) | n/a |
| BKSY | 16.43 | −6.68% | 17.62 | 17.86 | 16.40 | **2%** | 16.94 | no AH print | 1.22 |
| RDW | 5.89 | −8.18% | 6.28 | 6.29 | 5.78 | 23% | 5.98 | no AH print | 0.68 |
| ASTS | 23.58 | −8.14% | 25.18 | 25.18 | **22.52** | 40% | 23.47 | 23.96 (16:01) | 0.74 |
| MRVL | 131.58 | −9.09% | 139.70 | 140.75 | 128.14 | 27% | 132.3 | 131.22 (16:14) | 0.70 |
| **MU** | **629.79** | **−11.01%** | 669.39 | 672.07 | 622.22 | 15% | 635.8 | 627.16 (16:31) | 1.01 |
| VELO | 3.01 | −10.68% | 3.25 | 3.34 | 2.98 | 7% | 3.10 | no AH print | n/a |
| NBIS | 87.30 | −10.74% | 94.62 | 95.28 | 84.30 | 27% | 87.3 | 86.90 (16:30) | 1.39 |
| CRWV | 42.60 | −11.86% | 46.69 | 47.04 | 41.22 | 24% | 43.0 | 42.60 (16:32) | 0.82 |
| OUST | 24.98 | −10.45% | 26.86 | 26.96 | 24.49 | 20% | 25.12 | no AH print | 0.79 |
| CRDO | 106.46 | **−13.07%** | 116.83 | 118.02 | 105.66 | 6% | 108.7 | no AH print | 0.76 |
| **KTOS** | 28.20 | **−1.05%** | 28.36 | 28.95 | 27.65 | 42% | 28.3 | 28.01 (16:04) | 0.60 |
| PL | 10.64 | −5.08% | 11.01 | 11.18 | 10.62 | 4% | 10.81 | no AH print | 0.96 |

**Notes:**
- All values are [FACT] from Twelve Data.
- Percent changes are measured against the Massive/Twelve Data Monday closes, which differ by a few cents from the Twelve Data quotes used in last night's post-market report.
- RVOL figures use feed volume against the 20-day Massive average and are **unverified**.
- **[VIEW]** Most names fell on below-average volume (RVOL ~0.6–0.8), which looks more like profit-taking than panic. NBIS (1.39×) and BKSY (1.22×) are the exceptions: sellers were heavier there.
- **KTOS** showed the best relative strength on the list (−1% on a −7% SMH day).

---

### 2️⃣ Morning setups: scorecard (from today's 08:05 UTC brief)

| Ticker | Morning plan | What happened (1h bars) | Status |
|---|---|---|---|
| **MU** | Entry $660–680 on a pullback that **holds $666** with a 4h higher low. Stop $625. T1 $775. | Opened $669.39 inside the zone, but the first hour broke $666 and fell to $629.45. The low was **$622.22, below the $625 stop**. Closed $629.79, **below the $650 shelf**. The confirmation never happened. | **INVALIDATED.** Confirmation failed, the stop level traded, and the "failed breakdown above $650" thesis from last night is void. |
| **CRWV** | Entry $45–47 retest. Confirmation: 4h higher low above $44.4. Stop $42.80. | Opened $46.69 in the zone, broke $44.4 in the first hour, low $41.22. Closed $42.60, below the stop. | **INVALIDATED.** The stop level traded. The 52-week low at $39.28 still holds. |
| **RKLB** | Entry $44–46 on a retest of $43.9–45.1. Confirmation: 4h reversal with a higher low, then a reclaim of 1h VWAP. Stop $41.80. | **The zone was reached** (low $44.57, at 10:30). Price made higher hourly lows and rose to $47.13 by 13:30, above VWAP, then faded to close $45.98, right at VWAP. The afternoon 4h candle closed red. | **NOT TRIGGERED.** The zone was tagged but there was no clean 4h reversal candle. The stop was not hit and the setup is alive. |
| **BKSY** | Entry $16.1–16.8. Confirmation: a close above $16.09, then a 4h higher low. Stop $15.20. | **The zone was reached** (low $16.40). The close of $16.43 is above $16.09 but at **2% of range**, on 1.22× volume. No higher low formed. | **NOT TRIGGERED.** Alive, but deteriorating. |
| **OUST** | Entry $24.5–25.5 on a retest that holds $23.6. Stop $22.90. | **The zone was reached** (low $24.49). Price held a tight $24.5–25.3 range all day and closed $24.98, just under VWAP ($25.12). | **NOT TRIGGERED.** The zone was tagged and $23.6 held, but no reversal candle formed. Still valid. |
| **MRVL** | Hold into Dec 1 earnings. Optional zone $138–142, stop $128. | Opened $139.70 in the zone, then broke $138 support. The low of **$128.14 was 14 cents above the stop**. Closed $131.58. | **NOT TRIGGERED** (stand-aside rule). $138 support broke, so the optional zone is **invalidated**. |
| **NBIS** | No trade. | Fell 10.7%; lost Monday's low of $95.80. | **N/A.** Avoid stance confirmed. |
| **RDW** | Avoid. Reconsider only above $7.65. | Lost the reclaimed $6.06 pivot; closed $5.89. | **N/A.** The re-evaluation condition from last night is reversed. |
| **ASTS** | Hold/monitor. Base needed above $22.7. | Made a **new 52-week low at $22.52**, then bounced to close $23.58. AH $23.96. | **N/A.** The base condition is **broken** (undercut $22.72). |
| **VELO** | Avoid. | Fell 10.7% to $3.01, near the $2.85 52-week low. | **N/A** |
| **CRDO** | Entry $112–118. Stop $104. Earnings Dec 1. | **The zone was reached** from the open, but price fell through it. Closed **$106.46**, below the zone and at 6% of range. The stop was not hit (low $105.66). | **NOT TRIGGERED** (no hold). At risk: the close is $2.46 above the stop. |
| **KTOS** | Entry $26.6–28.0, but only with a 4h/1h higher low **and a reclaim of $29.75**. Stop $25.40. | **The zone was reached** (low $27.65). A 1h higher low formed ($28.12 → $28.45). The high of $28.95 **did not reclaim $29.75**. | **NOT TRIGGERED.** The best-behaved setup today. |
| **PL** | Entry $10.4–11.0 on a hold of $10.35. Stop $9.70. | **The zone was reached** (low $10.62), and $10.35 held. Closed at the low of the day. | **NOT TRIGGERED.** Valid, but momentum is weak. |

**Last night's post-market plan (the more conservative levels):**
- **MU:** the $612 stop was not hit, but the "only on a retest that holds $650" condition **failed**, so there was no entry.
- **OUST:** the $27.00–27.50 retest failed; price opened below it.
- **RKLB:** the $46.90–48.30 zone traded at the open; the $43.40 stop was not hit.
- **BKSY:** the invalidation level of $16.09 held.

**[FACT] Summary:**
- **Invalidated:** MU and CRWV (their stop levels traded) and the optional MRVL zone ($138 support broke).
- **Zones tagged but not triggered:** RKLB, BKSY, OUST, CRDO, KTOS, PL. **No confirmations fired.**
- **Targets reached:** none.

---

### 3️⃣ Earnings, filings and news (today, including after-hours)

**SEC filings** (from EDGAR submissions, filed Nov 23 evening to Nov 24):
- **ASTS:** **Form 4** filed today at 16:01 ET. Director **Adriana Cisneros made open-market purchases** on Nov 20 ([SEC](https://www.sec.gov/Archives/edgar/data/1780312/000110465926131559/xslF345X06/tm2630590-1_4seq1.xml)):
  - 21,250 shares directly at $23.54.
  - 21,250 shares through an entity at $23.54.
  - 1,064 shares through her spouse at $23.45.
  - Total: about **43.6K shares, ~$1.0M**.
  - **[VIEW]** A meaningful director buy at the lows, the second insider buy in the space group after Redwire's CEO bought on Nov 20. It may explain the +1.6% AH tick.
- **BKSY:**
  - **S-8** filed today at 16:06 ET, registering **565,000 shares** for the 2026 Inducement Equity Incentive Plan adopted Oct 29 ([SEC](https://www.sec.gov/Archives/edgar/data/1753539/000175353926000170/blacksky-sx82026ieip.htm)). **[VIEW]** Routine; immaterial dilution.
  - Three **Form 4s** filed Monday evening confirm 10b5-1 sales on Nov 20 at ~$16.56–18.29:
    - CEO O'Toole: 20,000 shares ([SEC](https://www.sec.gov/Archives/edgar/data/1753539/000175353926000167/xslF345X06/wk-form4_1795477158.xml)).
    - CFO Dubois: 4,000 shares ([SEC](https://www.sec.gov/Archives/edgar/data/1753539/000175353926000166/xslF345X06/wk-form4_1795477120.xml)).
    - General Counsel Lin: 6,000 shares ([SEC](https://www.sec.gov/Archives/edgar/data/1753539/000175353926000168/xslF345X06/wk-form4_1795477191.xml)).
  - **[VIEW]** Planned sales; low signal.
- **RKLB:** **Five Form 144s** filed Nov 23 (dated as of the 23rd) for restricted-stock-vesting tax sales through Morgan Stanley.
  - Example: CFO Adam Spice, 9,401 shares (~$473K) ([SEC](https://www.sec.gov/Archives/edgar/data/1819994/000200101126000148/xsl144X01/primary_doc.xml)). Another: 626 shares (~$31K) ([SEC](https://www.sec.gov/Archives/edgar/data/1819994/000200101126000152/xsl144X01/primary_doc.xml)).
  - **[FACT]** This **confirms the Nov 23 Form 144 notice** the morning brief could not verify.
  - **[VIEW]** Routine tax-withholding supply; low materiality.
- **MU:** **DEF 14A** proxy, DEFA14A and annual report filed today at ~16:22 ET ([SEC proxy](https://www.sec.gov/Archives/edgar/data/723125/000072312526000034/mu-20261124.htm)). **[VIEW]** Routine annual-meeting paperwork; I have not reviewed its contents for anything unusual.
- **CRDO:** Form 4 filed Monday evening. Chief Legal Officer James Laufman had 7,379 shares withheld for tax at $122.94 on Nov 19 (code F) ([SEC](https://www.sec.gov/Archives/edgar/data/1807794/000162828026075508/xslF345X06/wk-form4_1795468994.xml)). **[VIEW]** Not a discretionary sale.
- **RKLB, MRVL, VELO, NBIS, CRWV, OUST, KTOS, PL:** no 8-K, S-3 or ATM filings found today. NBIS and CRWV file mostly 6-K/8-K; none are dated today in EDGAR.

**Company and sector news:**
- **MU:** No company-specific news. It fell with the memory group as the Monday rally reversed and rate-hike fears returned ([Yahoo](https://finance.yahoo.com/markets/stocks/articles/micron-sinks-7-chip-stocks-145159283.html), [Motley Fool](https://www.fool.com/investing/2026/11/24/why-micron-stock-dove-today/)). **[VIEW]** Dell's $132B AI backlog after the bell is a positive demand read-through for memory.
- **CRWV and NBIS:** the HPE CEO comment on not financing neoclouds drove the sector-wide decline, with no company-specific news ([Yahoo](https://finance.yahoo.com/markets/stocks/articles/spacex-falls-4-coreweave-down-185758049.html)). **[VIEW]** Financing is the core bear case for both. The comment hits the thesis directly, and Dell's beat does not cure it.
- **MRVL and CRDO:** No material news; both fell with semis. Both report **Tue Dec 1 after the close**.
- **RKLB, BKSY, RDW, OUST, KTOS, PL, VELO:** No material news beyond the filings above.
- **Earnings today:** none on the watchlist.
  - After hours, sector-relevant: **Dell beat** (details above).
  - HP, Workday, Autodesk and Ambarella also reported after the close ([StockTitan](https://www.stocktitan.net/articles/stock-market-today-live-november-24-2026)). I did not review those results.

---

### 4️⃣ Technical update (daily close vs. moving averages)

| Ticker | Close | SMA20 | SMA50 | SMA100 | SMA200 | RSI14 (Mon→Today) | MACD hist (Mon→Today) | ATR % |
|---|---|---|---|---|---|---|---|---|
| SPY | 718.79 | 743.11 (−3.3%) | 758.64 (−5.3%) | 758.85 (−5.3%) | 733.04 (−1.9%) | 41.5→40.5 | −4.29→−3.53 | 2.1% |
| QQQ | 638.12 | 671.32 (−4.9%) | 708.47 (−9.9%) | 709.22 (−10.0%) | 683.39 (−6.6%) | 42.2→39.5 | −3.25→−2.81 | 3.3% |
| SMH | 427.33 | 483.88 (−11.7%) | 543.59 (−21.4%) | 555.22 (−23.0%) | 525.57 (−18.7%) | 42.5→37.6 | −3.20→−3.30 | 7.0% |
| RKLB | 45.98 | 55.06 (−16.5%) | 60.73 (−24.3%) | 65.85 (−30.2%) | 77.45 (−40.6%) | 41.7→38.3 | −0.73→−0.95 | 11.1% |
| BKSY | 16.43 | 20.06 (−18.1%) | 20.30 (−19.1%) | 22.43 (−26.8%) | 26.90 (−38.9%) | 41.0→37.9 | −0.45→−0.57 | 11.2% |
| RDW | 5.89 | 7.46 (−21.0%) | 8.96 (−34.2%) | 9.81 (−39.9%) | 10.73 (−45.1%) | 38.5→35.4 | −0.10→−0.11 | 12.1% |
| ASTS | 23.58 | 32.60 (−27.7%) | 44.71 (−47.3%) | 54.40 (−56.7%) | 70.85 (−66.7%) | 33.2→30.9 | −0.36→−0.33 | 15.9% |
| MRVL | 131.58 | 161.00 (−18.3%) | 216.99 (−39.4%) | 216.38 (−39.2%) | 189.16 (−30.4%) | 38.6→35.3 | −0.27→−0.07 | 12.8% |
| **MU** | 629.79 | 761.90 (−17.3%) | 901.98 (−30.2%) | 914.21 (−31.1%) | 775.34 (−18.8%) | 42.5→37.4 | −4.91→**−6.09** | 10.8% |
| VELO | 3.01 | 4.85 (−38.0%) | 7.37 (−59.2%) | 9.73 (−69.1%) | 12.51 (−75.9%) | 30.7→28.8 | −0.07→−0.05 | 20.7% |
| NBIS | 87.30 | 127.55 (−31.6%) | 176.61 (−50.6%) | 194.05 (−55.0%) | 179.78 (−51.4%) | 36.0→33.6 | −2.21→−2.03 | 19.9% |
| CRWV | 42.60 | 50.65 (−15.9%) | 66.53 (−36.0%) | 75.99 (−43.9%) | 87.52 (−51.3%) | 43.3→39.0 | +0.31→**+0.17** | 15.8% |
| OUST | 24.98 | 31.62 (−21.0%) | 34.58 (−27.8%) | 36.84 (−32.2%) | 33.16 (−24.6%) | 42.3→38.2 | −0.72→−0.82 | 13.1% |
| CRDO | 106.46 | 131.99 (−19.3%) | 165.96 (−35.9%) | 192.46 (−44.7%) | 181.00 (−41.2%) | 42.6→38.0 | −0.25→−0.51 | 14.9% |
| KTOS | 28.20 | 34.87 (−19.1%) | 39.60 (−28.8%) | 45.75 (−38.4%) | 57.78 (−51.2%) | 30.3→29.8 | −0.67→−0.58 | 8.1% |
| PL | 10.64 | 12.86 (−17.2%) | 14.64 (−27.3%) | 18.25 (−41.7%) | 25.64 (−58.5%) | 36.3→33.9 | −0.14→−0.17 | 9.7% |

**[FACT]** Every watchlist name and every index ETF closed **below all four SMAs**.

**Breakdowns, breakouts and level changes:**
- **MU breakdown.** It lost $650 (the Nov 5 low and Monday's reclaim) and closed $629.79, giving back two-thirds of Monday's gain. The MACD histogram is widening negative again.
  - **[VIEW]** Monday's "failed breakdown" is now a **failed reclaim**, which is bearish.
  - New support: $622 (today's low), then $585 (Nov 20 low). Resistance: $650, $672, then $720.
  - Volume of 1.01× is average, not climactic.
- **ASTS** set a new 52-week low at $22.52 and recovered 4.7% from it. **[VIEW]** A possible undercut-and-reclaim. It needs a close above $25.2 (today's open) to matter.
- **MRVL** broke the $138–139 double low. Next support: $120.6. The MACD histogram is still contracting (−0.07), so momentum is neutral, not accelerating down.
- **CRWV:** the MACD histogram is still positive (+0.17) but fading. Price is $3.3 above the $39.28 52-week low. **[VIEW]** This is the double-bottom-or-break level.
- **CRDO** closed below its $112–118 support zone at 6% of range. **[VIEW]** A bearish close; $104 is the line.
- **BKSY** ($16.43, vs. the $16.09 Nov 20 low), **PL** ($10.64, vs. the $10.35 52-week low) and **VELO** ($3.01, vs. $2.85) all closed **within 2–6% of their lows, near the bottom of the day's range**. **[VIEW]** Tomorrow's open decides retest-hold versus breakdown.
  - My 52-week lows come from Massive adjusted candles: BKSY $15.07, RDW $5.12. These differ from the morning brief's $13.25 and $4.87.
- **KTOS:** RSI is below 30 (29.8), but the MACD histogram is improving and price is holding $27.65–28.95. **[VIEW]** Relative-strength divergence versus semis. A reclaim of $29.75 is still needed.
- **Indices:**
  - SPY undercut Monday's low by ~$1.4 and recovered, closing at 76% of range.
  - QQQ filled part of Monday's gap: low $631.23, below Monday's ~$642.
  - SMH retraced about half of Monday's +15%.
  - **[VIEW]** A rotation day (Dow up, semis down), not liquidation. The 200-DMA reclaim on SPY ($733) is still the regime test, and it is 2% away.

---

### 5️⃣ Plan for tomorrow (Wed Nov 25: last full session before Thanksgiving)

**Regime [VIEW]:** Bear-market rally that is fading in high-beta tech; the broad market is stable. PCE at 8:30 ET is the swing factor.
- A hot core PCE reinforces the Dec 9 hike: a negative for every long-duration name here.
- A soft print could spark a second relief attempt, helped by Dell's AI backlog.
- **Keep size at about half normal.** Do not enter before 10:00 ET (after the data reaction).
- Thin pre-holiday liquidity: expect exaggerated moves.

| Ticker | Signal (vs. morning) | Entry zone | Stop | Targets | R:R (T1/T2) | Condition / note |
|---|---|---|---|---|---|---|
| **KTOS** | **POTENTIAL BUY** (=), best relative strength | $27.65–28.40 | $25.40 | T1 $32.0, T2 $35.5 (SMA20) | From $28.0: **1.5 / 2.9** | Enter only after a 1h close above **$29.00** (today's high) or a reclaim of $29.75. No catalyst; a close below $26.60 invalidates. |
| **OUST** | **POTENTIAL BUY** (=) | $24.50–25.20 | $22.90 | T1 $28.75, T2 $32.0 | From $24.9: **1.9 / 3.6** | Needs a 1h close above **$25.35** with $24.49 held. |
| **RKLB** | **HOLD / MONITOR** (=) | $44.6–46.0 | $41.80 | T1 $52.2, T2 $55.0 | From $45.5: **1.8 / 2.6** | Upgrade to Potential Buy on a hold of $44.57 **plus** a 1h close above $47.15 (today's high). Form 144 tax sales are routine supply. |
| **BKSY** | **POTENTIAL BUY → watch closely** (weakened) | $16.10–16.60 | $15.20 | T1 $18.8, T2 $20.3 | From $16.4: **2.0 / 3.3** | Needs a **reclaim of VWAP $16.94** on a 1h close. A daily close below $16.09 → invalid. |
| **PL** | **POTENTIAL BUY** (=), weak | $10.40–10.80 | $9.70 | T1 $12.1, T2 $13.0 | From $10.6: **1.7 / 2.7** | Needs a 1h higher low above $10.62 and a reclaim of $10.95. A close below $10.35 → invalid. Earnings Dec 10. |
| **MU** | **HOLD / MONITOR** (↓ from Potential Buy) | $588–600 (retest of the Nov 20 low) | $560 | T1 $650, T2 $672 | From $594: **1.6 / 2.3** | Alternative: a daily close back **above $650** re-opens long. The Dec 1 UBS chat and ~Dec 16 earnings (est.) are the catalysts. Do not average down between $600 and $650. |
| **CRWV** | **HOLD / MONITOR** (↓ from Potential Buy) | speculative $39.5–41.0 (double-bottom test) | $37.80 | T1 $47.0, T2 $50.7 (SMA20) | From $40.3: **2.6 / 4.2** | Only with a 1h higher low above $39.28. The HPE financing comment hits the thesis; size very small. |
| **CRDO** | **HOLD / MONITOR** (↓ from Potential Buy) | none until reclaim | $104 | — | — | Needs a daily close back above **$112**. Earnings Dec 1 after the close; prefer waiting for the reaction. |
| **MRVL** | **HOLD / MONITOR** (=) | none before Dec 1 | — | — | — | Support $120.6. After earnings, look for a hold above $128 or a reclaim of $140. |
| **ASTS** | **HOLD / MONITOR** (=) | none | — | — | — | A director's ~$1.0M buy is a positive. Reconsider on a daily close above **$25.20** with $22.52 held. |
| **NBIS** | **AVOID** (↓ from Hold) | — | — | — | — | Heaviest volume selling (1.39×) and financing risk. Support $80.7, then $73.5. |
| **RDW** | **AVOID / HIGH RISK** (=) | — | — | — | — | Lost $6.06. CEO buy versus ATM and Underperform rating. |
| **VELO** | **AVOID / HIGH RISK** (=) | — | — | — | — | $2.85 52-week low is in play. |

**R:R definition:** distance to target ÷ distance to stop, from the stated entry. These are [VIEW] levels derived from [FACT] price data. Every "POTENTIAL BUY" is conditional on its trigger. **There are no unconditional buys.**

**Key events (Wed Nov 25, ET):**
- **8:30:** October **PCE / core PCE**, **Q3 GDP (second estimate)** and **weekly jobless claims** (moved up a day for the holiday). Sources: [Kiplinger](https://www.kiplinger.com/investing/economy/this-weeks-economic-calendar), [Nasdaq week ahead](https://www.nasdaq.com/articles/week-ahead-pce-data-thanksgiving-holiday). [FACT] for the schedule; consensus figures not verified.
- **14:00:** **Beige Book**, per [financecalendar](https://www.financecalendar.com/events/2026-11-25/). [EST]: confirm on federalreserve.gov.
- **Fed speakers:** none confirmed in my searches. [EST] The pre-FOMC blackout begins Sat Nov 28 for the Dec 8–9 meeting.
- **Earnings reaction:** Dell (+~4% AH) at the open is the sentiment test for AI hardware.
- **Watchlist earnings:** none tomorrow. Next up: MRVL and CRDO on Dec 1 (after the close), and PL on Dec 10.
- **Calendar:** Thu Nov 26 market **closed**. Fri Nov 27 early close at 13:00 ET.

**Top 3 things to watch tomorrow [VIEW]:**
1. **Core PCE at 8:30.** A hot print plus a 95% hike probability means semis and neoclouds likely make lower lows. SMH $418 is today's low and the line to watch.
2. **Whether MU holds $622 or reclaims $650.** A reclaim of $650 re-opens the long thesis; a loss of $622 targets the $585–600 retest.
3. **Retest-or-break names: BKSY $16.09, PL $10.35, CRWV $39.28.** Each closed near its day's low, just above key support.

---
*Not investment advice. Prices are delayed feed data as of the Nov 24 close and after-hours. Confirm live quotes before acting.*
