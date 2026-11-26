## 🌙 Post-Market Briefing: Thursday, November 26, 2026 (Thanksgiving)

> **US equity markets were CLOSED today (Thanksgiving).** There was no regular, pre-market or after-hours session.
> - **[FACT]** Massive `/v1/marketstatus/now` at 16:32 ET reports `nyse: closed, nasdaq: closed`. `/v1/marketstatus/upcoming` lists Nov 26 as *closed (Thanksgiving)*.
> - **Friday Nov 27 is a half session**: stocks close at **1:00 PM ET (20:00 Bucharest)**. Massive also lists the early close (18:00 UTC).
> - Next full session: **Monday Nov 30**.
>
> **Data provenance.** Every price below is from **Wed Nov 25, 2026**, the last session.
> - Source: Massive aggregates (flagged "DELAYED"), pulled 2026-11-26 ~21:35 UTC. Daily bars run from Sep 2025 to Nov 25, 2026. 1-minute bars are used for the after-hours prints.
> - I computed the indicators from those bars: SMA 20/50/100/200, RSI(14) using Wilder smoothing, and MACD(12,26,9). **RV** (relative volume) = Nov 25 volume ÷ the prior 20-day average.
> - The minute data confirms there are **0 bars dated Nov 26**.
>
> **Labels.** **[FACT]** means confirmed by data, a filing or a primary source. **[REPORTED]** means secondary coverage. **[EST]** means unconfirmed. **[OPINION]** means my analysis.
>
> **Not investment advice.**
>
> **Watchlist.** The 10 core names, plus the 3 extra candidates from this morning's brief (`reports/2026-11-26-market-intelligence.md`, on branch `claude/pensive-clarke-33whiy`): **KTOS, COHR, VSAT**.

---

### 1) Session recap: last session, Wed Nov 25 (no trading today)

Context: Nov 25 was a **sharp gap-down and full intraday reversal**.
- The indexes bottomed between 09:45 and 11:50 ET, then closed near their highs.
- After-hours (AH) extended the bounce. "AH" below is the last 1-minute print of the Nov 25 extended session (16:00–20:00 ET). AH volume is thin, so treat these prints as indicative.

| Ticker | Close | % chg | RV | High | Low | AH price (time ET) | AH vs close |
|---|---|---|---|---|---|---|---|
| SPY | 716.70 | -0.29% | 1.16 | 718.43 | 695.45 | 720.43 (19:59) | +0.5% |
| QQQ | 633.93 | -0.65% | 1.34 | 634.89 | 607.74 | 636.57 (19:59) | +0.4% |
| SMH | 422.46 | -1.01% | 1.05 | 422.97 | 393.88 | 428.00 (19:59) | +1.3% |
| RKLB | 47.02 | +2.26% | 1.05 | 48.16 | 42.12 | 48.26 (19:59) | +2.6% |
| BKSY | 15.97 | -2.68% | 1.19 | 16.65 | 14.62 | 16.13 (19:51) | +1.0% |
| RDW | 5.89 | -0.17% | 0.96 | 6.08 | 5.395 | 6.08 (19:59) | +3.2% |
| ASTS | 26.02 | +10.25% | 1.39 | 26.665 | 22.50 | 26.98 (19:59) | +3.7% |
| MRVL | 130.93 | -0.49% | 0.83 | 131.14 | 117.80 | 133.61 (19:59) | +2.0% |
| MU | 601.25 | -4.53% | 1.47 | 604.95 | 548.13 | 615.28 (19:59) | +2.3% |
| VELO | 3.165 | +5.50% | 0.81 | 3.30 | 2.75 | 3.19 (19:59) | +0.8% |
| NBIS | 84.99 | -2.66% | 1.25 | 87.26 | 75.60 | 88.24 (19:59) | +3.8% |
| CRWV | 42.57 | -0.08% | 1.15 | 43.02 | 37.40 | 43.56 (19:59) | +2.3% |
| OUST | 25.77 | +3.12% | 0.94 | 26.54 | 22.25 | 26.38 (19:58) | +2.4% |
| KTOS | 28.95 | +2.62% | 0.85 | 29.35 | 26.83 | 29.35 (19:59) | +1.4% |
| COHR | 196.19 | -0.03% | 0.88 | 199.92 | 174.96 | 202.42 (19:59) | +3.2% |
| VSAT | 61.01 | +0.91% | 0.54 | 62.28 | 55.55 | 61.50 (19:29) | +0.8% |

