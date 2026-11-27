## 🌙 Post-Market Briefing: Friday, November 27, 2026 (Black Friday half day)

**Prepared:** ~23:30–00:15 Bucharest (21:30–22:15 UTC). The regular session closed early at **13:00 ET (18:00 UTC)**.

**Morning plan graded below:** [reports/2026-11-27-market-intelligence.md](https://github.com/kapi-5678/site/blob/claude/pensive-clarke-m413xa/reports/2026-11-27-market-intelligence.md), on branch `claude/pensive-clarke-m413xa`.

**Price data:**
- **Today's OHLC and hourly bars** are from Twelve Data, retrieved 21:35–21:50 UTC.
  - Massive (Polygon) returned `NOT_AUTHORIZED` for today's `/v1/open-close` and today's minute bars, because the plan has no same-day data.
- **History through Wed Nov 25** is from Massive daily candles.
- Previous closes match across both feeds (e.g. MU $601.25, SPY $716.70).
- SMA 20/50/100/200, RSI(14, Wilder), MACD(12,26,9) and ATR(14) are computed in-house on that history plus today's close.

**Data caveats:**
- **Closes:** Twelve Data's "close" is the last regular-session print it received and can differ from the official closing auction by about ±0.5%. Other sources show SPY at $728.32 and QQQ at $650.99, against $728.78 and $650.76 here.
- **After-hours prices are unavailable.**
  - Massive blocks same-day data.
  - Twelve Data returns HTTP 403 ("Pre-market and post-market data are available on the Pro plan").
  - No AH price is shown, rather than inventing one.
  - **No watchlist name filed an 8-K or released earnings after the bell** (EDGAR checked; see §3).
- **Relative volume (RVOL)** is feed volume divided by the 20-day Massive average, and it is **unverified**.
  - SPY (2.2×) and QQQ (4.3×) are implausible for a holiday half day, so they show n/a.
  - MU's feed volume is 50.4M. Motley Fool showed 26.8M partway through the session.
  - Treat every RVOL as indicative only.

**Labels:** **[FACT]** = sourced or computed from data · **[EST]** = estimate, calendar rule or unconfirmed · **[VIEW]** = my analysis or opinion. Not personalised financial advice.

---

### 🧭 What happened today

- **[FACT] Wednesday's hammer got follow-through.** Every watchlist name closed green, and most closed in the top 10–20% of their range.
  - **Index closes:**
    - S&P 500: **7,297.49 (+1.6%)**
    - Nasdaq Composite: **24,129.50 (+2.3%)**
    - Dow: **50,774.94 (+1.2%)**
  - **Week:** Nasdaq **+6.7%**, S&P **+5.6%** (its best week since April 2025), Dow **+5.5%** (its best since 2022).
  - **10-year yield:** about **4.94%**, up.
  - Source: [Yahoo Finance close recap](https://finance.yahoo.com/markets/stocks/articles/stock-market-today-major-indexes-140450439.html).
- **[FACT] Chips led.** SMH rose **+4.07%**, and the SOX was reported up about 4.7%.
  - MU and MRVL each rose more than 7%. SanDisk gained about 16%.
  - **Nvidia lagged at +0.8%.**
  - Sources: [Yahoo AlphaCheck](https://finance.yahoo.com/markets/article/chip-stocks-lead-a-black-friday-rally-but-nvidia-misses-out-alphacheck-145727185.html), [Trending Topics](https://www.trendingtopics.eu/ai-stocks-black-friday-rally/).
- **[EST / Reported] The move looks like repositioning, not news.**
  - Reuters, as cited by secondary sources, said futures still lean toward a **December Fed hike**.
  - Holiday volume was thin.
  - Nvidia reportedly fell about 3% early on **reports of halted AI-server shipments to Southeast Asia and chip-export issues**. This matters for CRWV and NBIS (Johor, Singapore and Indonesia builds).
  - Sources: [Crypto Briefing](https://cryptobriefing.com/nasdaq-100-gains-2-percent-session-high), [Finimize](https://finimize.com/content/wall-street-tiptoed-back-into-beaten-down-ai-stocks).
- **[VIEW] The day was constructive, but the decisive test was missed by a hair.**
  - **QQQ closed at 650.76.** That is **$0.24 below the 651 "broad confirmation" line**, after an intraday high of 651.34.
  - **SPY slipped back under its 200-day (733.3).**
  - A half-day rally on thin volume is the weakest kind of confirmation. **Monday Nov 30 needs a QQQ close above 651.** MRVL and CRDO earnings on Tue Dec 1 then become the real tell for AI connectivity.

---

### 1️⃣ Session recap

| Ticker | Close | % chg | Open | High | Low | Close in range | AH price | RVOL (feed) |
|---|---|---|---|---|---|---|---|---|
| **SPY** | 728.78 | +1.69% | 725.86 | 729.15 | 719.61 | 96% | n/a | n/a |
| **QQQ** | 650.76 | **+2.65%** | 645.72 | 651.34 | 636.72 | 96% | n/a | n/a |
| **SMH** | 439.67 | **+4.07%** | 435.00 | 440.27 | 421.88 | 97% | n/a | 1.06 |
| RKLB | **50.95** | **+8.36%** | 49.46 | 50.95 | 47.47 | **100%** | n/a | 1.00 |
| BKSY | 17.40 | +8.95% | 16.78 | 17.62 | 16.28 | 84% | n/a | 0.70 |
| RDW | 6.44 | +9.34% | 6.26 | 6.45 | 5.96 | 98% | n/a | 1.36 |
| ASTS | 26.86 | +3.23% | 26.50 | 26.89 | **24.66** | 99% | n/a | 1.14 |
| MRVL | **141.01** | **+7.70%** | 139.41 | 141.82 | 132.32 | 91% | n/a | 1.01 |
| MU | **645.76** | **+7.40%** | 630.28 | 654.44 | 607.27 | 82% | n/a | 1.36* |
| VELO | 3.38 | +6.79% | 3.36 | 3.44 | 3.24 | 72% | n/a | 0.41 |
| NBIS | 89.40 | +5.18% | 89.67 | 89.88 | 83.88 | 92% | n/a | 1.15 |
| CRWV | 44.14 | +3.69% | 43.81 | 44.22 | 40.88 | 98% | n/a | 0.71 |
| OUST | **28.27** | **+9.70%** | 27.50 | 28.27 | 26.30 | **100%** | n/a | 1.01 |
| CRDO | **116.30** | **+8.90%** | 111.00 | 116.40 | 104.73 | 99% | n/a | 1.01 |
| KTOS | 30.40 | +4.99% | 30.20 | 30.59 | 29.56 | 81% | n/a | 0.71 |
| KRMN | 30.91 | +5.60% | 30.35 | 31.35 | 29.67 | 74% | n/a | 0.69 |

**Notes:**
- All values are [FACT] from Twelve Data. % change is measured against the Nov 25 close.
- \* For MU's RVOL, see the volume caveat above.
- AH is unavailable on both feeds' plans. On a half day, the extended session ran 13:00–17:00 ET.
- **[VIEW] Relative strength:**
  - **The leaders were OUST, RDW, BKSY, CRDO and RKLB** (each +8–10%). These are high-beta names behaving as high beta.
  - **The laggards were ASTS (+3.2%) and CRWV (+3.7%).** ASTS was digesting Wednesday's +10%. CRWV still trades like credit.
  - **No name made a new low today.**

---

### 2️⃣ Setup scorecard vs. this morning's brief

| Ticker | Morning setup | What happened | Verdict |
|---|---|---|---|
| **QQQ** (market filter) | Close above 651 = broad confirmation; close below 606 = stand aside | High 651.34, close **650.76** | ⚪ **Not triggered** (missed by $0.24). 606 was never threatened. |
| **RKLB** | Entry $45.0–47.5 on a pullback holding $44.5, **or** a close above $48.8 on ≥1.2× volume. Stop 41.80. T1 52.2 | Low **47.47** touched the top of the zone. Close **50.95**, above 48.8, but feed RVOL was only 1.00× | 🟢 **Triggered** (zone fill by $0.03, plus a price breakout). The volume condition was **not met**. Neither stop nor T1 was hit. |
| **BKSY** | No setup until a close above $17.90 | High 17.62, close 17.40 | ⚪ **Not triggered**. It did reclaim the 16.1–16.4 broken support. |
| **RDW** | No trade; revisit on a close above $6.65 | High 6.45 | ⚪ **Not triggered** |
| **ASTS** | Entry $23.8–25.0 on a pullback holding the base, or a close above $27.40. Stop 21.90 | Low **24.66**, inside the zone, and the base held. Close 26.86 | 🟢 **Triggered** (pullback entry). The close above 27.40 did **not** happen. Neither stop nor target was hit. |
| **MRVL** | Entry $126–132, confirmation on a 4h close above $134. Stop 116.50. T1 150 | Gapped to 139.41. Low **132.32** was $0.32 above the zone. Close 141.01 | 🟡 **Confirmation triggered, entry zone not filled.** No fill at plan prices. |
| **MU** | Needed a **daily close above $630**, then entry $595–630. Stop 545. T1 707 | Close **645.76** | 🟢 **Triggered** (confirmation). Price closed above the entry zone, so the next fill is on a pullback. |
| **VELO** | No trade | — | ⚪ N/A |
| **NBIS** | Potential buy only on a close above $90.5 (entry $82–88). Stop 74 | High **89.88**, close 89.40 | ⚪ **Not triggered** (missed by $0.62) |
| **CRWV** | No trade; revisit on a close above $48.3 | High 44.22 | ⚪ **Not triggered** |
| **OUST** | Confirmation on a close above $28.75; entry $24.5–25.8 | Low 26.30, which did not reach the zone. Close **28.27** at the high | ⚪ **Not triggered** (missed by $0.48) |
| **CRDO** | Entry $100–107. Alert on a close above $107. Stop 92. T1 122.5 | Low **104.73**, inside the zone. Close **116.30** | 🟢 **Triggered** (zone filled and the close confirmed). T1 not hit. |
| **KTOS** | Entry $27.5–29.0, confirmation on a close above $29.75. Stop 26.20 | Low 29.56, which did not reach the zone. Close **30.40** | 🟢 **Triggered** (confirmation close). The zone was not filled. |
| **KRMN** | Confirmation on a close above $30.85; entry $27.5–29.5. Stop 26.00 | Low 29.67. Close **30.91** | 🟡 **Marginally triggered.** The close was $0.06 above the trigger, within the feed's ±0.5% error. Treat it as unconfirmed until Monday holds above 30.85. |

**No setup was invalidated, and no stop was hit.**

---

### 3️⃣ Earnings, filings and material news (Nov 26–27, including after hours)

**[FACT] SEC EDGAR:** none of the 13 tickers filed anything dated Nov 26 or Nov 27. That covers **no 8-K, no Form 4, no S-3 and no 424B (ATM)**.
- The latest RKLB filings are five Form 4s and two Form 144s, filed **Nov 25** for **Nov 23 sales**. The sellers were F. Klein, A. Kampani, M. B. Clevenger, A. Ricupati and A. Spice, at $48.92–51.75, and the filings reference 10b5-1. This was already known, not new. [EDGAR RKLB](https://www.sec.gov/cgi-bin/browse-edgar?action=getcompany&CIK=1819994&type=4)

**No earnings releases** came from any watchlist name today, after hours included.

| Ticker | Today's news |
|---|---|
| **RKLB** | **[FACT] The 101st Electron mission succeeded** (press release on GlobeNewswire, 01:38 UTC Nov 27). Mission details could not be retrieved (HTTP 403). Routine cadence, not a thesis changer. [GlobeNewswire](https://www.globenewswire.com/news-release/2026/11/27/3411054/0/en/mission-success-rocket-lab-launches-101st-electron-mission.html) |
| **RDW** | **[Reported] No company news** behind the move. Motley Fool speculates it is positioning ahead of the **LANDEURO 2026** defense symposium (Wiesbaden, Dec 3–4), where Redwire is showcasing its UAVs and sensors. [Motley Fool](https://www.fool.com/investing/2026/11/27/why-did-redwire-stock-pop-on-friday/) |
| **MU** | **[Reported] No company catalyst.** The move was an "oversold bounce" in memory, attributed to StreetInsider. [Motley Fool](https://www.fool.com/investing/2026/11/27/why-micron-investors-are-giving-thanks-after-thanksgiving/) |
| **MRVL** | No company news. Earnings previews only. Earnings are **Tue Dec 1 after the close** [FACT, per company IR in this morning's brief]. [Zacks preview](https://www.zacks.com/stock/news/3036617/mrvl-to-post-q3-earnings-time-to-buy-sell-or-hold-the-stock) |
| **CRDO** | No company news. Earnings are **Tue Dec 1 after the close**. [Zacks preview](https://www.zacks.com/stock/news/3035918/credo-technology-ahead-of-q2-earnings-how-to-approach-the-stock-now) |
| **CRWV / NBIS** | No company news. **[Reported] Sector risk:** Nvidia AI-server shipments to Southeast Asia reportedly halted, plus export issues. [Yahoo AlphaCheck](https://finance.yahoo.com/markets/article/chip-stocks-lead-a-black-friday-rally-but-nvidia-misses-out-alphacheck-145727185.html) |
| BKSY, ASTS, VELO, OUST, KTOS, KRMN | **No material news.** Massive's news feed and a web search found only commentary and comparison articles. |

---

### 4️⃣ Technical update (daily close vs. SMAs, momentum)

| Ticker | Close | 20d | 50d | 100d | 200d | RSI14 | MACD hist. (prev → now) | ATR % | Note |
|---|---|---|---|---|---|---|---|---|---|
| SPY | 728.78 | 738.3 | 757.2 | 758.4 | **733.3** | 45.2 | −2.92 → −1.51 | 2.3 | Below all four. It failed to reclaim the 200d. |
| QQQ | 650.76 | 663.5 | 705.7 | 707.9 | 683.7 | 43.9 | −2.50 → −0.94 | 3.6 | Histogram near a positive cross |
| SMH | 439.67 | 470.5 | 538.7 | 552.1 | 525.8 | 41.0 | −3.27 → −1.70 | 7.2 | Reclaimed 435 |
| RKLB | 50.95 | 54.1 | 60.1 | 65.2 | 77.2 | 45.3 | −0.95 → −0.63 | 10.7 | **Breakout above 48.8 / 49.6**. The 52.2 gap is next. |
| BKSY | 17.40 | 19.8 | 20.1 | 22.3 | 26.8 | 42.7 | −0.65 → −0.58 | 11.5 | Back above broken support at 16.4 |
| RDW | 6.44 | 7.17 | 8.76 | 9.73 | 10.70 | 41.1 | −0.10 → −0.05 | 10.6 | Pressing 6.45–6.65 |
| ASTS | 26.86 | 31.0 | 43.3 | 53.4 | 70.2 | 38.1 | **−0.08 → +0.18** | 13.0 | **MACD bull cross.** Triple-bottom base at 22.5 |
| MRVL | 141.01 | 151.1 | 213.0 | 214.5 | 189.7 | 39.7 | **+0.23 → +1.27** | 10.7 | Momentum expanding. Gap 132.3–138.5 left open |
| MU | 645.76 | 728.4 | 888.8 | 907.8 | 777.7 | 40.2 | −7.77 → −4.98 | 10.8 | Reclaimed 630. The histogram is still negative |
| VELO | 3.38 | 4.48 | 7.09 | 9.53 | 12.41 | 33.7 | −0.02 → +0.03 | 17.1 | A dead-cat bounce until proven otherwise |
| NBIS | 89.40 | 118.6 | 171.6 | 191.7 | 179.8 | 35.1 | −1.76 → −1.01 | 18.9 | Stalled under 90.5 |
| CRWV | 44.14 | 48.8 | 65.0 | 75.1 | 87.0 | 40.8 | +0.13 → +0.26 | 15.6 | Still just below the morning 4h 20-EMA (44.7) |
| OUST | 28.27 | 31.0 | 34.3 | 36.5 | 33.2 | 45.0 | −0.78 → −0.54 | 12.0 | Closed at the high, just under 28.75 |
| CRDO | 116.30 | 126.2 | 163.8 | 189.6 | 180.8 | 42.4 | **−0.48 → +0.30** | 12.8 | **MACD bull cross.** Gap 107–111 |
| KTOS | 30.40 | 33.6 | 38.9 | 45.3 | 57.2 | 38.1 | −0.42 → −0.18 | 6.9 | Above 29.75. 31.6 is next |
| KRMN | 30.91 | 36.8 | 35.2 | 41.8 | 57.5 | 41.0 | −1.39 → −1.17 | 9.8 | At the 30.85 trigger |

**[FACT] Every ticker still closes below its 20-, 50-, 100- and 200-day SMAs.** No name has reclaimed its 20-day yet.

**[FACT] MACD bullish crosses today:** ASTS and CRDO turned positive, and VELO turned marginally positive. MRVL and CRWV were already positive.

**Levels that changed [VIEW]:**
- **New support:** RKLB 48.8–49.5, MRVL 132.3–134 (the open gap), MU 630, CRDO 107–111 (gap), ASTS 24.7 (today's low), KTOS 29.6.
- **New resistance:** QQQ 651.3, NBIS 89.9–90.5, OUST 28.3–28.75, RDW 6.45–6.65, BKSY 17.6–17.9.

**Breakouts on volume:** none qualify cleanly. RKLB, OUST and CRDO broke out on price, but half-day feed RVOL of about 1.0× is not "on volume". **[VIEW]**

---

### 5️⃣ Plan for the next session (Mon Nov 30) [VIEW unless labeled]

**Market filter:**
- **QQQ daily close above 651** turns on broad confirmation, so sizes can go to half normal.
- **QQQ below 636.7** (today's low) is a warning.
- **QQQ below 606** means stand aside.
- **Size stays at quarter to half** until QQQ reclaims its 20-day at 663.5.

| Ticker | Signal | Entry zone | Stop | T1 / T2 | R/R from mid-entry | Trigger / note |
|---|---|---|---|---|---|---|
| **MU** | **POTENTIAL BUY (triggered)** | $630–640 pullback holding 630 | $604 | $707 / $728 (20d) | from 635: +11.3% / +14.6% vs −4.9% → **2.3 : 3.0** | Confirmed. Don't chase above 655. Earnings Dec 17 [Reported]. |
| **ASTS** | **BUY triggered / HOLD** | Add only on a close above $27.40 or a hold of $25.0–25.8 | $24.40 (tightened from 21.90) | $28.5 / $31.0 (20d) | from 25.5: +11.8% / +21.6% vs −4.3% → **2.7 : 5.0** | MACD bull cross. The launch-date headline is the swing factor. |
| **CRDO** | **HOLD half size (triggered)** | No new adds before earnings | $103.90 (raised from 92) | $122.5 / $131 | — | **Earnings Tue Dec 1 after the close is binary.** Consider trimming into $120–122.5. |
| **MRVL** | **POTENTIAL BUY, earnings binary** | $134–138.5 (gap fill), quarter size at most | $129.90 | $150 / $155 | from 136: +10.3% / +14.0% vs −4.5% → **2.3 : 3.1** | Earnings Tue Dec 1 after the close. Skipping the print entirely is valid. |
| **RKLB** | **POTENTIAL BUY (upgraded from HOLD)** | $48.8–50.0 retest | $46.80 (below today's low) | $52.2 / $56.5 | from 49.4: +5.7% / +14.4% vs −5.3% → 1.1 : 2.7 | Holders from the morning zone: raise the stop from 41.80 to 46.80. |
| **KTOS** | **POTENTIAL BUY (triggered)** | $29.6–30.4 | $28.40 | $31.6 / $33.6 (20d) | from 30.0: +5.3% / +12.0% vs −5.3% → 1.0 : 2.3 | T1 R/R is thin, so T2 is the real objective. |
| **KRMN** | **POTENTIAL BUY, needs confirmation** | $30.0–31.0 after a **close above $30.85 is held** | $29.20 | $33.25 / $35.2 (50d) | from 30.5: +9.0% / +15.4% vs −4.3% → **2.1 : 3.6** | Today's trigger was marginal. |
| **OUST** | **HOLD / MONITOR** → potential buy on a close above $28.75 | $28.75–29.5 after trigger | $26.20 | $31.0 (20d) / $34.3 | from 29.1: +6.5% / +17.9% vs −10.0% → 0.7 : 1.8 | Weak R/R to T1. |
| **NBIS** | **HOLD / MONITOR** → speculative on a close above $90.5 | $88–91 after trigger, one-third size | $83.50 | $97.8 / $110 | from 90: +8.7% / +22.2% vs −7.2% → 1.2 : 3.1 | Southeast Asia export headline risk [Reported]. |
| **BKSY** | **HOLD / MONITOR** | Close above $17.90 (Investor Day Dec 2 [Reported]) | $15.90 | $20.1 (50d) / $22.5 | — | Unchanged |
| **RDW** | **AVOID** → revisit on a close above $6.65 with volume | — | — | — | — | Bounce had no news. ATM overhang. |
| **CRWV** | **AVOID** | — | — | — | — | Close above $48.3 and a financing resolution needed |
| **VELO** | **AVOID** | — | — | — | — | — |

**Key events:**

| When | Event | Status |
|---|---|---|
| Sat Nov 28 – Thu Dec 10 | **Fed blackout period** (FOMC Dec 8–9): no Fed speakers Monday | [EST] calendar rule |
| Mon Nov 30 | Chicago PMI; Dallas Fed manufacturing survey | [EST] usual calendar slot |
| Mon Nov 30 | Month-end rebalancing flows, after a strong week | [EST] |
| **Tue Dec 1** | **JOLTS 10:00 ET**; ISM Manufacturing 10:00 ET | JOLTS [FACT] per [StockTitan](https://www.stocktitan.net/articles/stock-market-today-live-november-27-2026); ISM [EST] |
| **Tue Dec 1, after the close** | **MRVL Q3 FY27** (call 1:30pm PT); **CRDO Q2 FY27** (call 2pm PT) | [FACT] per company IR |
| Wed Dec 2 | BKSY Investor Day; Tradr leveraged space ETF launch | [Reported] |
| Thu Dec 3 | Senate hearing with Nvidia's Jensen Huang | [Reported] |
| Thu–Fri Dec 3–4 | LANDEURO 2026 (RDW exhibiting) | [Reported] |
| Fri Dec 4 | November jobs report | [EST] first-Friday rule |

**No watchlist earnings on Monday.**

---

### 🎯 Bottom line

1. **[FACT] Five of the morning setups triggered** with no stops hit: MU, ASTS, CRDO, KTOS and RKLB. MRVL confirmed but never dipped into its entry zone, and KRMN is marginal.
2. **[FACT] The rally had no company news and no filings behind it.** It was a sector-wide oversold bounce on a thin half day, with chips leading (SMH +4.1%).
3. **[FACT] QQQ missed the 651 confirmation line by $0.24.**
4. **[VIEW] Monday's QQQ close above 651 is the gate to adding size.** Tuesday's MRVL and CRDO prints are the next real test.
5. **[VIEW] Raise stops** on the positions that triggered: RKLB to 46.80, ASTS to 24.40, CRDO to 103.90.

*Data limitations: no after-hours quotes; half-day volumes are unverified; closes are within about ±0.5% of the official auction. Verify prices with your broker before acting.*
