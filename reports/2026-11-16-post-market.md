## 🌙 Post-Market Briefing: Monday, November 16, 2026

**Data notes (please read first)**
- **Retrieved:** 2026-11-16, 21:32–21:50 UTC (23:32–23:50 Bucharest; 16:32–16:50 ET).
- **Today's prices.** Massive (Polygon) again refuses same-day data on this plan (daily bar, minute bars and `/v1/open-close` for today all return "not authorized"). Today's open/high/low/close and volume therefore come from the **Stock Analysis** daily history pages, read at about 16:50 ET. I cross-checked every close against **Twelve Data**; the largest gap is 19 cents (ALAB), most are under 5 cents. Stock Analysis' Nov 13 rows match Massive exactly, which is why I trust it for today.
- **History:** daily candles through Nov 13 are from Massive. All % changes are today's close vs. the Massive Nov 13 close. "5D" is vs. the Nov 9 close.
- **Relative volume is provisional.** It is today's Stock Analysis volume divided by the 20-day average from Massive. The volume was read under an hour after the close and may be revised upward. Twelve Data's volume was unusable again (for example 0.47M shares for RKLB and 3.5B for NVDA).
- **After-hours:** Twelve Data extended quote with its own timestamp, taken 30–45 minutes after the close. After-hours trading runs until 20:00 ET, so these are early prints. Twelve Data's intraday pre/post bars are not on this plan.
- **Indicators:** computed by me from the candles: SMA 20/50/100/200, RSI(14, Wilder), MACD(12,26,9), ATR(14). They include today's close. Intraday checks use 30-minute regular-session bars from Twelve Data.
- **Morning brief:** setups are checked against `reports/2026-11-16-market-intelligence.md`, which sits on branch `claude/pensive-clarke-pm5ftv` (not on this branch). The three extra candidates in that file are **LUNR, CRDO, ALAB**.
- **Filings:** checked through SEC EDGAR full-text search at 21:45 UTC. EDGAR blocked direct document downloads from this environment, so I could list today's filings but not read them.
- **Labels:** **[Confirmed]** = SEC filing or company release. **[Reported]** = media. **[Est.]** = unconfirmed. **Opinion** = my analysis. Not personalised financial advice.

---

### 🧭 The day in three lines
1. **Broad AI and chip selloff ahead of Nvidia.** SMH -5.1%, QQQ -2.7%, SPY -1.9%. All 13 watchlist names closed lower, and nine of them fell more than 6.5%. Reported drivers: new US chip export restrictions, Treasury pressure on Nvidia, and a ULA Vulcan launch failure that hit space names.
2. **Three support levels from this morning's alert list broke on a closing basis:** **MU lost its 200-day average** ($719.02 vs. $767.13), **NBIS closed below $109** ($107.13) and **OUST closed below $32** ($31.23). Volume was below average on all three except NBIS (1.07×), so these are breaks without a volume confirmation.
3. **No morning setup triggered with confirmation, and no stop or target was hit.** RKLB, CRWV, CRDO and ALAB closed inside their entry zones without a reversal. LUNR fell through its zone. MU gapped below its zone and never traded in it.

---

### 1. Session recap

