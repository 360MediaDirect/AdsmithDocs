# Open Issues — Plain-Language Overview

_Last updated 2026-09-05 06:06:29 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Bug]** **Saved offer options don't reach the live offer** — Several options you set when editing an offer currently get dropped and never appear on the live offer. This fix makes sure each option either works end-to-end or is cleaned up so it isn't misleading. (#295)
- **[Feature]** **Automatic performance projection for new offers** — Instead of relying on a manual gut-check, you'll get a data-driven estimate of how a new offer is likely to perform, based on your own history of similar offers. (#322)
- **[Bug]** **Auto-register offers now respect all the usual eligibility rules** — Auto-firing offers currently skip duplicate, conflict, and address de-duplication checks, so a visitor could get an offer that should have been blocked. This makes them follow the same rules as every other offer. (#355)
- **[Bug]** **"Conflicting Offers" setting now actually enforced** — For offers edited in the current admin, the mutual-exclusion between conflicting offers was silently doing nothing. This restores it so conflicting offers are correctly kept apart. (#358)
- **[Feature]** **Decide the fate of the HubSpot List ID field** — This offer field currently has no effect at all. We'll either build the HubSpot connection behind it or remove the field so it doesn't imply something that isn't happening. (#362)

## Placements
- **[Bug]** **Manually selected offers now carry over correctly** — On Manual-delivery placements, the list of hand-picked offers wasn't migrating, so the new platform showed the wrong or no offers. This restores the exact selected offers and their order. (#370)
- **[Feature]** **Preview reflects your unsaved edits** — On placement and offer edit pages, Preview will show your current in-progress changes instead of only the last saved version, so you can check edits before saving. (#292)
- **[Bug]** **Placement pixel examples that actually work** — The on-screen pixel example used a format the system didn't recognize, quietly corrupting tracking values. This makes the documented example work correctly so attribution data stays clean. (#384)

## Data Clients
- **[Feature]** **Post-conversion delivery steps restored** — The legacy "after success" delivery/redirect behavior for certain clients is being brought over so those clients keep working as before. (Nearly complete.) (#327)
- **[Feature]** **Legacy pre-ping validation brought forward** — Hundreds of clients relied on custom pre-checks that don't currently run on the new platform. This ports that validation so those checks apply again before a lead is delivered. (#338)
- **[Bug]** **Accurate lead-validation status for manually submitted leads** — Leads submitted through the manual/broker path always reported "validated" regardless of the real result. This wires in the real validation check so the status is truthful. (#366)

## Surveys
- **[Feature]** **Design-tab settings fully reflected in the survey** — Every customization option on the Design tab will be checked and connected so what you set is what visitors see, with no dead options. (#288)
- **[Bug]** **Survey lead submission won't hang** — When several outside services are slow at once, a lead submission can be cut off with an error. This reworks the flow so it always returns a clean result instead of failing hard. (#367)

## Dashboard & Reports
- **[Feature]** **Live "today" numbers on the dashboard** — The dashboard will show up-to-the-hour impressions, clicks, leads, and revenue for the current day in the correct time zone. (#34)
- **[Task]** **Investigate report numbers that don't match the old system** — We're comparing the new platform's report figures against the legacy system on a fixed date range to find and explain any differences. (#271)

## Admin & Users
- **[Feature]** **Hide admin controls that do nothing** — Some settings (certain user permissions and a few data-client and pre-ping options) are saved but not actually used. We'll hide or remove them so a control never implies access or behavior that doesn't exist. (#296)
- **[Task]** **Users screen gap review** — A documented comparison of the old Users management area against the new one, so we know exactly which features (like bulk actions and extra columns) still need to be added. (#80)

## Advertisers
- **[Feature]** **Per-advertiser pre-ping checks verified** — We'll confirm the new pre-ping works correctly for each active advertiser, checking field mapping and success rules before switching over. (#41)
- **[Task]** **Side-by-side pre-ping testing** — The new pre-ping runs alongside the old one on the same leads so we can compare results and fix any differences before it goes fully live. (#40)

## General / Across the App
- **[Task]** **One place to track "old vs. new" completeness** — An overarching tracker that rolls up every remaining gap between the legacy system and New Adsmith Frontend, so progress is visible in one number instead of scattered items. (#319)
- **[Bug]** **Campaign offer-group counts show correctly** — A data-reading quirk could make certain campaign offer groups come back empty. This fixes the parsing so offer groups and their counts display reliably. (#372)

## Modals
- **[Feature]** **Refreshed voucher-style visitor modal** — The visitor modal will match the legacy "voucher" look: a personalized header with a voucher number, a per-offer progress bar that recolors as offers are claimed, a branded offer row with Claim/No Thanks, and a trust footer. (#386)

## Behind the Scenes
- **[Feature]** **Historical stats roll-up** — A scheduled process to summarize hourly data into daily totals so long-term reports load reliably. (#35)
- **[Task]** **Faster survey performance** — Adding a caching layer so survey configurations and offer data load more quickly for visitors. (#42)
- **[Task]** **Evaluate an old stats job** — Reviewing whether a legacy background stats job is still needed or can be retired. (#33)
- **[Task]** **Run new and old background jobs in parallel** — Running the new scheduled jobs alongside the existing ones and watching for differences before switching over. (#43)
- **[Task]** **Retire lower-risk background jobs (Tier 3)** — Turning off the least critical old jobs once their replacements are proven stable. (#44)
- **[Task]** **Retire the next set of background jobs (Tier 2)** — Switching off additional old stats jobs after a monitoring period. (#45)
- **[Task]** **Retire the most critical background jobs (Tier 1)** — Carefully turning off the highest-stakes jobs last, with an immediate fallback plan. (#46)
- **[Task]** **Rollback procedures documented** — Clear, tested steps to revert each production system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides created** — Step-by-step guides for handling common operational issues. (#49)
- **[Feature]** **Slack-to-issue helper** — A tool that turns action items from Slack conversations into tracked work items automatically, reducing manual copy/paste. (#272)
- **[Task]** **Weekly progress scorecard** — An automated weekly summary of how close the new platform is to full parity with the old one. (#323)
- **[Task]** **Automated testing runs in the pipeline** — Wiring the full end-to-end test suite to run automatically after each update so regressions are caught before they reach users. (#376)
- **[Task]** **Cleaner, more reliable automated tests** — Adding cleanup and isolation so test runs don't leave stray data or interfere with each other. (#377)
- **[Task]** **Test-suite audit follow-ups** — Tracking the remaining fixes from a review of the automated test setup. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
