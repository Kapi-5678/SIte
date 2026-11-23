## 🌙 Post-Market Briefing: Monday, November 23, 2026

**Prepared:** ~23:45 EET (21:45 UTC), after the US close.
**Price data:**
- **Today's OHLC and after-hours (AH) prices** come from Twelve Data quotes, retrieved 21:33–21:40 UTC. Massive (Polygon) does not serve same-day bars on this plan; it returned "NOT_AUTHORIZED" for today's daily, minute and open-close data.
- **History through Fri Nov 20** comes from Massive daily candles.
- Indicators (SMA 20/50/100/200, RSI 14, MACD 12/26/9, ATR 14) are computed in-house on that history plus today's close.

**Data gaps:**
- **Relative volume for today is not available.** Twelve Data's intraday volume on this plan is partial: SPY shows 2.8M against a ~58M average, which cannot be consolidated volume. I am not quoting today's RVOL rather than guessing.
- AH prices are Twelve Data's "extended" last trade. Where the AH timestamp equals the 16:00 ET close, no after-hours trade was reported to that feed.

**Labels:** **[FACT]** = sourced or computed from data · **[EST]** = estimate or unconfirmed · **[VIEW]** = my analysis or opinion. Nothing here is personalised financial advice.

---

### 🧭 What happened today