| Ticker | Close | % chg | 5D | Open | High | Low (time ET) | Rel. vol (prov.) | After-hours (ET) | AH vs close |
|---|---|---|---|---|---|---|---|---|---|
| **SPY** | 739.95 | -1.91% | -1.7% | 749.66 | 749.82 | 738.07 (14:30) | 1.43× | 740.20 @ 16:28 | +0.0% |
| **QQQ** | 661.75 | -2.67% | -2.6% | 671.04 | 672.15 | 660.48 (15:30) | 0.84× | 662.08 @ 16:29 | +0.0% |
| **SMH** | 461.90 | -5.11% | -5.2% | 468.71 | 473.33 | 460.64 (15:30) | 0.84× | 463.20 @ 16:15 | +0.3% |
| RKLB | 57.37 | -6.76% | -2.5% | 59.65 | 61.90 | 57.16 (15:30) | 0.71× | 57.24 @ 16:27 | -0.2% |
| BKSY | 23.15 | -2.73% | -3.1% | 23.17 | 24.25 | 22.85 (09:30) | 0.61× | no post-close print | n/a |
| RDW | 7.05 | -8.80% | -13.5% | 7.42 | 7.46 | 7.02 (15:30) | 0.72× | 7.04 @ 16:07 | -0.1% |
| ASTS | 28.58 | **-12.33%** | -22.5% | 31.62 | 32.04 | 28.30 (15:30) | **1.30×** | 28.45 @ 16:01 | -0.5% |
| MRVL | 145.36 | -7.27% | -6.0% | 147.56 | 149.16 | 144.04 (10:00) | 0.70× | 145.92 @ 16:10 | +0.4% |
| MU | 719.02 | **-7.62%** | -1.9% | 734.16 | 739.12 | 716.38 (15:30) | 0.87× | 723.47 @ 16:40 | +0.6% |
| VELO | 3.55 | **-14.46%** | -43.0% | 4.00 | 4.06 | 3.54 (15:30) | 1.23× | no post-close print | n/a |
| NBIS | 107.13 | -7.55% | -24.3% | 106.80 | 111.55 | 104.75 (09:30) | 1.07× | 107.82 @ 16:32 | +0.6% |
| CRWV | 49.88 | -6.12% | +1.8% | 49.36 | 52.06 | 48.59 (09:30) | 0.70× | 50.02 @ 16:35 | +0.3% |
| OUST | 31.23 | -6.72% | -19.0% | 31.59 | 32.33 | 30.78 (10:00) | 0.64× | no post-close print | n/a |
| LUNR | 11.73 | -9.77% | -2.6% | 12.53 | 12.60 | 11.63 (15:30) | 0.86× | 11.75 @ 16:00 | +0.2% |
| CRDO | 120.71 | -8.21% | -9.2% | 122.62 | 124.62 | 118.60 (09:30) | 0.79× | 121.02 @ 16:30 | +0.3% |
| ALAB | 202.34 | -8.79% | -6.7% | 209.00 | 211.64 | 201.00 (09:30) | 0.92× | 203.40 @ 16:38 | +0.5% |
| *NVDA (context)* | 156.14 | -4.12% | -12.6% | 159.02 | 163.20 | 155.01 (13:30) | 1.57× | 156.67 @ 16:42 | +0.3% |

Low times are the start of the 30-minute bar that held the low.

- **Shape of the day:** gap down at the open, a bounce that peaked around 11:00–11:30 ET, then a steady slide into the close. Seven watchlist names (RKLB, RDW, ASTS, MU, VELO, LUNR, plus QQQ and SMH) made their lows in the final 30 minutes. That is a weak close.
- **Volume:** most declines came on **below-average** volume (0.6–0.9×). The exceptions are ASTS (1.30×), VELO (1.23×), NVDA (1.57×) and SPY (1.43×). Opinion: this looks like buyers stepping away before Nvidia rather than forced selling, but the volume figures are provisional.
- **After-hours is flat to slightly higher** (MU +0.6%, NBIS +0.6%, ALAB +0.5%). No watchlist company reported after the close.
- **Indices [Reported, from a live blog that may not show final values]:** S&P 500 -1.92% to 7,416.59, Nasdaq Composite -2.49% to 24,509.76, Dow -1.41% to 51,608.17, Russell 2000 -1.70% to 2,742.94. The point changes reconcile exactly with Friday's closes. 10-year yield about 5.12%. WTI crude -3.8% to $85.21 ([Yahoo Finance](https://finance.yahoo.com/markets/live/stock-market-today-monday-november-16-dow-sp-500-nasdaq-nvidia-oil-091631084.html)).

---

### 2. Morning setups: what happened

