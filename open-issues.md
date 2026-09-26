# Open Issues — Plain-Language Overview

_Last updated 2026-09-26 06:07:26 UTC · 33 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never take effect** — Several options you can set on an offer (certain modal settings, the display URL, and a few data-handling flags) currently don't carry through to the live experience. This ensures the settings you save actually apply. (#295)
- **[Bug]** **Manually selected offers now carry over on migrated placements** — On Manual-delivery placements the chosen offer list was coming over empty, so the wrong offers displayed. This makes sure your selected offers, in the right order, transfer correctly. (#370)
- **[Bug]** **"Conflicting Offers" rule enforced again** — For offers edited in the current admin, the conflicting-offers setting had quietly stopped working. This restores it so offers that shouldn't appear together are properly kept apart. (#358)
- **[Bug]** **Auto-register offers now run the same duplicate and conflict checks** — Auto-registering offers were skipping the duplicate and conflict screening other offers go through, which could fire leads that should have been blocked. This applies those checks consistently. (#355)
- **[Feature]** **Preview offers and placements with unsaved changes** — The Preview button will show your in-progress edits instead of only the last saved version, so you can check a change before committing it. (#292)
- **[Feature]** **Automatic performance projections for new offers** — New offers could get an automated estimate of how they're likely to perform, based on your historical offer data, replacing the manual gut-check review. (#322)
- **[Feature]** **Decide the future of the HubSpot List ID field** — This offer field currently does nothing. The work will either build a real HubSpot connection behind it or remove the unused field so the form isn't misleading. (#362)

## Data Clients

- **[Feature]** **Bring back custom pre-check validation** — Custom per-client lead screening from the old platform hasn't been carried over. This restores it so leads are validated before delivery, just as before. (#338)
- **[Feature]** **Restore after-success delivery steps** — Post-conversion delivery and redirect steps from the old platform are being ported so leads continue to be handed off correctly after a successful conversion. (#327)
- **[Bug]** **Real lead-validation results for manually processed leads** — In one lead-processing path, the "validated" indicator was always marked true regardless of the real outcome. This wires in genuine validation so the result is accurate. (#366)

## General / Across the App

- **[Task]** **Overall parity tracking with the old system** — An umbrella effort to confirm every feature, behavior, and number in New Adsmith Frontend matches the legacy platform before it's retired, so nothing gets missed. (#319)
- **[Task]** **Weekly parity scorecard** — A regularly refreshed report showing how close the new platform is to fully matching the old one, so remaining gaps are spotted and worked through. (#323)
- **[Bug]** **Campaign offer-group lists load correctly** — The same list-reading issue fixed on placements is now being fixed for campaigns, so campaign offer groups show the right items in the right order. (#372)

## Reports & Dashboard

- **[Task]** **Confirming report numbers match the old system** — During testing, dashboard report figures didn't line up with the legacy app. This investigation pins down why and confirms the numbers can be trusted. (#271)
- **[Feature]** **Live "today" numbers on the dashboard** — The dashboard's "today" view will show up-to-the-hour impressions, clicks, leads, and revenue for the current day. (#34)

## Surveys

- **[Feature]** **Every design option will actually work** — An audit and sync so all customizations in the Design tab are reflected in the live survey, with no settings that quietly do nothing. (#288)
- **[Bug]** **Prevent lead submissions from timing out** — When several outside checks run one after another, a submission could run past the time limit and fail. This reworks the timing so submissions finish cleanly. (#367)

## Users

- **[Task]** **Users screen compared to the old system** — A review of what the old Users area could do versus the new one, so missing capabilities (like bulk actions and extra columns) can be prioritized. (#80)

## Behind the Scenes

- **[Feature]** **Faster survey performance** — Adding a caching layer so survey configurations and offer data load more quickly. (#42)
- **[Feature]** **Historical stats roll-up** — Building the routine that gathers daily stats into historical totals for reporting. (#35)
- **[Feature]** **Per-advertiser pre-check validation** — Verifying the new lead pre-check works correctly for each advertiser before switching over. (#41)
- **[Feature]** **Slack-to-task helper** — Exploring a Slack assistant that turns conversation notes into tracked tasks automatically. (#272)
- **[Task]** **Side-by-side pre-check testing** — Running the new lead pre-check alongside the old one to confirm the results match before the switch. (#40)
- **[Task]** **Run background jobs in parallel** — Running the new scheduled background jobs alongside the existing ones in production and watching for any differences. (#43)
- **[Task]** **Gradual switchover of background jobs (lower priority)** — Retiring the least critical old scheduled jobs first, with close monitoring. (#44)
- **[Task]** **Gradual switchover of background jobs (mid priority)** — Retiring the next set of old scheduled jobs once the earlier ones prove stable. (#45)
- **[Task]** **Gradual switchover of background jobs (most critical)** — Retiring the most critical old jobs last, with immediate rollback ready if needed. (#46)
- **[Task]** **Rollback procedures documented** — Writing and testing step-by-step recovery plans for each system in case anything goes wrong. (#48)
- **[Task]** **Troubleshooting guides** — Creating reference guides for handling common operational issues quickly. (#49)
- **[Task]** **Review an old stats job** — Checking whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Automated admin tests in the release pipeline** — Adding the existing automated checks to the release process so admin issues are caught before they reach users. (#376)
- **[Task]** **Safer, cleaner automated testing** — Improving how automated tests isolate their data and clean up afterward to reduce false failures. (#377)
- **[Task]** **Automated-testing audit follow-ups** — Addressing the remaining findings from a review of the automated test setup. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
