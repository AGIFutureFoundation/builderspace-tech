# GRANTS_500 — Master Grant Programme Spreadsheet

*Built 2026-11-24 for the AGI Future Foundation estate. Companion file: `GRANTS_500.csv` (518 rows × 10 columns). Sibling: the sponsors spreadsheet in `~/workspace/fundraising/sponsors/` (product-credit programmes live there, not here).*

## The headline numbers

- **518 genuine grant programmes** — the 500 target was reached without padding. Pure product-credit programmes were excluded unless the funder itself calls the offer a grant; equity accelerators (a16z speedrun, EF, Antler, Neo, Boost VC) were excluded as investments, not grants.
- **SUBMITTED: 15 rows** — the 13 sprint submissions (Transformative AI Fund, Sentient, Nosana, Bitrefill Partner, Aptos, fal.ai Research, Project Galileo ×2 entities = 14 rows) plus 2 grant awards already in hand (Cartesia Startups grant ≈$7,200 active; OpenRouter grant credits $15 verified).
- **ELIGIBLE NOW: 34** — open calls where no gate binding our entities was found in the funder's own published criteria. Most still carry one named human step (an account, a signature, a fact only Mike holds) — the TOP 25 below are the ones where that step is smallest.
- **GATED: 173** — a real gate binds us today. The dominant gate by far: **a federal 501(c)(3) determination letter / IRS listing, which neither nonprofit holds.** Neither entity is ever described as 501(c)(3) anywhere in the sheet; the Foundation's status is stated as determination-pending and the Fellowship's as §508(c)(1)(A) exempt-by-status.
- **TO VERIFY: 174** — the programme is real and verified to exist, but its binding gates (or current round) were not confirmable from published sources in this pass.
- **EXCLUDED: 122** — invitation-only, internal (university-only), students-only, geography-excluded, permanently closed, or not a grantmaker at all. These are tracked deliberately so nobody fires them by mistake.

## Counts by type

| Type | Rows |
|---|---|
| Cash grant | 387 |
| In-kind grant | 37 |
| RFP | 35 |
| Fellowship | 27 |
| Prize | 25 |
| Residency | 7 |
| Partnership (Bitrefill — submitted sprint row, included for count integrity) | 1 |

## Counts by entity fit

| Entity | Rows |
|---|---|
| AGI Future Foundation | 264 |
| Multiple entities | 107 |
| BuilderSpace (Delaware C-corp, forming) | 57 |
| AGI Fellowship | 29 |
| WAVE (on hold — rows kept for when Mike resumes it) | 14 |
| No fit (tracked as excluded) | 47 |

## How it was built