- **[FACT]** It was the best day for US stocks since April 2025.
  - S&P 500 +4.7%, pulling it out of correction. Nasdaq-100 almost +7% (still in correction). Dow +~1,450 points. Philadelphia Semiconductor Index (SOX) +14%. Memory stocks +~18%.
  - **Nvidia +31.5%**, the largest one-day market-cap gain on record (~$950B per Bloomberg). The catalyst was **Nvidia's reinstatement of Jensen Huang as CEO**.
  - Huang had been briefly removed. Reports say the SEC has opened an investigation linked to the episode. President Trump said he urged the reinstatement.
  - Sources: [NBC News](https://www.nbcnews.com/business/markets/stocks-rebound-ai-tech-selloff-nvidia-rcna610833), [ABC News](https://abcnews.com/Business/stock-market-rebounds-sharply-after-selloff/story?id=138373790), [Quartz](https://qz.com/nasdaq-sp500-rebound-nvidia-huang-return-stocks-112326), [Motley Fool midday](https://www.fool.com/coverage/stock-market-today/2026/11/23/stock-market-midday-nov-23-nasdaq-surges-nearly-7-as-jensen-huang-s-return-sparks-historic-ai-rebound/).
- **[FACT]** Exact index closing figures differ slightly across sources, and some early reports were intraday. The ETF closes below come from candle data and take precedence.
- **[VIEW]** This was a **short-covering / relief gap, not yet a trend change**:
  - SPY, QQQ and SMH are all still below their 20-, 50- and 100-day SMAs. SPY and QQQ are also still below their 200-day.
  - Most watchlist names **gapped up 10–35% and then faded**. BKSY, ANET, KRMN and NBIS closed in the **bottom 15%** of the day's range.
  - **MU was the clear exception**: it closed at 76% of its range, above its broken $650 level.
  - The macro overhang is unchanged: PCE on Wednesday and a likely FOMC hike on Dec 9.

---

### 1️⃣ Session recap

| Ticker | Close | % chg | Open | High | Low | Close in range | AH price (time ET) | RVOL |
|---|---|---|---|---|---|---|---|---|
| **SPY** | 722.56 | +4.75% | 724.39 | 727.98 | 713.57 | 62% | 723.44 (16:29) | n/a |
| **QQQ** | 651.18 | +7.02% | 655.98 | 657.45 | 642.03 | 59% | 651.01 (16:27) | n/a |
| **SMH** | 459.79 | +14.93% | 468.28 | 468.77 | 449.64 | 53% | 459.46 (16:17) | n/a |
| RKLB | 49.62 | +9.25% | 52.16 | 52.16 | 48.32 | 34% | 49.60 (16:14) | n/a |
| BKSY | 17.58 | +7.39% | 17.91 | 18.68 | 17.50 | 7% | no AH print | n/a |
| RDW | 6.415 | +13.54% | 6.50 | 6.615 | 6.23 | 48% | 6.46 (16:09) | n/a |
| ASTS | 25.665 | +10.29% | 27.28 | 27.28 | 25.03 | 28% | 25.67 (16:00) | n/a |
| MRVL | 144.57 | +18.23% | 146.20 | 149.96 | 139.36 | 49% | no AH print | n/a |
| **MU** | **707.84** | **+19.06%** | 690.61 | 720.56 | 666.86 | **76%** | 708.42 (16:32) | n/a |
| VELO | 3.38 | +13.61% | 3.41 | 3.54 | 3.27 | 41% | no AH print | n/a |
| NBIS | 97.65 | +20.10% | 110.02 | 110.02 | 95.80 | 13% | 98.69 (16:30) | n/a |
| CRWV | 48.37 | +22.42% | 50.83 | 51.90 | 46.53 | 34% | 48.65 (16:30) | n/a* |
| OUST | 27.88 | +17.14% | 27.74 | 28.58 | 26.90 | 58% | no AH print | n/a |
| MRCY | 76.22 | +5.63% | 76.19 | 77.24 | 74.63 | 61% | no AH print | n/a |
| ANET | 177.93 | +6.15% | 185.54 | 187.21 | 177.07 | 8% | 179.20 (16:28) | n/a |
| KRMN | 30.335 | +3.71% | 31.275 | 31.56 | 30.195 | 10% | no AH print | n/a |

**Notes:**
- All values in the table are [FACT] from Twelve Data.
- *CRWV's feed volume of 109.1M (~1.56× its 20-day average of 69.9M) is the only figure that looks consolidated. It is unverified, so I am not relying on it.
- After-hours moves were small, all within ±1.1%. **[VIEW]** Nothing material was priced after the bell.

---

### 2️⃣ Morning setups: scorecard

| Ticker | Morning plan | What happened | Status |
|---|---|---|---|
| **BKSY** | Entry $16.00–16.80 after holding $16.1 and a 1H close above $17.04. Stop $14.90. | Gapped to $17.91; the low was $17.50, so price **never traded in the entry zone**. It held above $17.04 all day but faded to close near the low. Stop not hit. | **NOT TRIGGERED** (gapped over the zone). Setup still valid. |
| **RKLB** | Entry $43.50–46.50 only after a sweep of $43.89 and a reclaim of $46.97. Stop $41.40. | No sweep: the low was $48.32. Gap-and-fade from $52.16. | **NOT TRIGGERED** |
| **MU** | Upgrade trigger: a daily close above **$650**, then entry $650–660, stop $588, T1 $786. | Closed **$707.84**, a failed breakdown confirmed. But price never came back to $650–660 (the low was $666.86). | **TRIGGER CONDITION MET.** No fill in the entry zone, so do not chase. |
| **MRVL** | No trade before Dec 1 earnings. | +18%, closed above $132.5 and the 5-day VWAP of $140.3. | **N/A** (stand-aside rule) |
| **CRWV** | Revisit on a reclaim of $40.6 plus a higher 4H low. | Reclaimed $40.6 by a wide margin (close $48.37). The higher 4H low is not confirmed after one session. | **PARTIAL.** Reclaim yes, structure not yet. |
| **NBIS** | Speculative only on a sweep of $73.5 and a reclaim of $81. | No sweep (low $95.80). Opened at the high ($110.02) and faded 11%. | **NOT TRIGGERED** |
| **RDW** | Revisit on a daily close above $6.06. | Closed **$6.415**. | **RE-EVALUATE CONDITION MET** (watch item, not an entry) |
| **OUST** | Re-evaluate on a reclaim of $27.35. | Closed **$27.88**. | **RE-EVALUATE CONDITION MET** |
| **ASTS** | Needs a base and a reclaim of $27.58. | High $27.28: **rejected just below the trigger**. | **NOT TRIGGERED** |
| **VELO** | No trade. | +13.6%; still far below every MA. | **N/A** |
| **MRCY** | Entry $66–70 on a pullback. Stop $63. | The low was $74.63. | **NOT TRIGGERED** |
| **ANET** | Entry $158–162 only. Stop $151.50. | The low was $177.07; price reclaimed the 200-DMA but closed at the low of the day. | **NOT TRIGGERED** |
| **KRMN** | A daily close above $30.50 sets up the entry. | High $31.56, but **closed $30.335**, below the trigger. | **NOT TRIGGERED** |

**[FACT]** No stops were hit and no targets were reached. **No setup was invalidated.**

---

### 3️⃣ Earnings, filings and news (today, including after-hours)

**SEC filings** (from EDGAR submissions data):
- **RDW:** **Form 4.** CEO and Chairman Peter Cannito made an **open-market purchase** of 8,900 shares at **$5.73** on Nov 20, filed today at 16:09 ET. He now holds 833,040 shares directly. ([SEC](https://www.sec.gov/Archives/edgar/data/1819810/000181981026000146/xslF345X06/wk-form4_1795468158.xml)) **[VIEW]** The purchase is small (~$51K) but a bullish signal: the CEO bought on the breakdown day.
- **MRCY:** **S-3ASR filed Fri Nov 20 after the close** (16:02 ET). It is an automatic universal shelf: debt, preferred, common, warrants. No amount or ATM program is specified in the sections I read; terms are deferred to future prospectus supplements. The Plan of Distribution section was not reviewed. ([SEC](https://www.sec.gov/Archives/edgar/data/1049521/000104952126000101/s-3asr2026.htm))
  - Also a Form 144 today: officer Stuart Kupinsky, 1,000 shares (~$76K), restricted-stock vesting; it follows monthly sales of the same size. ([SEC](https://www.sec.gov/Archives/edgar/data/1049521/000195917326008201/xsl144X01/primary_doc.xml))
  - **[VIEW]** The shelf adds optional dilution supply. It was not flagged in the morning brief and modestly weakens the MRCY setup.
- **ANET:** Form 144. Director Charles Giancarlo plans to sell 20,000 shares (~$3.7M) from an option exercise, for a family trust. **[VIEW]** Routine; low materiality. ([SEC](https://www.sec.gov/Archives/edgar/data/1596532/000196858226001170/xsl144X01/primary_doc.xml))
- **CRWV:** Seven Form 144s (proposed insider sales) were filed late Friday, Nov 20. ([example](https://www.sec.gov/Archives/edgar/data/1769628/000195004726011418/xsl144X01/primary_doc.xml)) **[VIEW]** This is continuing insider supply into any bounce.

**Company news:**
- **MU, MRVL, CRWV, NBIS:** No company-specific material news. All moved on the Nvidia/Huang sector rebound. ([Motley Fool on MU](https://www.fool.com/investing/2026/11/23/why-nvidia-rehiring-jensen-huang-is-making-micron-stock-skyrocket-today/))
- **RKLB:** No material news. Today's articles rehash the Nov 9 Neutron price increase from $55M to $70M. ([Space.com](https://www.space.com/space-exploration/launches-spacecraft/theres-tremendous-demand-rocket-lab-raises-price-of-neutron-launch-from-usd55-million-to-usd70-million))
- **BKSY, ASTS, VELO, OUST, KRMN:** No material news.
- **Earnings today:** none on the watchlist.

---

### 4️⃣ Technical update (daily close vs. moving averages)

| Ticker | Close | SMA20 | SMA50 | SMA100 | SMA200 | RSI14 (Fri→Today) | MACD hist (Fri→Today) | ATR % |
|---|---|---|---|---|---|---|---|---|
| SPY | 722.56 | 745.67 (−3.1%) | 759.41 (−4.9%) | 759.18 (−4.8%) | 732.92 (−1.4%) | 24.9→41.6 | −5.38→−4.27 | 2.6% |
| QQQ | 651.18 | 675.48 (−3.6%) | 709.80 (−8.3%) | 710.07 (−8.3%) | 683.27 (−4.7%) | 26.6→42.2 | −4.76→−3.24 | 3.7% |
| SMH | 459.79 | 490.40 (−6.2%) | 545.87 (−15.8%) | 556.98 (−17.4%) | 525.46 (−12.5%) | 26.1→42.4 | −5.73→−3.22 | 7.2% |
| RKLB | 49.62 | 55.68 (−10.9%) | 61.08 (−18.8%) | 66.32 (−25.2%) | 77.60 (−36.1%) | 35.6→41.7 | −0.67→−0.73 | 11.8% |
| BKSY | 17.58 | 20.20 (−13.0%) | 20.40 (−13.8%) | 22.54 (−22.0%) | 26.94 (−34.7%) | 36.0→41.0 | −0.33→−0.45 | 11.9% |
| RDW | 6.415 | 7.61 (−15.7%) | 9.06 (−29.2%) | 9.87 (−35.0%) | 10.76 (−40.4%) | 30.2→38.5 | −0.12→−0.10 | 12.4% |
| ASTS | 25.67 | 33.52 (−23.4%) | 45.41 (−43.5%) | 54.97 (−53.3%) | 71.25 (−64.0%) | 27.6→33.1 | −0.51→−0.36 | 15.6% |
| MRVL | 144.57 | 166.59 (−13.2%) | 218.79 (−33.9%) | 217.55 (−33.5%) | 188.92 (−23.5%) | 27.9→38.5 | −1.57→−0.28 | 11.3% |
| **MU** | 707.84 | 776.86 (−8.9%) | 907.94 (−22.0%) | 917.76 (−22.9%) | 774.11 (−8.6%) | 29.5→42.5 | −9.67→−4.90 | 10.5% |
| VELO | 3.38 | 5.05 (−33.0%) | 7.51 (−55.0%) | 9.85 (−65.7%) | 12.56 (−73.1%) | 25.6→30.8 | −0.11→−0.07 | 19.5% |
| NBIS | 97.65 | 131.70 (−25.9%) | 179.01 (−45.4%) | 195.31 (−50.0%) | 179.81 (−45.7%) | 28.5→35.9 | −3.05→−2.21 | 19.3% |
| **CRWV** | 48.37 | 51.50 (−6.1%) | 67.30 (−28.1%) | 76.43 (−36.7%) | 87.79 (−44.9%) | 32.6→43.3 | **0.00→+0.31** | 14.5% |
| OUST | 27.88 | 32.01 (−12.9%) | 34.74 (−19.7%) | 37.09 (−24.8%) | 33.14 (−15.9%) | 33.0→42.3 | −0.78→−0.72 | 13.2% |
| MRCY | 76.22 | 78.09 (−2.4%) | 79.61 (−4.3%) | 89.07 (−14.4%) | 90.23 (−15.5%) | 41.6→47.2 | −0.28→−0.29 | 7.8% |
| **ANET** | 177.93 | 182.18 (−2.3%) | 191.82 (−7.2%) | 188.83 (−5.8%) | **168.78 (+5.4%)** | 41.5→46.6 | +0.26→−0.18 | 8.7% |
| KRMN | 30.335 | 38.17 (−20.5%) | 35.62 (−14.8%) | 42.40 (−28.5%) | 58.35 (−48.0%) | 35.9→38.3 | −1.27→−1.36 | 14.3% |

**Breakouts, breakdowns and level changes:**
- **[FACT]** Today's volume could not be measured, so no "on volume" claims are made for today.
- **MU** reclaimed **$650** (Nov 5 low) and closed 9% above it. **[VIEW]** This is a failed breakdown, the strongest technical repair on the list. $650–670 becomes support. Next resistance: the 200-DMA at $774 and the 20-DMA at $777.
- **CRWV:** MACD histogram turned positive (**bullish signal-line cross**); price reclaimed $40.6 and $46.9 (the old 5-day VWAP). The new 52-week low of $39.28 is the line in the sand. Resistance is the 20-DMA at $51.50; the intraday high of $51.90 stalled there.
- **ANET** reclaimed its **200-DMA** ($168.8) but faded from $187.21 to the session low. **[VIEW]** The intraday rejection at the 20/50-DMA cluster ($182–192) shows sellers are still active there.
- **MRVL** reclaimed $132.5 and $140.3; its MACD histogram is nearly flat (−0.28). **[VIEW]** Mechanically constructive, but the Dec 1 print decides.
- **OUST** (above $27.35) and **RDW** (above $6.06) reclaimed their broken pivots.
- **Gap-and-fade, bearish intraday:** NBIS (−11% from its open, closed at 13% of range), ANET (8%), BKSY (7%), KRMN (10%), ASTS (28%). **[VIEW]** Sellers used the gap to exit. Tuesday's open needs to hold today's lows (NBIS $95.80, BKSY $17.50, ASTS $25.03) or these round-trip.
- **Indices:** SPY reclaimed its Friday VWAP ($701.8) and is back near its 200-DMA ($732.9, −1.4%). QQQ is near its 5-day VWAP (~$650, per the morning brief).
  - **[VIEW]** Daily MACD histograms are still negative but contracting. RSIs reset from ~25 to ~42 in one session.

---

### 5️⃣ Plan for tomorrow (Tue Nov 24)

**Regime [VIEW]:** Relief rally into overhead supply.
- The first test is whether the market can **hold the gap**: SPY above ~$713.6 (today's low), QQQ above ~$642.
- A hold plus a higher low would make today a potential capitulation reversal; a fill back below Friday's VWAPs would put it back to breakdown.
- Keep size at **about half normal**; ATRs are still 8–20%.
- Do not buy the first 30–60 minutes after a gap.

| Ticker | Signal (vs. morning) | Entry zone | Stop | Targets | R:R | Condition / note |
|---|---|---|---|---|---|---|
| **MU** | **POTENTIAL BUY** (↑ from AVOID) | $655–675 retest | $612 (below the $650 shelf, minus ~0.5 ATR) | T1 $775 (200/20-DMA), T2 $830 | From $665: **2.1 / 3.1** | Only on a retest that holds $650 with a 1H higher low. At $708 (chase) the R:R is <1. Dell earnings Tue after the close is a read-through. |
| **BKSY** | **POTENTIAL BUY** (=) | $16.80–17.20 (holding Fri VWAP $16.94 / $17.04) | $15.85 (below the $16.09 shelf) | T1 $19.80, T2 $20.40 (50-DMA) | From $17.00: **2.4 / 2.9** | The close at 7% of range is a warning. A daily close below $16.09 invalidates. |
| **OUST** | **POTENTIAL BUY** (↑ from AVOID) | $27.00–27.50 (retest of $27.35) | $25.00 | T1 $32.00 (20-DMA), T2 $33.10 (200-DMA) | From $27.30: **2.0 / 2.5** | Needs the retest to hold $27.35 on a 1H close. |
| **RKLB** | **HOLD / MONITOR** (↓ from Potential Buy; zone missed) | $46.90–48.30 (gap-fill to Fri VWAP) | $43.40 (below the $43.89 Nov 5 low) | T1 $52.80, T2 $55.70 (20-DMA) | From $47.50: **1.3 / 2.0** | Below-par R:R. Alternative: a daily close above $52.20 (today's open and high) → momentum entry. |
| **MRVL** | **HOLD / MONITOR** (=) | none before Dec 1 | — | — | — | Earnings Dec 1 after the close. Post-print: a gap that holds above $140 is the signal. |
| **CRWV** | **HOLD / MONITOR** (↑ from AVOID) | speculative $44–46 if a higher 4H low forms | $39.00 | T1 $51.50, T2 $57.00 | From $45: ~1.0 / 1.7 | R:R is too thin. Debt (~$47B) and insider Form 144 supply are overhangs. Upgrade on a daily close above $51.90. |
| **RDW** | **HOLD / MONITOR** (↑ from AVOID) | speculative $6.06–6.25 on a retest | $5.55 (below Fri's low of $5.59) | T1 $7.60 (20-DMA) | From $6.15: **2.4** | The CEO's open-market buy is a plus. Small cap; ATR 12%. |
| **ANET** | **POTENTIAL BUY at $158–162 only** (=) | $158–162, or alternatively a daily close above $182.2 (20-DMA) | $151.50 | T1 $182, T2 $192 | From $160: **2.6 / 3.8** | Closed at the session low after rejecting the MA cluster. Dell read-through Tue. |
| **MRCY** | **HOLD / MONITOR** (↓ from Potential Buy) | $66–70 (pullback), or a daily close above $79.6 (50-DMA) | $63.00 | T1 $78.3, T2 $89.0 | From $68: 2.0 / 4.2 | The new S-3ASR shelf adds dilution optionality. |
| **KRMN** | **HOLD / MONITOR** (=) | a daily close above $30.50, then $30–31 | $27.00 | T1 $35.70, T2 $38.50 | From $30.5: 1.5 / 2.3 | Rejected at $31.56 and closed at 10% of range. |
| **ASTS** | **AVOID / HIGH RISK** (=) | — | — | — | — | Rejected just under the $27.58 reclaim level. Revisit on a daily close above $27.58. |
| **NBIS** | **AVOID / HIGH RISK** (=) | — | — | — | — | Worst gap-fade on the list. Revisit only on a daily close above $110. |
| **VELO** | **AVOID / HIGH RISK** (=) | — | — | — | — | Micro-cap downtrend. |

**R:R math [EST], from the stated entry:**
- **MU:** (775−665)/(665−612) = 2.1 on T1; T2 (830−665)/53 = 3.1.
- **BKSY:** (19.80−17)/(17−15.85) = 2.4.
- **OUST:** (32−27.3)/(27.3−25) = 2.0.
- **RKLB:** (52.8−47.5)/(47.5−43.4) = 1.3.
- **RDW:** (7.6−6.15)/(6.15−5.55) = 2.4.

**Key events Tue Nov 24 [FACT, per calendars]** ([Investrade](https://investrade.com/weekly-event-calendar-11-23-2026-11-27-2026/), [Newsquawk](https://newsquawk.com/headlines/newsquawk-weekly-economic-calendar---23rd-27th-november-2026)):
- **09:00 ET:** Case-Shiller home prices (Sep).
- **10:00 ET:** Conference Board Consumer Confidence (Nov) and Richmond Fed Manufacturing.
- **13:00 ET:** $70B 5-year note auction. **[VIEW]** Watch the tail; yields matter for long-duration growth names.
- **Before the open:** Analog Devices (ADI; semis read-through), Medtronic, Best Buy, Dollar Tree, Dick's, Burlington.
- **After the close:** **Dell** (AI-server demand: read-through for MU, CRWV, NBIS, ANET), HP, Workday, Autodesk, Ambarella, Nutanix.
- **Fed speakers:** none scheduled for Tuesday ([Fed calendar](https://www.federalreserve.gov/newsevents/2026-November.htm)).
- **Wed Nov 25:** October PCE / core PCE, Q3 GDP (second estimate), durable goods, $44B 7-year auction. **Thu Nov 26:** market closed. **Fri Nov 27:** half day.
- **Still ahead:** MRVL earnings Dec 1; FOMC decision Dec 9 (hike heavily priced, per the morning brief); MU earnings mid-Dec [EST].

---

### 🔑 Top takeaways

1. **[FACT]** It was a historic relief rally: S&P +4.7%, SOX +14%, NVDA +31.5% on Jensen Huang's reinstatement. **[VIEW]** But most watchlist names gapped and faded into the close (NBIS, BKSY, ANET, KRMN closed in the bottom 15% of the range). Tuesday has to hold today's lows before this counts as a bottom.
2. **[FACT]** **MU triggered its upgrade condition** by closing at $707.84, well above $650. The $650–660 entry zone never traded. **[VIEW]** Now a POTENTIAL BUY on a retest of $655–675, stop $612; do not chase $708.
3. **[FACT]** No morning setup filled: BKSY and RKLB gapped over their entry zones, and no stops were hit. OUST and RDW reclaimed their pivots, and RDW's CEO bought shares Friday at $5.73. MRCY filed a universal shelf (S-3ASR) on Friday evening. Dell reports Tuesday after the close; PCE is Wednesday.

*Limitations: today's consolidated volume and minute bars were not available on either data plan, so relative volume and 4H structure for today are not reported. Intraday open/high/low values come from Twelve Data's quote. Index % moves from news sources vary slightly; the ETF figures above are from candle data.*
