## 🌙 Post-Market Briefing: Saturday, November 21, 2026 — weekend edition (no US session)

**Data notes (read first)**
- **US markets were closed today, Saturday.** There is no session to recap. This note covers three things:
  - Friday's **final** after-hours prints. Friday's post-market report only had early prints, from about 16:30 ET.
  - Filings and news released since Friday's report.
  - The plan for **Monday, Nov 23**.
- **Retrieved:** 2026-11-21, 21:30–22:10 UTC (23:30–00:10 Bucharest).
- **Prices:** Massive `/v1/open-close` for Nov 20, and Massive 1-minute bars for the last extended-hours print and its timestamp.
  - Massive's open-close had no record for RKLB, so I used its last 1-minute bar instead.
  - Massive's open-close and minute bars both came back empty for SMH. I used the afterHours value from my first pull, before the rate limit hit, and it has no timestamp.
- **Filings:** SEC EDGAR submissions API, for every watchlist name plus the three candidates (ONTO, ALAB, KTOS). The window is filings accepted after 16:30 ET on Nov 20.
- **News:** Massive `/v2/reference/news`, for articles published since 20:30 UTC on Nov 20. I also ran a web search for next week's calendar.
- **Morning brief checked:** `reports/2026-11-21-market-intelligence.md` (branch `claude/pensive-clarke-tjjh86`; it is not on this branch). Its candidates are **ONTO, ALAB and KTOS**.
- **Prior report:** Friday's post-market report is on branch `claude/confident-hypatia-ryr7o0`, file `reports/2026-11-20-post-market.md`.
- **Labels:** [F] = fact with a source. [E] = estimate or unconfirmed. [O] = my opinion. Educational analysis only; not personalised advice.

---

### 🧭 Three takeaways
1. **[F] Friday's after-hours session recovered some of the loss.**
   - Every name finished the extended session +1% to +5% above its close. SPY was +1.1% ($697.49 @ 19:59 ET), QQQ +1.5% and SMH +2.65%.
   - The strongest were OUST +5.2%, RDW +4.3% and RKLB/NBIS about +4%.
   - **[O]** These prints were on thin volume. They are not a confirmed reversal.
2. **[O] RKLB and BKSY ended after-hours at or near their trigger levels.**
   - RKLB's last print was $47.40, above its $47.0 trigger. BKSY's was $16.87, just under its $17.0 trigger.
   - After-hours prints do **not** count as triggers. Both setups need confirmation in Monday's regular session.
3. **[F] No material news or filings over the weekend.**
   - CoreWeave filed seven Form 144s (non-discretionary sell-to-cover on RSU vesting, about $2.3M in total). Nebius filed one Form 4 (an RSU grant).
   - **Key event next week:** Wednesday Nov 25 at 08:30 ET brings Oct PCE, Q3 GDP (2nd estimate) and durable goods. Markets are **closed Thursday for Thanksgiving**, and Friday is a shortened session.

---

### 1. Session recap — Friday Nov 20 close and final extended-hours prints