**[FACT]** Nov 25 index closes: S&P 500 7,183 (-0.25%), Nasdaq Composite 23,586 (-0.62%) ([Motley Fool recap](https://www.fool.com/coverage/stock-market-today/2026/11/25/stock-market-today-nov-25-nvidia-slides-3-9-as-the-market-considers-hot-pce-inflation-data-and-new-tariff-proposals/)).

**[OPINION]**
- The AH bid was broad: every watchlist name closed AH above its regular close.
- But it was thin, and a holiday gap of 1.5 days makes Friday's open the real test of whether the reversal holds.

---

### 2) This morning's setups: did anything trigger?

**No setup could trigger today because there was no session.** Status of each setup from the Nov 26 morning brief:

| Ticker | Morning signal | Zone / confirmation / stop | Status | Where price sits (Nov 25 AH) |
|---|---|---|---|---|
| RKLB | POTENTIAL BUY | Zone $44.0–46.5; confirm with a 4h close > $48.8 or a daily close > $50.7; stop $39.50 | **Not triggered** (market closed) | $48.26: above the zone, just under the $48.8 trigger |
| ASTS | POTENTIAL BUY (spec.) | Zone $24.5–26.0; confirm with a daily close > $28.50; stop $21.90 | **Not triggered** | $26.98: above the zone; the trigger is ~5.6% away |
| MRVL | POTENTIAL BUY (after earnings) | Wait for the Dec 1 print; zone $120–130; stop $112 | **Not triggered** (by design, pre-earnings) | $133.61 |
| KTOS | POTENTIAL BUY | Entry $27.5–29.0; confirm with a daily close > $29.75; stop $25.90 | **Not triggered** | $29.35: inside striking distance of the trigger |
| COHR | POTENTIAL BUY | Entry $180–190; confirm by holding > $175 or a daily close > $216; stop $166 | **Not triggered** | $202.42: above the zone; don't chase |
| VSAT | POTENTIAL BUY | Entry $58–61; confirm with a daily close > $64.20; stop $54.40 | **Not triggered** | $61.50: at the top of the zone |
| BKSY | HOLD / MONITOR | Re-evaluate on a close > $18.0 after Investor Day | **Not triggered** | $16.13 |
| MU | HOLD / MONITOR | Wait for a reclaim of $630 / a higher low > $548 | **Not triggered** | $615.28 |
| OUST | HOLD / MONITOR | Breakout only on a close > $28.75 | **Not triggered** | $26.38 |
| RDW, VELO, NBIS, CRWV | AVOID | — | **n/a** | — |

**Invalidated: none.** No stops were hit, and no targets were reached.

---

### 3) Earnings, filings and material news (Nov 25 after the close, and Nov 26)

**There were no earnings releases on the watchlist.** **[FACT]** EDGAR does not accept filings on federal holidays, so nothing was filed on Nov 26. I checked each EDGAR company feed for filings dated Nov 23 or later. I found **no 8-K, S-3, 424B or other ATM-related filing** for any watchlist name.

**Filings found (all routine unless noted):**

- **COHR – notable insider BUY [FACT].**
  - **Who and what:** a Form 4 filed Nov 25 by director **Stephen G. Pagliuca** reports **open-market purchases (code P)** on Nov 23–24.
  - **Size:** ~67.9k shares at $213.55–221.52 on Nov 23 and ~102.0k shares at $191.35–198.25 on Nov 24. That totals ~170k shares, roughly **$34–35M** (my calculation from the filing).
  - **Source:** [Form 4](https://www.sec.gov/Archives/edgar/data/820318/000089914026001413/0000899140-26-001413-index.htm).
  - **[OPINION]** This is a large director purchase into the drawdown, and a constructive signal for the COHR thesis.
- **RKLB [FACT].**
  - **Form 4s:** five filed Nov 25 (Klein, Kampani, Clevenger, Ricupati, Spice) report sales of ~105k shares in total on Nov 23 at $48.92–51.75. There are also two Form 144s filed Nov 25.
  - **Sources:** [example Form 4](https://www.sec.gov/Archives/edgar/data/1819994/000200101126000153/0002001011-26-000153-index.htm), [Form 144](https://www.sec.gov/Archives/edgar/data/1819994/000195004726011541/0001950047-26-011541-index.htm).
  - **[EST]** The identical price tiers across all five insiders look like coordinated sell-to-cover or plan sales rather than discretionary selling. The filings do not state this.
- **CRWV [FACT].** Multiple Form 4s filed Nov 24 show RSU conversions (code M) followed by sales at ~$42.28 on Nov 20, which is consistent with tax withholding ([example](https://www.sec.gov/Archives/edgar/data/1769628/000176962826000482/0001769628-26-000482-index.htm)). The Form 4s are routine; the credit overhang from the morning brief still stands.
- **BKSY [FACT].** An S-8 filed Nov 24 registers employee-plan shares, a minor dilution source ([S-8](https://www.sec.gov/Archives/edgar/data/1753539/000175353926000170/0001753539-26-000170-index.htm)).
- **MU [FACT].** The DEF 14A proxy and the Annual Report to Shareholders were filed Nov 24 ([index](https://www.sec.gov/Archives/edgar/data/723125/000072312526000034/0000723125-26-000034-index.htm)). These are routine.
- **ASTS, MRVL, RDW, VSAT [FACT].** Single routine Form 4s filed Nov 23–24.
- **VELO, OUST, KTOS, NBIS:** no new filings since Nov 23.

**News on Nov 26 (Massive `/v2/reference/news`, from Nov 24 21:00 UTC onward):**

| Ticker | News |
|---|---|
| RKLB | **No material news.** Only commentary: "[fell to its lowest price in about a year](https://www.fool.com/investing/2026/11/26/rocket-lab-stock-just-fell-to-its-lowest-price-in-about-a-year-is-it-a-buy-now/)" (Fool). **[REPORTED]** Sector context: SpaceX got FCC approval for 1 million satellites on Nov 25 ([Fool](https://www.fool.com/coverage/stock-market-today/2026/11/25/stock-market-today-nov-25-spacex-gets-historic-fcc-approval-for-1-million-satellites-is-this-its-next-growth-engine/)). |
| BKSY, ASTS, VELO, OUST, VSAT | **No material news.** |
| RDW | **No material news.** Only peer commentary on Planet Labs. |
| MRVL | **No material news.** Only Zacks/Fool pieces. One is [Credo "ahead of Q2 earnings"](https://www.zacks.com/stock/news/3035918/credo-technology-ahead-of-q2-earnings-how-to-approach-the-stock-now?cid=CS-ZC-FT-analyst_blog|most_popular_stocks-3035918), a read-across for AI connectivity. |
| MU | **No material news.** Commentary only, e.g. "[Micron and 6 other big names are down >50%](https://www.fool.com/investing/2026/11/25/micron-and-6-other-big-names-are-down-more-than-50-are-they-bargains-now/)". |
| NBIS | **No material news.** Commentary only: "[fell despite 571% revenue growth](https://www.fool.com/investing/2026/11/25/nebius-stock-fell-despite-571-revenue-growth-here-s-why/)". |
| CRWV | **No material news.** Commentary only: "[could soar 125% … after a PT cut](https://www.fool.com/investing/2026/11/25/coreweave-stock-could-soar-130-according-to-one-wall-street-analyst-even-after-a-price-target-cut-is-it-a-buy/)". The **[REPORTED]** ≥$4B chip-backed loan from the morning brief is still unpriced as far as I can find. |
| KTOS | **No material news.** |
| COHR | **No material news** beyond the Form 4 above. **[REPORTED]** It appeared on Zacks' "[New Strong Buy Stocks for Nov 26](https://www.zacks.com/commentary/3034910/new-strong-buy-stocks-for-november-26th?cid=CS-ZC-FT-zacks_1_rank_additions-3034910)" list. |

**Macro (unchanged from the morning brief) [FACT]:**
- October PCE: headline 3.8% annualized, core 3.3% y/y.
- About **98% odds of a 25 bp hike at the Dec 8–9 FOMC**.
- Proposed 20–40% tariffs on 14 economies.
- Sources are linked in the morning brief.

---

### 4) Technical update (daily, as of the Nov 25 close; nothing changed today)

| Ticker | Close | SMA20 | SMA50 | SMA100 | SMA200 | RSI14 | MACD hist (prev) | 1-mo | Read |
|---|---|---|---|---|---|---|---|---|---|
| SPY | 716.70 | 740.33 | 757.89 | 758.54 | 733.16 | 39.8 | -2.92 (-3.53) | -6.9% | Below all SMAs. The 695 low held above the 20-day low of 686.75. |
| QQQ | 633.93 | 666.73 | 707.05 | 708.46 | 683.50 | 38.6 | -2.50 (-2.81) | -12.1% | 607.74 low vs the 606.23 Nov 20 low: a retest held. Needs a close > ~657.5. |
| SMH | 422.46 | 476.59 | 541.11 | 553.62 | 525.65 | 36.9 | -3.27 (-3.33) | -24.3% | **New 20-day low of 393.88**, then a long lower wick. |
| RKLB | 47.02 | 54.48 | 60.40 | 65.48 | 77.33 | 39.8 | -0.95 (-0.95) | -19.4% | Hammer above the 52-week low of 39.98. Momentum is flat. |
| BKSY | 15.97 | 19.90 | 20.19 | 22.34 | 26.86 | 36.8 | -0.65 (-0.58) | -16.6% | **Breakdown: new 52-week low of 14.62.** MACD still falling. |
| RDW | 5.89 | 7.30 | 8.86 | 9.77 | 10.72 | 35.4 | -0.10 (-0.11) | -33.7% | Downtrend; 5.12 is the 52-week low. |
| ASTS | 26.02 | 31.79 | 44.04 | 53.92 | 70.50 | 36.3 | -0.08 (-0.32) | -38.0% | Triple bottom ~22.5 plus a +10% engulfing candle on RV 1.39. The MACD histogram is nearly flat. |
| MRVL | 130.93 | 154.96 | 215.01 | 215.38 | 189.41 | 35.1 | **+0.23 (-0.07)** | -46.2% | **Bullish daily MACD histogram cross.** Double-bottom area 117.8–120.6. |
| MU | 601.25 | 742.80 | 895.48 | 910.84 | 776.48 | 35.7 | -7.77 (-6.09) | -35.3% | **Lower low (548.13 < 585.25)** on RV 1.47. Momentum is worsening. |
| VELO | 3.165 | 4.66 | 7.23 | 9.63 | 12.46 | 30.9 | -0.02 (-0.05) | -54.0% | **New 52-week low of 2.75.** RSI is near oversold. |
| NBIS | 84.99 | 122.68 | 174.12 | 192.95 | 179.74 | 33.1 | -1.76 (-2.03) | -50.1% | **Lower low of 75.60**, near the 52-week low of 73.52. |
| CRWV | 42.57 | 49.59 | 65.72 | 75.58 | 87.26 | 38.9 | +0.13 (+0.17) | -28.5% | **New 52-week low of 37.40**, then a reversal. |
| OUST | 25.77 | 31.23 | 34.42 | 36.66 | 33.18 | 39.9 | -0.78 (-0.82) | -21.4% | Undercut the 23.60 low (22.25), then reversed. |
| KTOS | 28.95 | 34.26 | 39.23 | 45.53 | 57.45 | 32.7 | -0.42 (-0.58) | -29.9% | Higher low: 26.83 vs the 26.60 52-week low. MACD improving. |
| COHR | 196.19 | 208.74 | 251.75 | 274.57 | 296.09 | 43.1 | +1.18 (+1.62) | -16.8% | MACD histogram positive but fading. Strongest RSI in the AI group. |
| VSAT | 61.01 | 67.58 | 68.31 | 71.56 | 65.92 | 43.6 | -0.97 (-1.13) | -13.2% | Double bottom 55.53/55.55. Light volume (RV 0.54). |

**Levels that changed versus the prior brief: none.** No session was held, so no new highs, lows or SMA values.
- **[OPINION]** The Nov 25 AH prints suggest RKLB ($48.8), KTOS ($29.75) and VSAT ($64.2) could test their confirmation levels early on Friday.
- Holiday half-sessions have thin volume. **A trigger on volume below average should be treated as unconfirmed.**

---

### 5) Plan for tomorrow (Fri Nov 27, half session: 9:30 AM – 1:00 PM ET / 16:30–20:00 Bucharest)

**Overall stance [OPINION]:** **WAIT / small starters only.**
- The regime is still bearish: QQQ and SMH are below every SMA, and a Fed hike is ~98% priced.
- Half sessions have low liquidity and can produce false breakouts. **Prefer acting on Monday Nov 30 confirmation** unless a trigger comes with clearly above-average volume.

| Ticker | Signal | Entry zone | Confirmation | Stop | T1 / T2 | Note |
|---|---|---|---|---|---|---|
| **KTOS** | POTENTIAL BUY | $27.5–29.0 | Daily close > $29.75 | $25.90 | $34.30 / $39.20 | Best R/R. Nov 25 AH reached $29.35, so the trigger is close. |
| **ASTS** | POTENTIAL BUY (spec.) | $24.5–26.0 (pullback only) | Daily close > $28.50 on RV > 1 | $21.90 | $31.80 / $38.00 | Don't chase an AH-driven gap above $27. |
| **RKLB** | POTENTIAL BUY | $44.0–46.5 | Close > $48.8 (4h) or > $50.7 (daily) | $39.50 | $54.50 / $60.40 | Insider Form 4 sales look routine [EST]. |
| **MRVL** | POTENTIAL BUY (post-earnings) | $120–130 after the print, or breakout > $150 | Dec 1 earnings reaction | $112 | $155 / $175 | **No new position before Dec 1 (Tue, after the close).** |
| **COHR** | POTENTIAL BUY | $180–190 (pullback) | Hold > $175 or a close > $216 | $166 | $215 / $247 | **Upgraded conviction [OPINION]** on the ~$34M director open-market buy. Don't chase above ~$205. |
| **VSAT** | POTENTIAL BUY | $58–61 | Daily close > $64.20 | $54.40 | $67.60 / $75.00 | Needs volume. |
| BKSY | HOLD / MONITOR | Re-assess after Investor Day | Close > $18.0 | $14.4 | — | Investor Day Wed Dec 2. |
| MU | HOLD / MONITOR | — | Higher low > $548 and a reclaim of $630 | — | — | AH reached $615. Earnings ~Dec 16–17 [EST]. |
| OUST | HOLD / MONITOR | $27.5–28 retest | Close > $28.75 | $24.4 | $31.2 / $34.4 | — |
| RDW | AVOID | — | Close > $6.60 to revisit | — | — | — |
| VELO | AVOID | — | — | — | — | Microcap with dilution risk. |
| NBIS | AVOID | — | Close > $100 to revisit | — | — | — |
| CRWV | AVOID | — | — | — | — | Credit stress; the loan pricing is pending. |

**Key events:**

- **Fri Nov 27:**
  - US stocks close early at 1:00 PM ET; bond markets at 2:00 PM ET [REPORTED, per SIFMA guidance].
  - No watchlist earnings.
  - **[EST]** No tier-1 US macro releases and no scheduled Fed speakers found. Black Friday retail headlines are possible.
- **Sat Nov 28 [EST]:** Under the standard rule (the second Saturday before the meeting), the **FOMC blackout for Dec 8–9 should begin**. That means no Fed speakers from then until the decision.
- **Next week:**
  - **MRVL Q3 FY27 earnings, Tue Dec 1, after the close** [FACT, per the IR notice linked in the morning brief].
  - **BKSY Investor Day, Wed Dec 2, 8:00 AM EST** [FACT].
  - Credo (CRDO) earnings this coming week [REPORTED, date unconfirmed]. It is a read-across for MRVL and COHR.
  - ISM Manufacturing ~Dec 1 [EST].
  - November jobs report ~Fri Dec 4 [EST].

---

### 🔑 Top takeaways

1. **No session today (Thanksgiving).** Nothing triggered and nothing was invalidated. Friday is a 1 PM ET half session, and the Nov 25 after-hours bid (SMH +1.3%, NBIS +3.8%, ASTS +3.7%) faces its first test there.
2. **The most important new fact: a COHR director bought ~170k shares (~$34–35M) in the open market on Nov 23–24** (Form 4 filed Nov 25). It supports the COHR candidate, but price ($202 AH) is above the $180–190 entry zone.
3. **KTOS and RKLB are closest to their confirmation levels** ($29.75 and $48.8 respectively). The **binary event that matters next is MRVL earnings on Dec 1**. Keep exposure light until QQQ closes above ~657.5.

*Data: Massive aggregates, market status and news (delayed), pulled 2026-11-26 ~21:35 UTC. SEC EDGAR company feeds. Twelve Data was not needed. I did not invent any prices; every price is from the Nov 25 session.*
