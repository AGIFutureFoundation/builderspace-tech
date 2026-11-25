# AGENT TRAINING GUIDE — Running the Outreach & Grants Operation

*The complete operating manual for the next agent doing this work, distilled from the November 2026 sprint (184 outreach items, 20 of 25 sprint applications submitted, $77,280.98 headline secured stack). Written so a fresh agent with no other context can run the process. Compiled 2026-11-24. The companion charts live in `charts.html`; the system that automates this manual is specified in `~/workspace/builderspace-testing/ONE_APPLY_SYSTEM_SPEC.md`.*

---

## 1. The mission

Find startup programmes, grants, credits, and partnerships that fit our entities; verify eligibility honestly; file clean applications; capture every credit before it expires; and turn every funder response into a two-way relationship. The long-term product of this work is **One-Apply on BuilderSpace**: a system where a founder picks a programme and everything except the steps only a human may do happens automatically. Every manual step you take is a prototype of a feature — document what slows you down.

## 2. The three legal applicants — and only three

Applications are filed ONLY under legal entities that hold EINs. There are exactly three:

| Applicant | What it is | Use it when |
|---|---|---|
| **AGI Future Foundation** | California nonprofit public benefit corporation (SOS B20260196664), filed 2026-04-24. **No federal 501(c)(3) determination yet** — application in preparation. | Nonprofit programmes; grants requiring or favouring nonprofit status. Approved wording: "federal 501(c)(3) determination pending — application in preparation." Never claim 501(c)(3) status. |
| **AGI Fellowship** | California nonprofit religious corporation (SOS B20260229217), filed 2026-05-13. A church, exempt by status under §508(c)(1)(A); no determination letter, by the statute's design. | Church/religious and community programmes. Approved wording: "church, exempt by status under §508(c)(1)(A), no determination letter per the statute's design." |
| **AGI Corp** | Wyoming profit corporation, legal name **"AGI"** exactly (Filing ID 2024-001420982, filed 2024-03-05). Currently administratively dissolved (tax); reinstatement pending — **never attest good standing**. Website www.agicorp.network; email x@agicorp.network. | **Default applicant** wherever a programme does not require nonprofit status. |

**Project names are never applicants.** BuilderSpace, WAVE, SparkHub, SparkRefill/Coinbridge, Agent Bay and its clones, SmartCiti, TradeQuest, the food apps, and the RP1 worlds are projects or products that live *under* one of the three entities. If a form asks for an applicant, the answer is one of the three legal names above.

**Never enter either nonprofit into IRS-record verification** (Goodstack, GuideStar Charity Check, TechSoup, the IRS BMF): it cannot pass until a determination exists, and a failed check creates a record.

Key people: **Mike Rice** — President of both nonprofits; founder; the human who signs, pays, and supplies every credential step. **Russel Vacanti** — Secretary of both nonprofits; co-founder. Team size, when a form forces a band: the smallest band (1–10). Exact-number team fields are never guessed — stop and ask.

## 3. The verified-figures rule (read this twice)

Every number in an outbound application is pulled from **`~/workspace/fundraising/credits-sprint/APPLICATIONS_LOG.md`** — never typed from memory, never copied from another application, never taken from a marketing page.

- Applications submitted (sprint): **20 of 25** (Foundation 19, Fellowship 1, AGI Corp 0), as of 2026-11-24.
- Secured stack headline: **$77,280.98 across 19 vendors** — with one flagged exception: that headline contains a **$1,000 Exa line graded CONFLICT** (the programme record says blocked/never submitted). The conflict-free itemized total is **$76,280.98 across 18 vendors**. Until a console check resolves Exa, quote the itemized figure or quote the headline only with the conflict attached. A CONFLICT figure never goes into an application as fact.
- Cash raised: **$0**. Everything secured is non-cash credits. Never let "secured" read as cash.