| Ticker | Fri close | Final ext-hours | Time (ET) | vs close |
|---|---|---|---|---|
| SPY | 689.81 | 697.49 | 19:59 | +1.11% |
| QQQ | 608.45 | 617.72 | 19:59 | +1.52% |
| SMH | 400.06 | 410.65 | n/a (open-close afterHours field) | +2.65% |
| RKLB | 45.42 (Massive daily, per this morning's brief) | 47.40 | 19:59 | +4.4% |
| BKSY | 16.37 | 16.87 | 19:22 | +3.05% |
| RDW | 5.65 | 5.89 | 19:59 | +4.25% |
| ASTS | 23.27 | 24.10 | 19:59 | +3.57% |
| MRVL | 122.28 | 125.72 | 19:59 | +2.81% |
| MU | 594.51 | 610.60 | 19:59 | +2.71% |
| VELO | 2.975 | 3.08 | 19:43 | +3.53% |
| NBIS | 81.31 | 84.53 | 19:59 | +3.96% |
| CRWV | 39.51 | 40.95 | 19:59 | +3.63% |
| OUST | 23.80 | 25.03 | 19:59 | +5.17% |
| ONTO | 170.16 | 175.02 | 19:50 | +2.86% |
| ALAB | 180.35 | 186.20 | 19:58 | +3.24% |
| KTOS | 26.89 | 27.78 | 19:57 | +3.31% |

- **Two data gaps:**
  - **Regular-session closes differ slightly between sources** (for example, SPY's Friday close is 689.81 here). Friday's post-market report used Twelve Data closes.
  - **Friday's highs, lows and relative volume** are unchanged from that report and are not repeated here.
- **[O]** The late bounce matches the "reflex bounce likely" call. Whether it holds depends on Sunday-evening futures and Monday's open.

### 2. Setup check vs. this morning's brief
No regular session was held, so **no setup could trigger or be invalidated today**. The table shows where each setup's level stood at the last extended-hours print.

| Setup | Level that matters | Last ext-hours | Status |
|---|---|---|---|
| RKLB POTENTIAL BUY | Hold $43.89, then an hourly close above $47.0 | $47.40 | **Not triggered.** Above the level in extended hours only; needs Monday's regular session to confirm. |
| BKSY POTENTIAL BUY | Hold $16.09, then reclaim $17.0 | $16.87 | **Not triggered.** $0.13 below the trigger. |
| ONTO POTENTIAL BUY | Zone $158–168; trigger is $155 holding plus a reclaim of $186 | $175.02 | **Not triggered.** Price is above the zone. |
| ALAB HOLD/MONITOR | Hold $176.8, then reclaim $191 | $186.20 | **Not triggered.** |
| KTOS HOLD/MONITOR | Higher low above $26.6, then reclaim $31.6 | $27.78 | **Not triggered.** |
| SPY reversal filter | Reclaim Friday's VWAP ($701.8) or open ($713.6) | $697.49 | **Not met.** |

### 3. Earnings, filings and news since Friday's report
- **CRWV [F]:** Seven **Form 144s**, all dated Nov 20.
  - Filers: Intrator, Venturo, Agrawal, Goldberg, McBee, Jain and McVeety.
  - Total: about 55.5k shares, roughly $2.3M.
  - Each filing states the sales are a **mandatory, non-discretionary sell-to-cover** for tax withholding on RSU vesting.
  - **[O]** Not a discretionary selling signal. Example: [Intrator 144](https://www.sec.gov/Archives/edgar/data/1769628/000195004726011401/).
- **NBIS [F]:** **Form 4**. General Counsel Y. Almog received 10,795 RSUs on Nov 18, vesting quarterly from Jan 4, 2027. This is a grant, not a purchase or sale. **Not material.** [Filing](https://www.sec.gov/Archives/edgar/data/1513845/000151384526000156/)
- **RKLB, BKSY, RDW, ASTS, MRVL, MU, VELO, OUST, ONTO, ALAB, KTOS:** **No material news.** No EDGAR filings were accepted after Friday 16:30 ET.
  - Weekend coverage was opinion pieces only, such as Motley Fool articles on MU, NBIS and RKLB. They are not news. Example: [MU at lowest since May](https://www.fool.com/investing/2026/11/21/micron-stock-just-hit-its-lowest-price-since-may-i-d-buy-more-now/).
- **Macro/NVDA:** I could not find any confirmed new weekend headlines. **[E]** Check Sunday-evening futures before Monday's open.

### 4. Technical update
**No new daily bar was printed.**
- The daily closes vs. the 20/50/100/200-day SMAs, RSI, MACD and ATR are **unchanged** from Friday's post-market report and this morning's brief.
- Key point from those reports: every watchlist name is below its 20- and 50-day SMAs, and most are below their 200-day.

**Levels that matter for Monday [F, from Friday's data]:**
- SPY: $686.75 (Friday's low), $701.8 (VWAP), $713.6 (open), $732.8 (200-day).
- SMH: $396.89 (low).
- RKLB: $43.89 / $47.0. BKSY: $16.09 / $17.0. MU: $585.25 low; $510–540 is the watch zone.
- ONTO: $155 / $186. ALAB: $176.8 / $191.

### 5. Plan for Monday Nov 23 and the week [O]
**Signals are unchanged from this morning's brief:**
- **POTENTIAL BUY (confirmation required):** BKSY, RKLB, ONTO.
- **HOLD/MONITOR:** ALAB, KTOS, MU, MRVL, NBIS, OUST.
- **AVOID:** CRWV, ASTS, VELO, RDW.

**Execution rules:**
- **Do not chase a gap-up.** A Friday after-hours bounce of +3–5% often fades.
- Act only if the first-hour lows hold **and** price reclaims the trigger level on a regular-session hourly close with rising volume.
  - RKLB: above $47.0 (stop $41.90, T1 $55.9).
  - BKSY: above $17.0 (stop $15.20, T1 $20.3).
- Use half-size positions. ATRs are 10–20% of price.
- **If Monday gaps down below Friday's lows** (SPY < $686.75), stand aside. BKSY < $16.09 or RKLB < $43.89 on a close voids those setups.

**Key events this week:**
- **Mon Nov 23:**
  - SYM earnings after the close. It was screened out of the candidates, but it is an AI/robotics sentiment read.
  - [E] NY Fed's Williams speaks at about 3:00 PM ET ([U.S. Bank calendar](https://www.usbank.com/corporate-and-commercial-banking/insights/economy/outlook/weekly.html)).
- **Wed Nov 25, 08:30 ET [F]:**
  - Oct PCE and core PCE, Q3 GDP (2nd estimate), durable goods and jobless claims ([Newsquawk week ahead](https://www.newsquawk.com/headlines/week-in-focus--november-23rd-27th-highlights-include-us-pce-flash-pmis-aussie-cpi-and-ecb-minutes), [Kiplinger](https://www.kiplinger.com/investing/economy/this-weeks-economic-calendar)).
  - [E] The Cleveland Fed nowcast has core PCE at about 0.3% MoM / 3.2% YoY. A hot print would reinforce the pricing for a December hike.
  - [E] One calendar (Newsquawk) also lists FOMC minutes this week; others put them on Nov 18. Unconfirmed.
- **Thu Nov 26:** US markets **closed** (Thanksgiving).
- **Fri Nov 27:** Shortened session. Liquidity will be thin, so expect exaggerated moves.
- **Next:** MRVL and CRDO earnings Dec 1, BKSY Investor Day Dec 2, November jobs report Dec 4, FOMC Dec 9.

---
*Educational analysis only, not personalized investment advice. Extended-hours prints are thin and delayed. Verify before trading.*