1. **Mined first (111 rows):** the One-Apply v3 dataset (528 records — only grant-type records extracted, with their structured gates), `APPLICATIONS_LOG.md` (the sprint's 25 slots + bench), and `grants.json` (19 ranked matches). Sprint-verified statuses win over all later research.
2. **Web expansion (407 rows):** six category passes — EA/AI-safety funders (55), Web3 ecosystem grants (65), US federal programmes (70), corporate foundations (65), private/community/faith foundations (85), state/city + arts/media + robotics/STEM + wildlife (70) — each programme verified against a real source on 2026-11-24, apply URLs copied verbatim from sources, amounts and deadlines only as published.
3. **Deduped:** 3 semantic duplicates removed at merge (Coefficient Giving ×2, Disney Conservation Fund ×1).

## Where the well ran dry (honest notes)

- **Corporate grants produced zero ELIGIBLE NOW rows.** Every open corporate programme found requires the determination letter. The closest-to-actionable gated rows once the letter lands: Comcast NBCUniversal Local Impact Grants ($20K–$40K, SF Bay Area is an eligible market), Workday Foundation Human Connection Microgrants (up to $10K, fiscal sponsors allowed), Salesforce Agents for Impact ($200K–$300K, fiscal sponsorship accepted).
- **Federal programmes produced zero ELIGIBLE NOW rows.** SBIR/STTR waits on BuilderSpace's formation; NEA/NEH/IMLS wait on the determination letter; most of the rest need SAM.gov registration and/or a university or government lead applicant.
- **Web3 is a graveyard:** 24 of 65 rows are EXCLUDED — Optimism Grants Council dissolved, Web3 Foundation Grants closed Jan 2026, Interchain Foundation spun down, Aave Grants sunset, ENS Public Goods ended, Ethereum Foundation ESP open intake ended (Wishlist/RFP only). Virtuals has **no** grant programme (its Ecosystem Fund became an investment vehicle).
- **Church funders:** exactly one verified ELIGIBLE NOW row accepts a church by status with no determination letter — Lilly Endowment's National Clergy Renewal Program (up to $60,000; the gate is an ordained pastor in good standing, not tax status). Mustard Seed Foundation, UMCOR Mustard Seed Migration Grants, Thrivent Choice, and Louisville Institute's Pastoral Study Project are strong TO VERIFY candidates with no determination letter in their published eligibility.
- **Discontinued federal programmes flagged in-row:** DOT SMART Grants (no new funding notices), SBA Community Navigator (ended 2024), NSF DISES (concluded), NEA Challenge America and Our Town (folded into Grants for Arts Projects).

## TOP 25 — fire next

*Eligible now; nothing missing beyond a send/apply or the single human step named. Ordered by deadline pressure, then size.*

| # | Programme | Funder | Amount | Deadline / cycle | The one step | Route |
|---|---|---|---|---|---|---|
| 1 | Seed Grants | The Pollination Project | Up to $1,000 | Cycle closes Nov 30, 2026 (estate records — re-verify at fire) | Filing already in flight; referee named (Frontier Tower) | https://thepollinationproject.org |
| 2 | ARENA 10.0 | ARENA / London Initiative for Safe AI | Costs covered | Dec 6, 2026, 11:59 pm AoE | Individual application | https://www.lesswrong.com/posts/AqeCfBTi42vu4j3CW/arena-10-0-call-for-applicants |
| 3 | Mozilla Foundation Fellowship 2027–28 | Mozilla Foundation | $125,000 | Dec 17, 2026, 11:59 pm PT | Mike rewrites the LOI in his own voice and submits | https://mzl.la/fellowshipsLOI |
| 4 | Incubators & Accelerators RFP | Coefficient Giving | $20,000–$7,500,000 | Stage 1 due Dec 18, 2026 | One check: confirm Coefficient accepts a parallel submission alongside the submitted Capacity Building EOI | https://coefficientgiving.org/apply-for-funding |
| 5 | AI Safety Grants | Foresight Institute | $75,000 (ask) | Dec 31, 2026 | Mike names/confirms references | https://foresight.org/ai-safety |
| 6 | CodeSupply (Open Internet Stack) | NLnet Foundation | €5,000–€50,000 | Jan 3, 2027, 12:00 CET | EU-dimension route decision; Mike authors final text | https://nlnet.nl/codesupply |
| 7 | Astera Residency — Spring 2027 | Astera Institute | Fully funded residency | Jan 7, 2027 | Mike applies personally | https://jobs.ashbyhq.com/astera/da1f2782-4125-4161-ad86-ff87d8445802 |
| 8 | Long-Term Future Fund | EA Funds | $1,000–$500,000 | Rolling | Submit the application | https://www.lesswrong.com/posts/esfZCw4YQ4eDxa9kB/apply-to-effective-altruism-funds-now |
| 9 | EA Infrastructure Fund | EA Funds | $1,000–$500,000 | Rolling | Submit the application | https://opportunitiesforyouth.org/2026/09/22/ea-funds-grants-apply-for-1000-500000-in-funding-for-high-impact-projects/ |
| 10 | Seed Grants | BlueDot Impact | $20,000–$200,000 | Rolling | Submit the application | https://grants.watch/programs?method=anytime&sort=name&page=9 |
| 11 | Rapid Grants | BlueDot Impact | Up to $20,000 | Rolling; decisions ~5 days | Submit the application | https://bluedot.org/grants/rapid |
| 12 | AI Safety Regranting | Manifund | $25,000 (ask) | Rolling | Mike creates the account and posts the ready proposal publicly | https://manifund.org |
| 13 | Internet Freedom Fund | Open Technology Fund | $75,000 concept note | Rolling | Mike creates the account; contract-capacity confirmation; budget draft | https://apply.opentech.fund/ |
| 14 | Emergent Ventures | Mercatus Center | Not stated | Rolling | Mike writes and submits himself (funder rejects AI-written applications) | https://mercatus.tfaforms.net/5099527 |
| 15 | STEM K-12 (NSF 25-545) | National Science Foundation | $350,000–$750,000 | Accepted anytime | SAM.gov + Research.gov registration; Mike submits | https://www.research.gov |
| 16 | Guild on 0G | 0G | $50,000 (ask) | Rolling | Mike completes KYC personally | https://0g.ai |
| 17 | Gitcoin Grants (GG rounds) | Gitcoin | Matching pools ($200K per GG23 OSS round) | Per-round windows | List the project when the next round opens | https://gitcoin.co/blog/overview-of-gg23-rounds |
| 18 | Awesome Foundation micro-grants | Awesome Foundation | $1,000 per chapter per month | Monthly chapter cycles | Name one specific bounded project | https://www.awesomefoundation.org |
| 19 | MIT Solve Global Challenges | MIT Solve | $10,000 Solver Award + prize pool | Annual cycle | Submit a solution when the cycle is open | (see CSV row) |
| 20 | Community GPU Grants | Hugging Face | In-kind ZeroGPU (large) for one Space | Rolling | Create the `ask-humanity-explorer` Space under the Foundation org, post the ready request | https://huggingface.co |
| 21 | External Researcher Access Program | Anthropic | $1,000 API credits | Reviewed first Monday monthly | Foundation Claude Console org + ID; Mike submits | https://support.claude.com |
| 22 | Researcher Access Program | OpenAI | Up to $1,000 API credits | December 2026 review | Mike's Educational Stage answer — the draft's sole blocker | https://openai.com/form/researcher-access-program/ |
| 23 | NAIRR Pilot allocations | NSF NAIRR Pilot | In-kind compute, 12 months | Monthly review (by the 15th) | Institutional @agifuturefoundation.org email (Gmail is rejected) | https://nairrpilot.org/opportunities/allocations |
| 24 | Spark Good Local Grants — church category | Walmart | $250–$5,000 | Feb 1–Apr 15, 2027 cycle | Fellowship food-ministry facts (site, days/hours, neighbours per distribution) | https://www.walmart.com/nonprofits |
| 25 | Partner Markets + USDA TEFAP | SF-Marin Food Bank | In-kind food allocation | January partner round | Same food-ministry facts as #24 | https://www.sfmfoodbank.org |

*First reserve: Lilly Endowment National Clergy Renewal Program (Fellowship, up to $60,000, annual) — fires as soon as the Fellowship's pastor-credential facts are confirmed.*

## Standing cautions

- Statuses are as of 2026-11-24 and decay: cycles close, rounds pause (the Web3 section shows how fast). Re-verify any row's openness on the funder's own page before firing — the house rule that already governs the sprint.
- Rows marked TO VERIFY are research leads, not eligibility findings. Do not quote them as eligible anywhere.
- The single biggest unlock for this entire sheet is the Foundation's Form 1023: 173 GATED rows, most of them gated on the determination letter alone.