**The cautionary example.** On 2026-11-24, one of our own applications (Supermemory) went out stating "93 programme applications submitted" and "$77,425.98" — while the verified record the same evening was 19 submissions and $77,255.98. Supermemory's system quoted the inflated figures back to us; they now sit in a provider's CRM under our name. The "93" apparently descended from a cumulative marketing count on the One-Apply page — a different data type from sprint submissions. Lesson, permanently: **figures live in the log, not in prose.** If a number isn't in the log with evidence, it doesn't exist.

## 4. The workflow, end to end

1. **Discover.** Sources: the One-Apply dataset (528 programmes / 483 providers, live at builderspace.tech/one-apply.html), sponsor/partnership lists under `~/workspace/fundraising/`, provider pages. Log candidates; never trust a list entry's status — lists go stale (see §9, P10).
2. **Verify eligibility from the programme's own published criteria** — the provider's page, read today, cited with its date. Not a blog, not an aggregator, not our own dataset. Verdicts are PASS / FAIL / UNVERIFIABLE, per entity: the same programme can pass for AGI Corp and fail for the Foundation (Google for Startups fails all three, for three different reasons). Check the traps specifically: nonprofit exclusions, religious exclusions, determination-letter requirements, founding-age windows, VC-funding requirements, partner/referral gates, one-applicant-only terms.
3. **Allocate the entity** and record the allocation with its reason and date. Allocations change (MongoDB moved twice in a day); a recorded allocation stops the next session re-litigating or double-filing.
4. **Build a packet**: the complete field block (legal name, address, website, contact, founding date, funding status, use-case text) plus the exact answers, so any operator — human or agent — can fire it without re-deriving anything. Use the approved status wordings from §2 verbatim; never retype them from memory into new prose.
5. **Fire** by the programme's route: email, web form, or portal/browser sitting. Per-entity separation (§6) applies at firing time.
6. **Apply the stop conditions** (§5) without exception.
7. **Capture the receipt** at filing time: confirmation-screen wording, confirmation email message ID, portal status line, or reference number. No receipt → the item is SUBMITTED-UNVERIFIED, never "submitted."
8. **Log every send** in APPLICATIONS_LOG.md (applications) or the relevant tracker, with date, entity, programme, route, and the receipt evidence. The log is the single source of truth; dashboards and charts are generated from it, never edited independently.
9. **Count only confirmed submissions.** An item counts when the log holds its confirmation, sent-email record, or verified portal status.
10. **Watch for the reply** and classify it on arrival: HOMEWORK (they ask something of us — becomes a task with a deadline; Phala's was 48 hours) · HUMAN HOLD (a person, no date — set a follow-up timer) · AUTO-ACK (no state change, ever) · DECLINE (terminal; capture the stated reason) · DECISION PENDING (note the stated window; when it lapses, chase).
11. **Send the win-win thank-you** on any substantive reply (§7). Auto-acks never trigger one.
12. **Track the capture point** (§8): every award arrives as a code, a claim window, or an activation step with a fuse. Record the fuse the day the award lands.

## 5. Stop conditions — hard stops, no exceptions

Stop the filing, report exactly what the step asks, and hand it to Mike when a form or flow requires:

- **An EIN value.** Never type, transmit, or record an EIN anywhere. Mike enters it himself, in-flow. (A form that merely asks whether the entity *has* an EIN is fine; the value is the line.)
- **A payment** — card entry, a fee, a paid plan conversion. Mike's card, Mike's hand. Watch for traps: Postman's free tier auto-converts to paid after 3 months unless cancelled; Phonic's Pro plan carries a $200/month minimum (Starter only); SambaNova's free tier *ends* if a card is linked.
- **A signature.**
- **Creating an account with a new password.** Passwords are Mike's hand via the Secure Vault. OAuth sign-in under his existing Google/GitHub sessions, where he has directed it, is the standing exception.
- **An attestation you cannot truthfully make** — good standing for AGI Corp, 501(c)(3) status for either nonprofit, revenue or funding the entities don't have.
- **A saved login used anywhere except its own site, in place.** Never extract or move credential values; they never pass through chat, files, or this guide.

## 6. Per-entity separation

- Where a programme fits multiple entities **and its terms allow**, file **separately per entity** — separate applications, separate accounts, separate emails (Xano, Tuta, Fireflies, and Discourse were each filed ×2–3 entities this way). Never file a combined application.
- Where terms allow **one applicant only** (Microsoft for Startups is the standing example: credits secured under the Foundation 2026-11-21), the best-fit entity files and the others are logged **closed-by-terms**. A second filing can endanger the secured position — the downside is asymmetric.
- Where terms are **silent** on sister entities (Deepgram), do not file the second entity; send a disclosure-first enquiry and record the decision.
- Mailbox reality: the Foundation Gmail (agifuturefoundation@gmail.com) is the only mailbox the agent reads. Fellowship mail lands at agent@agifellowship.church and AGI Corp mail at x@agicorp.network — both read by Mike/Why. Any filing whose confirmations land in an unread mailbox carries a **blind-filing warning**: say so before submitting, and create the relay/watch task at filing time.

## 7. The response playbook — win-win thank-yous

Standing rule (Mike, 2026-11-24), full text in `~/workspace/fundraising/response-playbook/`. Whenever a programme, funder, or offer-maker gives a **substantive** response — acceptance, offer, human review notice, homework, decision (including a decline Mike elects to answer), or a public response — send, promptly and on Mike's per-send approval, a Richie Norton-style thank-you that:

1. Thanks them **specifically** and clarifies the details of what was offered/decided (clarify by restating our understanding and asking them to correct it — never assert their programme's details).
2. Asks how we can best serve **them**: permission to post their logo, promote their events, talk publicly about what we build with their product/support.
3. Asks for their **social media handles** and marketing/outreach channels so we can lift up their project and tag them correctly.
4. Asks whether they have an **MCP server**, so we can represent their product, build on it, and share what we build in public.
5. Makes helping them a **stated priority** — a genuine win-win, not a form letter.

Then **do what was offered**: every offer becomes a row in the playbook TRACKER.md with an owner and a done-state (done = the live URL recorded). An offer we don't keep is worse than no offer. One letter per response; if we emailed the same person the same day on the same matter, fold the asks into the next reply instead of double-emailing.

## 8. Capture-point discipline — credits expire

Awards are not money in the bank; they are codes and windows. Standing examples from this sprint:

- **Phonic $250** signup credit: claim by **Nov 30, 2026**; the pilot's cancel-by is **Nov 29** (export everything first).
- **MongoDB** promo code (when issued): must be applied **within 30 days of receipt** — a deadline that starts on an unknown date, in an email to an unread mailbox. Record the receipt date the moment it surfaces.
- **Deepgram**: credits expire 12 months from issue; the application (2026-11-20) sat unchecked for days — an unchecked clock is a risk, not a comfort.
- **The Nov-2027 cliff**: ≈$72,200 of the secured stack expires inside one fortnight in November 2027. Expiry radar at 90/30/7 days, clustered, is the countermeasure.
- **Stytch**: each entity's 3-year window closes on its own incorporation date (AGI Corp's closes March 2027).
- Never store code *values* in trackers — receipt dates, deadlines, and evidence pointers only.

## 9. The 16 holdup patterns — one line each, with the countermeasure

Mined from this sprint's own record (`HOLDUP_ANALYSIS_2026-11-24.md`). Learn these; you will meet all of them.

| # | Pattern | Countermeasure |
|---|---|---|
| P1 | The application isn't the finish line — post-submission "homework" gates the award (Phala, Hatchet, Benevity). | Classify replies fast; homework becomes a task with the provider's deadline the day it lands. |
| P2 | Verification and reply mail lands in a mailbox the filer can't read. | Declare mailboxes per entity; blind-filing warning + relay task before submitting. |
| P3 | One-applicant-only programmes and sister-entity landmines (Microsoft, MongoDB, Deepgram). | Check one-applicant terms at gate time; log closed-by-terms for the other entities. |
| P4 | Duplicate submission, undetected at filing time (BlueDot Rapid went in twice via an Enter keypress). | Submission registry per programme×entity; after an ambiguous submit, verify — never resubmit. |
| P5 | Credits are issued as codes and windows; the window is the product (35 capture points, 6 expiring within a week). | Capture-point record on every award, with the fuse dated the day it lands. |
| P6 | Account-before-application, card-before-account prerequisite chains (AWS parked since Nov 22 on one card tap). | Map the chain before filing; batch account creation into one sitting. |
| P7 | Legal status no checker can verify; wording must be exact per funder (determination-pending, §508(c), dissolved). | Approved wording library, inserted verbatim; never improvise status language. |
| P8 | Our own numbers drift between filings (93 vs 19; $77,425.98 vs $77,255.98 — quoted back by a funder's CRM). | Verified-figures rule (§3): numbers are pulled from the log at draft time, never typed. |
| P9 | Auto-acks that look like progress; silence that means decline (Railway's ack; DigitalOcean's silence-as-decline). | Reply classification (§4 step 10); an ack never advances a pipeline stage. |
| P10 | Programmes die, move, or rename between research and filing (DigitalOcean Hatch sunset; Airbyte 404). | Re-verify the route at firing time; link audits on a cadence. |
| P11 | Deadlines in someone else's clock and calendar (Pollination ET-vs-PST; Cities Deliver's derived Nov 27 LOI deadline). | Store deadlines as published + converted; derive effective deadlines from counterparty calendars; plan against the earlier reading. |
| P12 | Everything converges on one person's hands — nine human steps open at once, several expiring while waiting. | Name each human step exactly; batch them into one sitting ordered by deadline × value unblocked. |
| P13 | Our own records disagree (MongoDB, NVIDIA, Exa, Murf — five live conflicts). | One governing source per data type (submissions: the log; money: the graded ledger); conflicts quarantined, resolved by evidence, never silently edited. |
| P14 | Eligibility discovered after drafting (Google × AGI Corp; fal.ai Startup; Datadog's referral gate). | Gates before drafting (§4 step 2). No draft exists for a pair that hasn't passed. |
| P15 | Receipt fragility — submissions that leave almost no proof (BlueDot's redirect; EA Funds' single dashboard link). | Receipt capture at filing time (§4 step 7); sensitive receipt links recorded as pointers, never copied into shared surfaces. |
| P16 | The matcher's answers move with the user's wording (free-text profile fields flip gates). | Controlled vocabulary on gate-read fields; show the deciding criterion and input with every verdict. |

## 10. Email formatting and signature

Every outgoing email — applications, outreach, thank-yous, job applications, all of it — is formatted as if typed by a human in a normal email editor: real HTML bold/headers where HTML is used, **no markdown asterisks**, no agent meta-commentary or process asides in the body. Standard signature:

Mike Rice
President & CEO, AGI Future Foundation
agifuturefoundation@gmail.com · 628-789-3750
LinkedIn: linkedin.com/in/infogurus/ · X: @DeSciDude
San Francisco, California

House style for outreach letters: gratitude first, generous, win-win, **to the point** (the ask and any deadline plain), qualitative benefit only (never invented statistics), and — for Fellowship-flavoured outreach — the Ask Humanity close (ask.fellowship.chat; one of the twenty questions quoted exactly from `~/workspace/fellowship/ASK_HUMANITY_20_QUESTIONS.md`, consent-first framing).

## 11. The one-click roadmap — from this manual to One-Apply features

Each manual step above maps to a system feature in `ONE_APPLY_SYSTEM_SPEC.md`. This table is the build order's logic: the features exist because their absence cost time, money, or accuracy in this sprint.

| Manual step (this guide) | One-Apply feature | What it automates |
|---|---|---|
| Verify eligibility per entity before drafting (§4.2) | **F1 — Gates before drafting** | Gate evaluation against the provider's own snapshotted criteria; PASS / FAIL / UNVERIFIABLE; recorded entity allocation. |
| Track codes, claim windows, cancel-bys (§8) | **F2 — Capture-point tracker** | Every award's capture object, relative deadlines that compute from the receipt date, 90/30/7-day expiry radar, trap flags at the exact step. |
| Batch Mike's taps into sittings (§9 P12) | **F3 — Human-step stager** | Each blocked item names its exact human step; steps batch into one sitting ordered by deadline × value, with the sitting's total yield shown; steps routed to whoever's hand they belong to. |
| Blind-filing warnings and relays (§6) | **F4 — Mailbox & verification routing** | Per-entity mailbox/readership map; email-of-record captured at filing; verification watch + automatic relay tasks. |
| One-applicant and duplicate discipline (§6, P3/P4) | **F5 — Duplicate & one-applicant guards** | Programme×entity submission registry with hard stops; one-applicant flags that block sister-entity drafts; duplicate alerts with a pre-drafted disclosure note. |
| Verified figures and exact status wording (§§2–3) | **F6 — Wording library + verified-figures service** | Approved strings inserted, never retyped; every number pulled from the ledger with its evidence grade and as-of time; CONFLICT figures cannot be inserted. |
| Reply classification (§4.10) | **F7 — Reply classification & pipeline truth** | HOMEWORK / HUMAN HOLD / AUTO-ACK / DECLINE / DECISION PENDING on arrival; silence-past-window flips to OVERDUE or PRESUMED DECLINED; playbook thank-you arms only on substantive replies. |
| Receipt capture (§4.7) | **F8 — Receipt capture** | The receipt object stored at filing; "submitted" is earned, never asserted; SUBMITTED-UNVERIFIED state with a verification task. |
| Governing sources and conflict quarantine (§9 P13) | **F9 — Record reconciliation** | Standing diff across dataset / log / ledger; governing source per data type; corrections ship as a visible list, never silent edits. |
| Careful profile wording (§9 P16) | **F10 — Profile robustness & matcher transparency** | Controlled vocabulary on gate-read fields; every verdict names its deciding criterion and input; profile-diff preview before saving. |
| Deadline conversion and derivation (§9 P11) | **F11 — Deadline engine** | Deadlines stored as published + converted; counterparty calendars derive effective deadlines; rule-shaped deadlines ("first Monday monthly") computed per item; decision windows on the same radar. |

**The one-click vision, honestly stated:** of 528 dataset records, most sit in the founder-portal lane — the founder files, under their own entity, with their own accounts. "One click" therefore means: the matcher and gates are instant (F1, F10), the packet is complete and pre-filled with verified figures (F6), the human steps are staged into a single guided sitting (F3), the filing is guarded against duplicates and one-applicant traps (F5), the receipt is captured automatically (F8), the reply is classified and the thank-you drafted (F7), and the credit's fuse is watched until it's safely applied (F2). The human still does the steps only a human may do — sign, pay, enter a credential — but they do them once, in one sitting, with everything else already done.

## 12. Records map — where everything lives

- Applications log (governing): `~/workspace/fundraising/credits-sprint/APPLICATIONS_LOG.md`
- Outreach dashboard + master CSV: `~/workspace/outreach-dashboard/`
- Tri-entity progress board: `~/workspace/fundraising/TRI_ENTITY_PROGRESS_2026-11-24.md`
- Response playbook (rule, templates, tracker): `~/workspace/fundraising/response-playbook/`
- Holdup analysis + system spec: `~/workspace/builderspace-testing/`
- This playbook (charts + guide): `~/workspace/one-click-playbook/`
- Live matcher: https://builderspace.tech/one-apply.html · Published lists: https://builderspace.tech/lists/

*Maintenance rule: every future holdup gets a pattern number (existing or new) in the analysis file; every pattern with three or more instances gets a spec feature or a recorded decision not to build one. And every figure in this guide carries its as-of date — when the log moves, this guide is regenerated, not patched from memory.*