| Ticker | Morning plan | Result | Detail |
|---|---|---|---|
| **RKLB** | Buy $55.50–58.00; confirm a 4h close back above its EMA20 with the daily low above $55; alternative: daily close above $62.50 on 1.3× volume; stop $52.50 | ⏸ **NOT TRIGGERED: in zone, no confirmation** | Entered the zone after 12:00 ET and closed in it at $57.37 (low $57.16). Lower highs all afternoon and a close near the low, so no 4h reclaim. Daily low held above $55. Stop not hit. |
| **CRWV** | Buy $47.00–50.00; confirm a 1h/4h higher low **and** the post-Nvidia reaction holding $47; stop $44 | ⏸ **NOT TRIGGERED: in zone, confirmation cannot complete before Nvidia** | Low $48.59 in the first 30 minutes, then every later bar held above it. Closed $49.88, inside the zone. It undercut Friday's $49.24 low. Stop not hit. |
| **MU** | Buy $740–770; confirm a daily close above the 200 DMA after Nvidia, then a 4h reclaim of $790; stop $695 | ❌ **NOT TRIGGERED: setup damaged** | Opened $734.16, **below** the zone, and the day's high was $739.12, so it never traded in the zone. Closed $719.02, about 6% under the 200 DMA ($767.13). Stop $695 not hit (low $716.38). |
| **OUST** | Buy $31.80–33.00; confirm a daily close above the 200 DMA ($32.87) plus a 1h bullish reversal; stop $29.80. "A close below $32 with volume means the 200 DMA failed." | ❌ **NOT TRIGGERED: setup damaged** | Traded in the zone only in the first hour (high $32.33). Closed $31.23, below $32, the 200 DMA ($32.92) and the 20 DMA ($32.40). Volume was light (0.64×), so the "with volume" condition is not met. Stop not hit (low $30.78). |
| **BKSY** | Wait for a retest of $22.00–22.80; stop $20.40 | ⏸ **NOT TRIGGERED** | Low $22.85, 5 cents above the zone. Closed $23.15 on light volume (0.61×). Smallest decline on the list. |
| **LUNR** | Wait for a retest of $12.10–12.70; stop $11.30 | ⚠️ **ZONE REACHED, RETEST FAILED** | Opened $12.53 inside the zone, lost $12.10 by midday and closed $11.73, below the zone and the $12.10 breakout level. No confirmation rule was set this morning; a zone fill at the $12.40 midpoint is 5.4% under water. Stop $11.30 not hit (low $11.63). |
| **CRDO** | $112–122, only on a reversal; invalidation $104 | ⏸ **NOT TRIGGERED: in zone, no reversal** | Low $118.60, close $120.71, a red candle closing in the lower half of its range. |
| **ALAB** | $195–210; invalidation $175 (signal: hold/monitor) | ⏸ **NOT TRIGGERED: in zone, no reversal** | Low $201.00, close $202.34, near the low. |
| **MRVL** | No trade; needs a base above $132.5 and a reclaim of $174.5 | ⏸ **NOT TRIGGERED; support broke** | Closed $145.36, below the $149 support (Friday's low $149.17). |
| **RDW** | No trade; reconsider on a daily close above $8.71 | ⏸ **NOT TRIGGERED; support broke** | Closed $7.05, below the $7.21–7.45 support band. |
| **ASTS** | No trade; reconsider on a close above $37.80 or a reversal at $27.6 | 🛑 **AVOID stands** | -12.3% on 1.3× volume. Low $28.30, 72 cents above the 52-week low ($27.58). No reversal candle. |
| **NBIS** | No trade; revisit after a base above $109 and a reclaim of $132 | 🛑 **AVOID stands; $109 broke** | Opened below $109, low $104.75, closed $107.13. First close under the $109 low. |
| **VELO** | No trade | 🛑 **AVOID stands** | New low at $3.54, closed $3.55, despite a contract announcement (see section 3). |

**Summary: triggered 0, in zone without confirmation 4 (RKLB, CRWV, CRDO, ALAB), damaged 3 (MU, OUST, LUNR), invalidated by a stop 0, targets hit 0.**

Alert levels from the morning brief: **NBIS $109 broken, MU $750 broken, OUST $32 broken, BKSY $20 intact.**

---

### 3. Earnings, filings and material news (Nov 16, incl. after-hours)

No watchlist company reported earnings today, and none filed an 8-K, Form 4, S-3 or ATM prospectus on Nov 14–16 (EDGAR full-text search, 21:45 UTC).

**Market-wide**
- **Chip export rules [Reported]:** the Commerce Department moved to close a loophole that let Chinese firms rent Nvidia computing capacity located abroad, with new restrictions affecting Southeast Asia ([AOL/Reuters](https://www.aol.com/articles/wall-street-slides-nvidia-casts-175434000.html), [Yahoo/Reuters](https://finance.yahoo.com/markets/stocks/articles/p-500-nasdaq-futures-slide-104351968.html), [Motley Fool](https://www.fool.com/investing/2026/11/16/why-amd-stock-was-sliding-today/)).
- **Nvidia [Reported]:** Treasury Secretary Bessent called for a "dramatic shakeup" at Nvidia and asked for answers on China export compliance within 10 days ([Motley Fool](https://www.fool.com/investing/2026/11/16/u-s-treasury-secretary-scott-bessent-just-issued-a-blistering-warning-to-nvidia/)). Yahoo reports Nvidia fell about 4% on word that its board is not considering bringing Jensen Huang back as CEO ([Yahoo Finance](https://finance.yahoo.com/markets/live/stock-market-today-monday-november-16-dow-sp-500-nasdaq-nvidia-oil-091631084.html)). NVDA closed $156.14 with RSI 22.7. Results are due **Tuesday after the close**.
- **Fed [Reported]:** Chair Warsh spoke in San Francisco and said AI could lift growth but could also lead to layoffs in a slowdown; commentators linked the afternoon selling to the remarks ([BigGo Finance](https://finance.biggo.com/news/bef30632-90cc-4372-880b-f01d685418a3)). I did not find a transcript.
- **Empire State manufacturing [Reported]:** 7.8 in November vs. 16.7 expected and 25.5 in October ([Zacks](https://www.zacks.com/stock/news/3030440/pre-markets-in-the-red-to-start-a-fresh-week)).
- **Space sector [Reported]:** a ULA Vulcan rocket failed about 10 minutes into flight on Sunday and destroyed 40 Amazon Leo satellites. No watchlist company had a payload on board; the concern is a tighter US launch bottleneck ([TIKR](https://www.tikr.com/blog/ast-spacemobile-sinks-8-as-ulas-vulcan-rocket-failure-rattles-space-stocks), [Benzinga](https://www.benzinga.com/trading-ideas/movers/26/11/63295932/rocket-lab-firefly-ast-spacemobile-stocks-drop-whats-going-on-with-space-stocks-monday)).

**VELO**
- **Defense award [Confirmed, company release]:** Velo3D was selected by the US Army DEVCOM Armaments Center for an award worth **up to $10M** under the Low-Cost Warheads and Lethal Payloads for Unmanned Systems challenge. The total depends on government funding of later phases ([Stockhouse](https://stockhouse.com/news/press-releases/2026/11/16/velo3d-selected-for-u-s-defense-award-with-potential-value-of-up-to-10-million)).
- Opinion: the stock fell 14.5% to a new low on above-average volume on the day of a positive release. That is the weakest reaction on the list.

**ASTS**
- **No company announcement** found for today. Coverage attributes the -12% move to the Vulcan failure, the tech selloff and existing overhangs (Q3 miss, constellation delay) ([TIKR](https://www.tikr.com/blog/ast-spacemobile-sinks-8-as-ulas-vulcan-rocket-failure-rattles-space-stocks)). BlueBirds 14–16 still have no confirmed launch date.

**MU**
- **No new company news** and no filing. Motley Fool ties the drop to Nvidia and mentions a DRAM price-collusion class action against Micron, Samsung and SK Hynix ([Motley Fool](https://www.fool.com/investing/2026/11/16/why-micron-stock-keeps-going-down/)). My search shows that suit was filed on June 25, 2026, so it is not new ([Quartz](https://qz.com/samsung-sk-hynix-micron-antitrust-class-action-memory-price-fixing-062526)).
- The "Form 4 dated Nov 15" flagged as unverified this morning does **not** appear on EDGAR. The latest insider filings are two Form 144s from Nov 12 (Sumit Sadana).

**MRVL**
- **No new company news** and no filing today. The move followed the chip sector, with Lumentum deal dilution cited again ([Motley Fool](https://www.fool.com/investing/2026/11/16/why-marvell-stock-is-down-today/)).

**NBIS**
- **Schedule 13G/A [Confirmed], filed today** by Situational Awareness LP (accession 0000935836-26-000604). I could not open the document, so I do not know whether the stake went up or down.
- A Form 4 for Marc Boroditsky was filed Nov 13 [Confirmed]; contents not read.
- One outlet mentions an analyst target cut today without naming the firm [Reported, unverified] ([Invezz](https://invezz.com/news/2026/11/16/coreweave-stock-falls-6-as-nvidia-leadership-uncertainty-weighs/)).

**CRWV**
- **No new company news.** A Form 4 for director Glenn Hutchins was filed Nov 13 [Confirmed]; contents not read. The reported $4B+ loan has still not been announced. Coverage ties today's drop to Nvidia and to last week's Microsoft report ([Seeking Alpha](https://seekingalpha.com/news/4673004-coreweave-nebius-lead-neocloud-decline-as-ai-stocks-prepare-for-nvidia-earnings), [TipRanks](https://www.tipranks.com/news/coreweave-nebius-and-iren-fall-in-pre-market-today-nov-16-heres-why)).

**LUNR**
- **Canaccord trimmed its price target to $38 and kept Buy** [Reported] ([MarketBeat](https://www.marketbeat.com/instant-alerts/analyst-intuitive-machines-nasdaq-lunr-stock-price-target-lowered-at-canaccord-genuity-group-2026-11-16/)).

**RKLB, BKSY, RDW, OUST, CRDO, ALAB:** **No material news.** No filing and no company headline today. RKLB coverage was commentary on last week's results and the Neutron price increase to $70M per launch ([Motley Fool](https://www.fool.com/investing/2026/11/16/not-spacex-not-blue-origin-the-space-stock-that-just-raised-its-l)).

---

### 4. Technical update (daily, includes today's close)

| Ticker | Close | 20 DMA | 50 DMA | 100 DMA | 200 DMA | RSI(14) | MACD line / signal | MACD histogram (prev) |
|---|---|---|---|---|---|---|---|---|
| SPY | 739.95 | 757.70 ↓ | 763.82 ↓ | 760.34 ↓ | 732.16 ↑ | 40.4 | -5.03 / -4.28 | -0.75 (-0.03) |
| QQQ | 661.75 | 692.62 ↓ | 716.72 ↓ | 713.90 ↓ | 682.44 ↓ | 37.8 | -13.88 / -13.04 | -0.84 (-0.09) |
| SMH | 461.90 | 513.81 ↓ | 557.70 ↓ | 565.83 ↓ | 524.18 ↓ | 35.6 | -24.27 / -22.37 | -1.90 (-0.84) |
| RKLB | 57.37 | 56.08 ↑ | 62.33 ↓ | 68.62 ↓ | 78.17 ↓ | 47.8 | -0.33 / -1.58 | +1.26 (+1.68) |
| BKSY | 23.15 | 19.75 ↑ | 20.61 ↑ | 22.97 ↑ | 27.01 ↓ | 60.3 | 0.96 / 0.25 | +0.71 (+0.82) |
| RDW | 7.05 | 8.08 ↓ | 9.49 ↓ | 10.13 ↓ | 10.85 ↓ | 38.4 | -0.52 / -0.55 | +0.03 (+0.08) |
| ASTS | 28.58 | 37.14 ↓ | 49.03 ↓ | 57.88 ↓ | 73.20 ↓ | 32.6 | -4.83 / -4.86 | +0.03 (+0.30) |
| MRVL | 145.36 | 190.16 ↓ | 227.64 ↓ | 224.15 ↓ | 187.33 ↓ | 32.6 | -24.59 / -22.42 | -2.17 (-2.39) |
| MU | 719.02 | 828.71 ↓ | 937.83 ↓ | 938.05 ↓ | 767.13 **↓ (new)** | 38.0 | -57.16 / -54.33 | -2.83 (-1.41) |
| VELO | 3.55 | 5.88 ↓ | 8.25 ↓ | 10.53 ↓ | 12.81 ↓ | 26.5 | -1.13 / -1.04 | -0.10 (-0.04) |
| NBIS | 107.13 | 147.97 ↓ | 192.21 ↓ | 202.65 ↓ | 179.46 ↓ | 33.9 | -20.35 / -18.76 | -1.58 (-0.68) |
| CRWV | 49.88 | 54.43 ↓ | 71.81 ↓ | 78.71 ↓ | 88.77 ↓ | 40.5 | -5.61 / -6.72 | +1.11 (+1.30) |
| OUST | 31.23 | 32.40 **↓ (new)** | 35.50 ↓ | 38.38 ↓ | 32.92 **↓ (new)** | 44.4 | -0.06 / -0.46 | +0.40 (+0.78) |
| LUNR | 11.73 | 11.08 ↑ | 12.85 **↓ (new)** | 14.42 ↓ | 19.26 ↓ | 49.4 | -0.14 / -0.51 | +0.37 (+0.45) |
| CRDO | 120.71 | 146.44 ↓ | 171.28 ↓ | 200.75 ↓ | 180.84 ↓ | 37.2 | -14.90 / -14.59 | -0.30 (+0.09) |
| ALAB | 202.34 | 242.75 ↓ | 292.10 ↓ | 311.28 ↓ | 257.72 ↓ | 35.8 | -25.30 / -24.95 | -0.35 (+0.02) |

↑ = close above the average, ↓ = close below. "(new)" = the close crossed that average today.

**Breakdowns and levels that changed**
- **MU: closed below the 200 DMA** for the first time in this pullback, by 6.3%, on 0.87× volume. The gap from Friday's $750.25 low to today's $739.12 high is now resistance. Support $716.4 (today's low), then $690–700, then **$650** (60-day low). Resistance $739–750, then $767 (200 DMA). MACD histogram widened to the downside.
- **NBIS: first close below the $109 low**, volume 1.07×. New support **$104.75**; there is no earlier level nearby on my 60-day data. Resistance $109, $111.55, then $115.9.
- **OUST: lost the 200 DMA ($32.92) and 20 DMA ($32.40)** on light volume (0.64×). Support $30.78, then about $28.2 (Nov 5 low). Resistance $32.3–32.9.
- **QQQ:** second close below the 200 DMA, now 3% under it. Support $660.5, then the Nov 5 low at **$647.05**. Resistance $672, then $682.4.
- **SMH:** -5.1%, 12% under its 200 DMA. Support $460.6, then the Nov 5 low at **$445.59**. Resistance $473.3 (Friday's low, today's high).
- **SPY:** still 1.1% above its 200 DMA ($732.16). The 60-day low is $732.71, so **$732–733 is the level to watch tomorrow.**
- **ASTS:** -12.3% on 1.30× volume, the only watchlist breakdown with clear volume behind it. Support is the 52-week low at **$27.58**. Resistance $30.4–32.0.
- **MRVL:** lost $149. Support $144.0, then **$132.54**. Resistance $149.2, then $156.8.
- **RDW:** lost the $7.21–7.45 band. Next support **$6.06**. Resistance $7.45.
- **LUNR:** lost the $12.10 breakout level and the 50 DMA ($12.85). Support $11.63, then the 20 DMA at $11.08. Resistance $12.10, then $12.60.
- **RKLB:** still above the 20 DMA ($56.08) by $1.29. Support $56.1, then $55. Resistance $59.5, then $61.9–62.3. MACD histogram positive but shrinking for a second day.
- **CRWV:** held a higher low intraday after the opening flush. Support $48.59, then $47. Resistance $52.06, then $54.4 (20 DMA).
- **CRDO and ALAB:** MACD histograms turned negative again. CRDO support $118.6, then $110.83. ALAB support $201.0, then $177.6.
- **VELO:** new low at $3.54, RSI 26.5. No support below.
- **BKSY:** unchanged structure. Still above the 20, 50 and 100 DMA. Support $22.85, then $22.2. Resistance $24.25, then $24.92.
- **No watchlist name broke out to the upside.**

---

### 5. Plan for Tuesday, Nov 17

Levels are opinion. Nvidia reports after Tuesday's close, so any entry made during Tuesday's session carries that event risk overnight.

| Ticker | Signal | Entry zone / trigger | Stop | Targets | Note |
|---|---|---|---|---|---|
| **BKSY** | ⏳ **WAIT FOR RETEST** | $22.00–22.80, held on light volume with an hourly higher low | $20.40 | $27.0 / $28.3 | Best relative strength on the list. Presents at Craig-Hallum on Tuesday. No chase above $24.25. |
| **RKLB** | ⏳ **WAIT: in zone, unconfirmed** | $55.50–58.00, only after an hourly close back above $59.5 with the 20 DMA ($56.1) holding | $52.50 | $62.3 / $68.0 | A daily close below $55 cancels the setup. |
| **CRWV** | ⏳ **WAIT: in zone, decide after Nvidia** | $47.00–50.00, only if Wednesday's reaction holds $47 and makes an hourly higher low | $44.00 | $62.0 / $72.5 | Half size at most. Do not enter before the print. |
| **MU** | 👀 **HOLD / MONITOR (downgraded from Potential Buy)** | Either a daily close back above $767 (200 DMA) after Nvidia, or a reversal candle in $650–700 | n/a until a new base forms | Resistance $739–750 / $767 / $829 | The $740–770 zone is now overhead resistance. This morning's setup is withdrawn. |
| **OUST** | 👀 **HOLD / MONITOR (downgraded from Potential Buy)** | Daily close back above $32.9 | $29.80 for anyone already in | $35.5 / $38.4 | Break came on light volume, so a quick reclaim is possible, but it needs to be seen first. |
| **LUNR** | 👀 **HOLD / MONITOR (downgraded from Wait for Retest)** | Daily close back above $12.10, or a hold of the 20 DMA ($11.08) with a reversal | $11.30 for anyone already in; $10.60 on a fresh entry at the 20 DMA | $12.85 / $14.6 | Retest failed today. |
| **CRDO** | 👀 **HOLD / MONITOR** | $112–122, only on a reversal day after Nvidia | $104 | $149 / $172 | In zone, falling. Moves with SMH. |
| **ALAB** | 👀 **HOLD / MONITOR** | $195–210, only on a reversal day after Nvidia | $175 | $247 / $294 | In zone, closed near the low. |
| **MRVL** | 👀 **HOLD / MONITOR** | No entry. Needs a base above $132.5 | n/a | Resistance $149.2 / $156.8 / $174.5 | Earnings date still unconfirmed (Nov 26 or Dec 1). |
| **RDW** | 👀 **HOLD / MONITOR, leaning avoid** | Daily close above $8.08 (20 DMA) as a first step | n/a | n/a | Next support $6.06. |
| **NBIS** | ⛔ **AVOID / HIGH RISK** | No entry. First sign of repair: a daily close back above $111.6 | n/a | Resistance $109 / $111.6 / $115.9 | New closing low for the move. |
| **ASTS** | ⛔ **AVOID / HIGH RISK** | No entry. Only a sweep of $27.58 that reverses the same day, or a confirmed launch date | n/a | n/a | Volume-backed breakdown. |
| **VELO** | ⛔ **AVOID / HIGH RISK** | None | n/a | n/a | Sold off on good news. |

**Key events**
- **Tue Nov 17, 8:30 am ET (15:30 Bucharest): October retail sales** [Reported]. September was +0.8% vs. +0.3% expected ([thetrading.tools](https://www.thetrading.tools/economic-calendar/retail-sales)). A strong number adds to December rate-hike pricing.
- **Tue Nov 17, after the close: NVIDIA Q3 FY27 results** [Reported date]. Usual timing is a release around 16:20 ET (23:20 Bucharest) and a call at 17:00 ET (00:00 Bucharest) [Est.]. Guidance was $108.0B ±2%. This is the first report under interim CEO Colette Kress, with export rules and the Treasury request as open questions. Direct read-through for MU, MRVL, CRWV, NBIS, CRDO and ALAB.
- **Tue Nov 17: BlackSky at the Craig-Hallum Alpha Select conference** [Confirmed, company release cited this morning].
- **Wed Nov 18:** FOMC minutes at 2:00 pm ET (21:00 Bucharest) [Reported]; BlackSky at the Global Space & Defense Tech Summit.
- **Thu Nov 19:** Anthropic begins trading on Nasdaq [Reported] ([Motley Fool](https://www.fool.com/investing/2026/11/16/anthropic-s-ipo-takes-place-on-november-19-investors-will-learn-these-3-key-details/)).
- **Fed speakers on Tuesday:** not verified.
- **No watchlist company has confirmed earnings tomorrow.**

**Stance (opinion):** no new positions on Tuesday. Every index and every watchlist name closed lower, three alert levels broke, and the largest single event of the month arrives after tomorrow's close. The useful work tomorrow is watching whether SPY holds $732–733, QQQ holds $647 and SMH holds $445.6 into the print. If Nvidia steadies the group, the first candidates are the names that held structure today (BKSY, RKLB, CRWV). If it does not, MU's next real support is $650 and NBIS has none nearby.

---

*Sources are linked inline. Today's prices and volumes are from Stock Analysis, cross-checked with Twelve Data; history is from Massive. Facts are labeled; levels, signals and the stance are opinion, not personalised investment advice.*
