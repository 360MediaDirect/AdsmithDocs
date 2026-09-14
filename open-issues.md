# Open Issues — Plain-Language Overview

_Last updated 2026-09-14 06:09:22 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Saved offer options that never reach live offers** — Several settings you fill in on an offer (like certain modal and display options) currently get dropped before they reach the live offer. Once fixed, the options you save will actually take effect, or unused ones will be cleaned up so the form only shows what really matters. (#295)
- **[Feature]** **Automatic performance projection for new offers** — Instead of relying on a manual gut-check, new offers will get an estimated performance projection based on your own historical offer data, giving you a data-driven read at intake. (#322)
- **[Bug]** **Auto-register offers skipping eligibility checks** — Auto-registering offers can currently fire even when they duplicate or conflict with an offer already shown, or when an address is a known duplicate. The fix applies the same duplicate, conflict, and address checks used everywhere else, so these offers behave consistently. (#355)
- **[Bug]** **"Conflicting Offers" setting not being enforced** — For offers edited in the current admin, the Conflicting Offers rule quietly stops working, so offers that should be mutually exclusive can both appear. This fix makes that setting reliably enforced again. (#358)
- **[Feature]** **Decide the future of the HubSpot List ID field** — The offer HubSpot List ID field currently does nothing. The team will either build a real HubSpot connection behind it or remove the field, so the form only shows controls that actually work. (#362)

## Placements

- **[Feature]** **Preview your unsaved placement and offer edits** — The Preview button will show your current, in-progress changes instead of the last saved version, so you can check how an edit looks before committing to it. (#292)
- **[Bug]** **Manually selected offers not carrying over** — On manual-delivery placements, the list of hand-picked offers is coming across empty, so the wrong offers display. The fix ensures your selected offers (and their order) are preserved. (#370)
- **[Bug]** **Pixel setup instructions that produce broken values** — The on-screen example for placement pixels doesn't match what the system actually understands, so pixels can send garbled tracking data. This fix aligns the two so pixels fire cleanly with correct values. (#384)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — Certain client-specific actions that ran after a successful conversion weren't carried over. This brings that behavior back so those clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients rely on custom validation that runs before a lead is accepted, and it currently isn't running on the new platform. This restores those checks so leads are validated as expected. (#338)
- **[Bug]** **Real lead validation on the manual/broker lead path** — Leads entered through the manual/broker path aren't being checked against the live validation service and always report as "valid." The fix makes that check real, matching the rest of the platform. (#366)

## Reports & Dashboard

- **[Feature]** **Up-to-the-hour numbers in the "Today" view** — The Dashboard's "today" figures for impressions, clicks, leads, and revenue will reflect current-day activity in real time. (#34)
- **[Feature]** **Faster, reliable historical reporting** — Daily totals will be rolled up automatically behind the scenes so historical reports load consistently and accurately. (#35)
- **[Task]** **Investigate report numbers that don't match the old system** — Some Dashboard report totals didn't line up with the legacy app during testing. This work tracks down the cause and confirms the numbers match. (#271)

## Surveys

- **[Feature]** **Design tab changes that actually show in the survey** — Every customization on the Design tab will be reflected in the live survey, and all form options across entities will be reviewed to make sure nothing is a dead control. (#288)
- **[Bug]** **Cleaner handling when outside services are slow** — When several third-party checks are slow at once, a lead submission can currently fail with a hard error. The fix keeps submissions within safe time limits so they return a clean result instead. (#367)

## General / Across the App

- **[Task]** **Users area gap review vs. the old system** — A documented comparison of what the old user-management screens offered versus the new ones, so missing pieces (like bulk actions and login details) can be prioritized. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — A few settings currently look active but have no effect, including some user-permission toggles. These will be hidden or removed so the admin only shows controls that truly work. (#296)

## Modals

- **[Feature]** **Refreshed voucher-style visitor modal** — The visitor modal will get the fuller legacy look: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with clear "Claim Offer" and "No Thanks" actions, and a trust footer. (#386)

## Behind the Scenes

- **[Task]** **Review of an older stats job** — Checking whether an older statistics routine is still needed or can be retired. (#33)
- **[Task]** **Side-by-side pre-ping testing** — Running the new pre-ping process alongside the old one to confirm they produce matching results before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each advertiser's pre-ping works correctly ahead of the switchover. (#41)
- **[Task]** **Faster survey performance groundwork** — Adding a caching layer so survey-related data loads more quickly. (#42)
- **[Task]** **Run new scheduled jobs alongside the old ones** — Deploying the new scheduled tasks in parallel with the existing ones and watching for any differences. (#43)
- **[Task]** **Retire older scheduled jobs (first group)** — Switching off lower-risk legacy scheduled tasks after the replacements prove stable. (#44)
- **[Task]** **Retire older scheduled jobs (second group)** — Turning off the next set of legacy scheduled tasks once monitoring looks clean. (#45)
- **[Task]** **Retire the most critical scheduled jobs (final group)** — Switching off the last and most important legacy tasks, with close monitoring and a quick way to revert. (#46)
- **[Task]** **Document how to roll back safely** — Written procedures for reversing each major system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Step-by-step guides for handling problems like lead-processing or stats hiccups. (#49)
- **[Feature]** **Tool to turn conversations into tracked tasks** — An assistant that reads team chat and files or updates work items automatically, cutting out manual copy-paste. (#272)
- **[Task]** **Single view of migration progress** — An umbrella tracker that rolls up all "match the old system" work into one overall progress picture. (#319)
- **[Task]** **Weekly migration progress scorecard** — An automated weekly report showing how close the new platform is to fully matching the old one. (#323)
- **[Bug]** **Campaign offer-group lists loading reliably** — A data-reading quirk could make a campaign's offer groups appear empty. This fix ensures those lists load correctly. (#372)
- **[Task]** **Run automated UI tests on every release** — Wiring the existing automated test suite into the release process so admin-screen regressions get caught before they reach users. (#376)
- **[Task]** **Keep automated tests from tripping over shared data** — Adding cleanup and isolation so automated tests don't leave behind or collide with shared test data. (#377)
- **[Task]** **Automated test suite review and follow-ups** — A review of the automated test suite that identified fixes to make it more dependable. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
