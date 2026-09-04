# Open Issues — Plain-Language Overview

_Last updated 2026-09-04 06:07:34 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Saved offer options now actually reach the live ad** — Several settings you configure on an offer weren't being carried through to what visitors actually see. This high-priority fix makes sure those options take effect instead of being silently dropped. (#295)
- **[Bug]** **Manually selected offers carry over correctly** — On Manual-delivery placements, the "Selected Offers" list was coming across empty, so the wrong offers displayed. Your chosen offers (and their order) will now show exactly as configured. (#370)
- **[Bug]** **Auto-register offers respect duplicate and conflict rules** — Automatic offers were skipping the group, conflict, co-duplicate, and address de-dupe checks. They'll now follow the same eligibility rules as every other offer, preventing bad or duplicate leads. (#355)
- **[Bug]** **"Conflicting Offers" enforcement works again** — For any offer edited in the new admin, the mutual-exclusion setting had quietly stopped working. This fix restores it so conflicting offers are properly kept apart. (#358)
- **[Feature]** **Preview your unsaved edits before saving** — On placement and offer edit screens, Preview will reflect the changes you're currently making instead of only the last-saved version, so you can check your work without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, new offers could be scored against your historical offer data to estimate how they're likely to perform, giving you a data-backed read at intake. (#322)
- **[Feature]** **Decision on the HubSpot List ID field** — This field currently does nothing behind the scenes. We'll either build the real HubSpot connection or remove the unused field so the form only shows options that work. (#362)

## Behind the Scenes

- **[Feature]** **Groundwork for historical reporting** — Building the process that rolls up daily activity so long-range report queries stay fast and accurate. (#35)
- **[Feature]** **Auto-file issues from conversations** — A helper that reads designated chat channels and turns action items into tracked tasks automatically, reducing manual note-taking. (#272)
- **[Bug]** **Prevent lead submissions from timing out** — When several outside checks run back-to-back, a submission could exceed the time limit and fail. We're reworking this so leads finish cleanly. (#367)
- **[Bug]** **Fix a data-reading glitch on campaign offer groups** — An edge case in how saved lists are read could cause offer groups to come back empty. This corrects it so counts and details load reliably. (#372)
- **[Task]** **Faster surveys through caching** — Adding a caching layer so survey and offer configurations load more quickly for visitors. (#42)
- **[Task]** **Run new pre-ping alongside the old system** — A high-priority side-by-side comparison to confirm the new lead pre-checks produce the same results before switching over. (#40)
- **[Task]** **Run new scheduled jobs in parallel** — All new background jobs run alongside the existing ones in production while we watch for any differences. (#43)
- **[Task]** **Retire old background jobs — first wave** — Turning off the lowest-risk legacy scheduled jobs once their replacements prove stable. (#44)
- **[Task]** **Retire old background jobs — second wave** — Switching off the next set of legacy jobs (various stats tasks) after the first wave holds steady. (#45)
- **[Task]** **Retire old background jobs — final, critical wave** — Carefully turning off the most critical legacy jobs (lead processing, offer-cap reset) last, with immediate rollback ready. (#46)
- **[Task]** **Review an old stats job** — Deciding whether a legacy stats task is still needed or can be safely retired. (#33)
- **[Task]** **Document rollback steps** — Writing clear procedures to quickly revert each system if something goes wrong during the switchover. (#48)
- **[Task]** **Troubleshooting runbooks** — Step-by-step guides for handling common issues so problems get resolved faster. (#49)
- **[Task]** **Weekly parity scorecard** — A living, auto-updated report that tracks how close the new platform is to matching the legacy system. (#323)
- **[Task]** **Run automated UI checks automatically** — Wiring the existing automated tests into the release process so admin-screen regressions get caught before they reach you. (#376)
- **[Task]** **Cleaner test data handling** — Improving how automated tests isolate and clean up their data so results stay reliable. (#377)
- **[Task]** **Automated test framework review** — A quality audit of the automated test suite to find and fix gaps. (#379)

## Data Clients

- **[Feature]** **Restore custom pre-lead checks** — High-priority work to bring back the per-client validation rules that ran before a lead was accepted, so those safeguards work on the new platform. (#338)
- **[Feature]** **Restore post-conversion delivery steps** — The "after-success" scripts that run once a lead converts are being ported over so delivery behaves the same as before. (#327)
- **[Bug]** **Accurate lead-validation status in the transactions path** — Leads processed through the manual/broker pipeline were reporting a fixed "validated" status. This makes that flag reflect the real validation result. (#366)

## General / Across the App

- **[Feature]** **Remove controls that don't do anything** — Some admin settings are saved but never actually used. We'll hide or remove them so the interface only shows options that have a real effect. (#296)
- **[Task]** **Users screen gap review** — Comparing the old and new Users areas to identify missing capabilities (like bulk actions and login/2FA details) and plan what to add. (#80)
- **[Task]** **Legacy-to-new parity tracking** — An overarching effort that rolls up every "match the old system" item into one view so nothing falls through the cracks until the old admin is retired. (#319)

## Dashboard / Reports

- **[Feature]** **See today's numbers in real time** — The dashboard will show up-to-the-hour impressions, clicks, leads, and revenue for the current day. (#34)
- **[Task]** **Investigate report figures vs. the old system** — High-priority check into why some dashboard report numbers didn't match the legacy app, so you can trust the figures. (#271)

## Surveys

- **[Feature]** **Design tab changes fully reflected in the survey** — Every customization you make on the design tab will actually show up in the live survey, with a full review to catch any options that aren't wired through. (#288)

## Modals

- **[Feature]** **Redesigned voucher-style visitor modal** — The visitor modal will get the polished legacy look: a personalized header with a voucher number, a color-coded progress bar that tracks claimed offers, branded offer rows, and a "Powered by (ad)smith / Verified Secure" footer. (#386)

## Placements

- **[Bug]** **Pixel tracking instructions that actually work** — The in-app pixel help text showed a macro format the system didn't recognize, which corrupted tracking values. We'll make the macros work as documented so attribution data stays clean. (#384)

## Advertisers

- **[Feature]** **Verify pre-ping for each advertiser** — High-priority checks confirming each active advertiser's pre-lead validation works correctly before switching over. (#41)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
