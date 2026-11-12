## 🌙 Post-Market Briefing: Thursday, November 12, 2026

**Data notes (please read first)**
- **Retrieved:** 2026-11-12, 21:32–21:41 UTC (23:32–23:41 Bucharest; 16:32–16:41 ET).
- **Today's prices are provisional.** Massive (Polygon) does not release same-day bars on this plan ("today's data before end of day" is refused), so today's open/high/low/close come from **Twelve Data**. Its close is the last regular-session print (15:59 ET bar), not the official closing-auction price. One cross-check: a media quote shows MU at $798.44 against $798.90 here, so expect differences of a few cents to ~0.1%.
- **History:** daily candles through Nov 11 are from Massive. All % changes are today's provisional close vs. the Massive Nov 11 close.
- **Relative volume for today is NOT available.** The Twelve Data same-day volume is unreliable (e.g. 346K for RKLB against a 21M average; 78.7M for MU where a media quote shows 26.8M). I left it out instead of printing a wrong number. The table shows yesterday's confirmed relative volume for context only. Any "on volume" judgment for today is therefore **pending**.
- **After-hours:** from the Twelve Data extended quote, with its own timestamp. Where the feed had no post-close print, it says so.
- **Indicators:** computed by me from the candles: SMA 20/50/100/200, RSI(14, Wilder), MACD(12,26,9). They include today's provisional close.
- **Morning brief:** setups are checked against `reports/2026-11-12-market-intelligence.md`, which sits on branch `claude/pensive-clarke-lmhof9` (not on this branch).
- **Labels:** **[Confirmed]** = SEC filing or company release. **[Reported]** = media. **[Est.]** = unconfirmed. **Opinion** = my analysis. Not personalised financial advice.

---

### 🧭 The day in three lines
1. **NVIDIA CEO Jensen Huang resigned, effective immediately [Confirmed].** CFO Colette Kress is interim CEO; NVDA still reports **Tue Nov 17** ([NVIDIA 8-K](https://www.sec.gov/Archives/edgar/data/0001045810/000104581026000082/nvidiaannouncesceotransiti.htm)). AI names gapped down hard at the open, then recovered most of it.
2. **Nebius fell 16.8%** after a revenue beat but a delayed ARR target, 2026 revenue at the low end, and higher capex [Confirmed, 6-K].
3. **Every watchlist name closed red**, but the semis held key supports: MU held its 200 DMA, QQQ closed back above its 200 DMA after undercutting it. Five morning setups triggered on the opening dip.

---

### 1. Session recap

| Ticker | Close (prov.) | % chg | High | Low | After-hours (ET) | Rel. vol Nov 11 (context) |
|---|---|---|---|---|---|---|
| **SPY** | 757.19 | -0.34% | 763.04 | 753.67 | 758.06 @ 16:35 | 0.79 |
| **QQQ** | 688.20 | -0.32% | 694.52 | 679.94 | 689.35 @ 16:34 | 0.87 |
| **SMH** | 501.91 | -1.00% | 509.87 | 484.74 | no post-close print | 1.27 |
| RKLB | 64.10 | -3.11% | 66.70 | 63.71 | 64.50 @ 16:30 | 1.14 |
| BKSY | 23.24 | -3.57% | 24.23 | 22.18 | no post-close print | 1.11 |
| RDW | 8.03 | -4.46% | 8.38 | 7.92 | no post-close print | 0.81 |
| ASTS | 34.48 | -5.84% | 36.47 | 34.45 | 34.38 @ 16:33 | 0.97 |
| MRVL | 164.48 | -2.56% | 169.58 | 155.97 | 164.68 @ 16:11 | 1.14 |
| MU | 798.90 | -1.53% | 799.70 | 764.57 | 804.69 @ 16:34 | 1.19 |
| VELO | 4.41 | -10.00% | 4.86 | 4.35 | no post-close print | 2.63 |
| NBIS | 128.73 | -16.78% | 132.69 | 118.81 | 130.00 @ 16:34 | 1.61 |
| CRWV | 56.59 | -6.89% | 58.56 | 50.17 | 57.00 @ 16:30 | 2.27 |
| OUST | 36.60 | -4.24% | 38.43 | 36.15 | no post-close print | 0.70 |
| ALAB | 227.89 | -1.31% | 234.20 | 211.65 | no post-close print | 0.81 |
| KTOS | 34.75 | -5.29% | 36.90 | 34.67 | no post-close print | 0.93 |
| PL | 13.90 | -3.10% | 14.43 | 13.75 | no post-close print | 0.73 |

- **Shape of the day:** almost every name made its low in the first 30 minutes (09:30–10:00 ET) and its high around 11:00–11:15 ET, then drifted lower into the close. ASTS, KTOS and VELO closed at or near their lows.
- **Indices [Reported]:** S&P 500 about -0.3% to -0.4%, Nasdaq Composite about -0.5% to -0.7% (sources differ on exact closes). NVDA fell roughly 4–5% after being down as much as 14% early. Bond yields rose on December rate-hike odds ([Yahoo Finance](https://finance.yahoo.com/markets/live/stock-market-today-thursday-november-12-sp-500-nasdaq-dow-nvidia-invest-110027430.html), [CNBC](https://www.cnbc.com/2026/11/11/stock-market-today-live-updates.html), [24/7 Wall St.](https://247wallst.com/cards/rate-hike-odds-are-doing-the-damage-and-the-nasdaq-s-0-61-gspc-market-bell-01m78s60347w0kk4y4pfd5e2p6)).
- **After-hours:** small and positive where prints exist (MU +0.7%, CRWV +0.7%, NBIS +1.0%, RKLB +0.6% vs. the provisional close). No after-hours shock.

---

### 2. Morning setups: what happened

| Ticker | Morning plan | Result | Detail |
|---|---|---|---|
| **MU** | Buy $765–785, confirm 4h close > $790, stop $695 | ✅ **TRIGGERED** | Low $764.57 at ~10:00 ET tagged the 200 DMA ($763.90). The 09:30–13:30 4h bar closed $796.25. Stop and targets untouched. |
| **ALAB** | Buy $207–218 on a 4h higher low, stop $194 | ✅ **TRIGGERED** | Low $211.65 at the open (higher low vs. $207.32 on Nov 10). 4h bar $215.50 → $230.05. |
| **OUST** | Buy $35.50–36.50, confirm 50 DMA holds and 1h recovers $37, stop $33.40 | ✅ **TRIGGERED, weak close** | Low $36.15, 50 DMA ($35.65) held, hourly closes above $37 from 10:30 to 13:30 ET. Then faded to $36.60, back under $37. |
| **BKSY** | Buy $21.75–23.00, confirm 100 DMA/gap holds with a 1h higher low, stop $19.80 | ✅ **TRIGGERED** | Low $22.18 (10:30–11:00 ET), above the $21.4–21.5 gap. Hourly higher lows after that; closed $23.24, above the 100 DMA ($22.99). |
| **PL** | Buy $13.30–13.80 if the 20 DMA holds, stop $12.30 | ✅ **TRIGGERED (marginal)** | Low $13.75, only the top 5 cents of the zone. 20 DMA ($13.55) held. Closed $13.90, near the day's low. |
| **MRVL** | Possible: higher low at $148–156 with a bullish 4h reversal, stop $138 | ⚠️ **TRIGGERED (marginal)** | Low $155.97, 3 cents inside the zone, then a 4h bar of $157.46 → $166.05. Morning signal was only HOLD/MONITOR. |
| **CRWV** | Buy $54.50–57.00, confirm $53.80 holds on lighter volume, stop $49.50 | ❌ **NOT TRIGGERED: confirmation failed** | Gapped to $50.89 and hit $50.17, straight through $53.80. Stop $49.50 was **not** hit (missed by $0.67). Recovered to close $56.59, back above the 20 DMA. |
| **RKLB** | Buy $61.50–63.50, stop $56.50 | ⏸ **NOT TRIGGERED** | Low $63.71, $0.21 above the zone. Inside day. |
| **NBIS** | Bull: hold > $160 first hour. Bear: gap below $134 → stand aside until $113–120 holds | 🛑 **BULL CASE INVALIDATED; bear case triggered** | Opened $119.88, never traded above $132.69. Low $118.81 sat inside the $113–120 zone and held for day one. |
| **RDW** | Trigger: daily close > $9.70 | ⏸ **NOT TRIGGERED** | Closed $8.03, back below the 20 DMA ($8.19). |
| **ASTS** | Trigger: daily close > $40 | ⏸ **NOT TRIGGERED** | Closed $34.48, at the day's low. |
| **KTOS** | Trigger: daily close > $39.20 | ⏸ **NOT TRIGGERED** | Closed $34.75, at the day's low. |
| **VELO** | No trade | — **AVOID stands** | Another -10% to $4.41; low $4.35. |

**No stop and no target was hit on any setup today.** Opinion: the triggered names were all bought on a news-driven gap down that reversed, which is a decent sign, but four of the six closed in the lower half of their range. Treat them as half-size until they hold tomorrow.

---

### 3. Earnings, filings and material news (Nov 12, incl. after-hours)

**Market-wide**
- **NVIDIA [Confirmed]:** Jensen Huang resigned as President, CEO and director, effective immediately. Colette Kress is interim CEO and stays CFO. Harvey C. Jones becomes the first board chair. A CEO search will consider internal and external candidates. Q3 FY27 results stay on **Tue Nov 17, ~1:20 pm PT** ([8-K](https://www.sec.gov/Archives/edgar/data/0001045810/000104581026000082/nvidiaannouncesceotransiti.htm)). Media link the exit to personal-conduct scrutiny and report the board pushed him out [Reported, conflicts with the "resigned" wording] ([CNBC](https://www.cnbc.com/2026/11/12/nvidia-jensen-huang-ceo-live-updates.html), [TechCrunch](https://techcrunch.com/2026/11/12/jensen-huang-is-out-at-nvidia-who-is-colette-kress-his-interim-replacement/)).

**NBIS: Q3 results [Confirmed, 6-K furnished before the open]** ([shareholder letter, Ex. 99.2](https://www.sec.gov/Archives/edgar/data/1513845/000110465926126008/tm2629571d1_ex99-2.htm))
- Revenue **$980.8M** (+571% YoY, +68% QoQ); consensus was ~$907M [Est.]. About **$325M was non-recurring** asset-light revenue.
- Adjusted EBITDA $465.8M (47% margin). ARR **$6.4B** at end of September. Cash $7.4B.
- **Negatives:** 2026 revenue now at the **low end of $3.0–3.4B**. ARR above $7B is pushed from December to **February 2027** (third-party capacity slipped to 1H 2027). 2026 capex raised to **~$27B** from $20–25B. About **$1.0B was raised through the ATM in Q3**.
- **2027 outlook:** revenue $12–13B, capex $40–45B, pre-tax breakeven in Q4 2027.
- A second 6-K with the interim financial statements was filed at 21:10 UTC ([6-K](https://www.sec.gov/Archives/edgar/data/1513845/000110465926126238/nbis-20261112x6k.htm)). No offering announced.

**CRWV**
- 10-Q for Q3 filed this morning [Confirmed] ([10-Q](https://www.sec.gov/Archives/edgar/data/1769628/000176962826000465/crwv-20260930.htm)).
- Planning an investment-grade loan of **at least $4B**, backed by chips and customer contracts, possibly next week; management guided to a 7–7.5% yield [Reported: Bloomberg via [Yahoo/StockTwits](https://finance.yahoo.com/markets/stocks/articles/coreweave-reportedly-plans-4b-investment-002640650.html), published Nov 11 evening].
- NVIDIA owns more than 10% of CoreWeave, which is why the Huang news hit it harder [Reported] ([Yahoo Finance](https://finance.yahoo.com/markets/stocks/article/coreweave-stock-sinks-as-resignation-of-jensen-huang-ripples-through-ai-trade-180319031.html)).

**MRVL**
- 8-K, Item 5.02 [Confirmed]: board expanded from 7 to 10. New independent directors effective Nov 12: Donna Morris (Walmart), Douglas Bettinger (Lam Research CFO), Sasan Goodarzi (Intuit CEO) ([8-K](https://www.sec.gov/Archives/edgar/data/1835632/000183563226000026/mrvl-20261111.htm)). Not price-moving (opinion).

**MU**
- Two Form 144 notices [Confirmed]: officer Sumit Sadana, 14,000 shares (~$11.4M) each, sale date Nov 11 ([144](https://www.sec.gov/Archives/edgar/data/723125/000195004726011002/xsl144X01/primary_doc.xml), [144](https://www.sec.gov/Archives/edgar/data/723125/000195004726011000/xsl144X01/primary_doc.xml)). I could not tell whether the second is a duplicate. Small relative to the float.
- The drop was read-through from NVIDIA, with no company news [Reported] ([Motley Fool](https://www.fool.com/investing/2026/11/12/why-micron-stock-dropped-on-thursday/)).

**OUST**
- Form 4 [Confirmed]: director Susan Heystee sold 7,551 shares at ~$37.44 on Nov 10, "for tax planning purposes"; 33,707 shares held after ([Form 4](https://www.sec.gov/Archives/edgar/data/1816581/000119312526458398/xslF345X06/ownership.xml)). Minor.

**RKLB, BKSY, RDW, ASTS, VELO, ALAB, KTOS, PL:** **No material news.** No 8-K, Form 4, S-3 or ATM filing on EDGAR for any of them on Nov 11–12 (checked at 21:35 UTC). Only commentary pieces appeared (e.g. [Zacks on RKLB's ESCAPADE](https://www.zacks.com/stock/news/3028394/can-rklb-s-escapade-mission-strengthen-its-deep-space-capabilities)).

---

### 4. Technical update (daily, includes today's provisional close)

| Ticker | Close | 20 DMA | 50 DMA | 100 DMA | 200 DMA | RSI(14) | MACD histogram |
|---|---|---|---|---|---|---|---|
| SPY | 757.19 | 759.47 ↓ | 764.81 ↓ | 760.07 ↓ | 731.62 ↑ | 48.5 | -0.28 (improving) |
| QQQ | 688.20 | 696.95 ↓ | 718.62 ↓ | 714.76 ↓ | 681.99 ↑ | 45.4 | -0.53 (improving) |
| SMH | 501.91 | 520.80 ↓ | 561.12 ↓ | 568.91 ↓ | 523.54 ↓ | 43.1 | -1.28 (improving) |
| RKLB | 64.10 | 55.24 ↑ | 62.51 ↑ | 69.09 ↓ | 78.40 ↓ | 56.3 | +1.81 (rising) |
| BKSY | 23.24 | 19.12 ↑ | 20.49 ↑ | 22.99 ↑ | 27.01 ↓ | 61.9 | +0.86 (flat) |
| RDW | 8.03 | 8.19 ↓ | 9.61 ↓ | 10.20 ↓ | 10.90 ↓ | 45.2 | +0.09 (flat) |
| ASTS | 34.48 | 38.21 ↓ | 50.29 ↓ | 58.61 ↓ | 74.06 ↓ | 39.0 | +0.35 |
| MRVL | 164.48 | 198.30 ↓ | 230.25 ↓ | 226.71 ↓ | 186.62 ↓ | 37.2 | -3.38 (improving) |
| MU | 798.90 | 843.05 ↓ | 947.38 ↓ | 945.70 ↓ | 763.90 ↑ | 44.1 | -4.24 (improving) |
| VELO | 4.41 | 6.17 ↓ | 8.56 ↓ | 10.81 ↓ | 12.91 ↓ | 30.4 | 0.00 (rolling over) |
| NBIS | 128.73 | 153.61 ↓ | 196.50 ↓ | 205.58 ↓ | 179.25 ↓ | 38.7 | +0.20 (fading) |
| CRWV | 56.59 | 55.40 ↑ | 73.22 ↓ | 79.68 ↓ | 89.22 ↓ | 46.0 | +1.26 (rising) |
| OUST | 36.60 | 32.03 ↑ | 35.65 ↑ | 38.56 ↓ | 32.82 ↑ | 54.6 | +1.10 (flat) |
| ALAB | 227.89 | 250.17 ↓ | 295.49 ↓ | 315.01 ↓ | 257.16 ↓ | 41.1 | -1.02 (improving) |
| KTOS | 34.75 | 38.67 ↓ | 42.40 ↓ | 47.35 ↓ | 60.48 ↓ | 36.9 | -0.17 (worsening) |
| PL | 13.90 | 13.55 ↑ | 15.47 ↓ | 19.68 ↓ | 26.10 ↓ | 47.1 | +0.26 (flat) |

↑ = close above the average, ↓ = close below.

**Breakouts / breakdowns and levels that changed**
- **NBIS: breakdown.** Lost the 20 DMA with a 22% opening gap. New resistance is the gap: **$132.7** (today's high), then $134–137, then $147.4 (Nov 11 low, gap top). Support: **$118.8** (today's low), then $113.3 (Nov 5 low). Volume confirmation pending.
- **VELO: breakdown continues.** New low for the move at $4.35 (previous low $4.53). Next support is the 52-week low at $4.02. RSI 30.
- **CRWV: gap fully tested, breakout not broken.** It gave back all of yesterday's gap intraday (low $50.17 vs. Nov 10 high $51.02) yet closed above the 20 DMA ($55.40). New key support: **$50.2**. Resistance: $58.6 (today's high), then $62.0.
- **MU: 200 DMA defended.** Low $764.57 against the 200 DMA at $763.90 and the Nov 11 low at $763.05. That zone ($763–765) is now the line in the sand. Resistance: $800 (today's high), $827.6, then the 20 DMA at $843.
- **QQQ: undercut and reclaimed the 200 DMA** ($681.99; low $679.94). A daily close below ~$680 would be a new negative.
- **SMH:** still below its 200 DMA ($523.54); low $484.74 held above the Nov 10 area. Correction not over.
- **MRVL:** filled the Nov 11 gap (low $155.97 vs. Nov 10 high $158.60) and bounced. Support $156, then $147.8. Resistance $169.6, then $174.5.
- **RKLB:** inside day above the 50 DMA ($62.51). 100 DMA resistance moved to **$69.09**.
- **OUST:** first test of the 50 DMA ($35.65) from above held. Resistance $38.4, then $40.4.
- **RDW:** slipped back under the 20 DMA ($8.19). Support $7.92, then $6.06.
- **ASTS / KTOS:** closed at the lows. ASTS support $32–33.7; KTOS support $31.6–32.5.
- **No watchlist name broke out to the upside today.**

---

### 5. Plan for tomorrow (Fri Nov 13)

Levels are opinion. "Open" means the morning setup triggered today on paper; I do not know whether you took it.

| Ticker | Signal | Entry zone / trigger | Stop | Targets | Note |
|---|---|---|---|---|---|
| **MU** | 🟡 **POTENTIAL BUY (setup open)** | Fresh entries only on a retest of $770–790 that holds; no chase above $830 | $695 (tighter option: daily close below $760) | $870 / $950 | Best-behaved large cap today. |
| **ALAB** | 🟡 **POTENTIAL BUY (setup open)** | $212–222 on a pullback that holds above $211.6 | $194 | $257 / $295 | Needs NVDA (Nov 17) to cooperate. |
| **OUST** | ⏳ **SETUP OPEN, needs follow-through** | $35.65–36.50 while the 50 DMA holds; add only on an hourly close back above $37.20 | $33.40 | $42 / $46 | Weak close. A daily close below $35.60 downgrades it. |
| **BKSY** | ⏳ **SETUP OPEN** | $22.20–23.00 | $19.80 | $27.00 / $29.00 | Must stay above the 100 DMA ($22.99) on a closing basis. |
| **PL** | 🟡 **POTENTIAL BUY (marginal fill)** | $13.30–13.80, better lower in the zone | $12.30 | $17.00 / $19.70 | Closed near the low; a close below $13.55 weakens it. |
| **MRVL** | 👀 **HOLD / MONITOR** | Higher low at $150–158 that holds | $138 | $186 / $198 | Deal-arbitrage overhang; earnings Dec 1. |
| **CRWV** | ⏳ **WAIT, reset** | $54.5–57.0 only after a session that holds above $55.0 (20 DMA / afternoon low) | $49.50 (below today's $50.17 low) | $62.0 / $69.5 / $73.2 | Confirmation failed today. Loan launch (reported, next week) is the catalyst. |
| **RKLB** | ⏳ **WAIT FOR RETEST** | $61.50–63.50 (unchanged) | $56.50 | $69.00 / $78.00 | Missed the zone by $0.21 today. |
| **NBIS** | 🛑 **STAND ASIDE** | No entry. Reconsider only after 2–3 sessions holding $118.8 **and** a daily close above $134.8 | n/a | First resistance $132.7–137, then $147–154 | Guidance cut plus ATM usage; a close below $113.3 opens a new leg down. |
| **RDW** | 👀 **HOLD / MONITOR** | Daily close above $9.70 (unchanged) | $8.40 on that trade | $10.90 / $12.60 | Weakening; below $7.92 look for $7.0 then $6.06. |
| **ASTS** | ⛔ **AVOID / HIGH RISK** | Daily close above $40 (unchanged) | $34.50 on that trade | $45 / $50.3 | Closed at the low. |
| **KTOS** | 👀 **HOLD / MONITOR** | Daily close above $39.20 (unchanged), or a reversal candle at $31.6–32.5 | $34.80 on the breakout trade | $44 / $47.5 | Drifting to support. |
| **VELO** | ⛔ **AVOID** | None | n/a | n/a | Revisit only after a base above $4.02 and a reclaim of $6.20. |

**Key events**
- **Fri Nov 13, 8:30 am ET (15:30 Bucharest): October PPI.** Most calendars show 8:30 ET; a couple list a different time, so confirm on the BLS site. Consensus about +0.3–0.4% m/m [Est.] ([fedratecalc](https://fedratecalc.com/us-economic-calendar/november-2026/), [Scotiabank](https://www.scotiabank.com/ca/en/about/economics/economics-publications/post.other-publications.calendar-of-economic-release-dates.calendar-of-economic-release-dates--november-2026-.html)). A hot print feeds December-hike pricing and hurts CRWV, NBIS, ASTS most.
- **Fed speakers Fri [Reported, single source, times unverified]:** Collins, Logan, Bowman, Daly, Jefferson ([Investing.com](https://uk.investing.com/news/stock-market-news/ppi-data-highlights-fridays-economic-calendar-93CH-4978607)).
- **Watchlist earnings tomorrow:** none that I found.
- **Next week:** retail sales and **NVIDIA earnings on Tue Nov 17**, now the first report under an interim CEO. Possible CoreWeave loan launch [Reported]. MRVL reports Dec 1.

**Stance (opinion):** keep half size. The opening flush was bought, which is constructive, but SMH is still below its 200 DMA, closes were soft, and tomorrow's PPI plus Tuesday's NVIDIA report are both binary. Do not add to anything that closes below today's low.

---

*Sources are linked inline. Today's prices are provisional Twelve Data values; history is from Massive. Facts are labeled; levels, signals and the stance are opinion, not personalised investment advice.*
