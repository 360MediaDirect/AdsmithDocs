# Open Issues — Plain-Language Overview

_Last updated 2026-09-18 06:07:27 UTC · 35 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Saved offer options now reach the live ad** — Several settings you configure on an offer (like modal options and the display URL) were being quietly dropped and never applied. This fix makes those saved choices actually take effect on the live experience. (#295)
- **[Bug]** **Manually selected offers display correctly** — On placements set to manual delivery, the offers you hand-picked (and their order) weren't carrying over, so the wrong offers appeared. This ensures your selected offers show exactly as chosen. (#370)
- **[Bug]** **"Conflicting Offers" rule works again** — When you set offers that shouldn't run together, that rule was being ignored for offers edited in the current admin. This restores proper enforcement. (#358)
- **[Bug]** **Auto-register offers respect duplicate and conflict rules** — Auto-registered offers were skipping the group, conflict, and duplicate-address checks that normal offers follow, which could fire unwanted duplicate leads. This brings them in line. (#355)
- **[Feature]** **Preview shows your unsaved edits** — When editing a placement or offer, the Preview button will reflect your current in-progress changes instead of the last saved version, so you can check a change before committing it. (#292)
- **[Feature]** **Automatic performance projection for new offers** — New offers could receive an estimated performance forecast based on your own historical offer data, replacing today's manual gut-check review. (#322)
- **[Feature]** **Decide the future of the HubSpot List ID field** — This field currently does nothing behind the scenes. We'll either build a real HubSpot connection for it or remove the unused field to avoid confusion. (#362)

## Advertisers & Data Clients

- **[Feature]** **Restore custom pre-checks for data clients** — Many data clients relied on custom, serve-time validation that isn't running on the new platform yet. This high-priority work brings those checks back so those clients behave as before. (#338)
- **[Bug]** **Accurate lead validation on the manual/broker path** — Leads entered through the manual/broker path were always reported as "passed" instead of being genuinely validated. This makes that result real and consistent with the rest of the system. (#366)
- **[Feature]** **After-success delivery steps restored** — Post-conversion delivery and redirect behavior for certain data clients will work on the new platform just as it did before. (#327)
- **[Feature]** **Per-advertiser pre-check validation** — Each advertiser's pre-check will be tested and confirmed correct before it goes live, so nothing breaks at switchover. (#41)

## Admin & General

- **[Task]** **Overall parity tracking with the old system** — A high-priority umbrella effort to confirm everything the legacy system did is matched in New Adsmith Frontend before the old one is retired. (#319)
- **[Task]** **Users screen feature comparison** — A review of what the old Users area could do versus the new one, to plan restoring missing capabilities like bulk actions and last-login details. (#80)
- **[Feature]** **Remove controls that don't do anything** — Some settings (certain user permissions plus a few data-client and pre-check options) look active but currently have no effect. Hiding or removing them keeps the admin trustworthy and clear. (#296)

## Reports & Dashboard

- **[Feature]** **Today's numbers on the Dashboard** — The "today" view will show up-to-date impressions, clicks, leads, and revenue for the current day. (#34)
- **[Task]** **Investigate report numbers vs. the old system** — A high-priority look into why some dashboard report figures don't match the legacy system, so the numbers can be trusted. (#271)

## Surveys

- **[Feature]** **Design choices show up in the live survey** — Ensuring every customization you make on the Design tab actually appears in the survey, plus a full sweep across all screens to catch any options that aren't wired through. (#288)

## Modals

- **[Feature]** **New voucher-style visitor modal** — The visitor modal gets a refreshed look: a personalized header with a voucher number, a progress bar that changes color as offers are claimed, branded offer rows with clear "Claim Offer" and "No Thanks" options, and a secure, branded footer. (#386)

## Behind the Scenes

- **[Feature]** **Faster historical reporting** — Detailed stats will be automatically summarized into daily totals so historical reports load quickly. (#35)
- **[Task]** **Speed up surveys and offers** — Adding a caching layer so survey and offer information loads faster for visitors. (#42)
- **[Bug]** **Prevent long lead submissions from timing out** — Lead submissions that check several outside services will finish reliably without hitting time limits. (#367)
- **[Bug]** **Fix campaign offer-group data reading** — Correcting how campaign offer-group lists are read so they're no longer mistakenly treated as empty. (#372)
- **[Task]** **Safety-test the new pre-check system** — Running the new pre-check system alongside the old one to confirm matching results before switching over. (#40)
- **[Task]** **Run new scheduled jobs in parallel** — Running the new background jobs side by side with the old ones to confirm they behave identically. (#43)
- **[Task]** **Retire lower-risk background jobs** — Turning off the first group of legacy scheduled jobs once their replacements prove stable. (#44)
- **[Task]** **Retire mid-tier background jobs** — Turning off the next group of legacy jobs after a week of stable monitoring. (#45)
- **[Task]** **Retire the most critical background jobs** — Carefully switching off the last and most important legacy jobs, with rollback ready if needed. (#46)
- **[Task]** **Document rollback steps** — Writing clear procedures to quickly revert each system if something goes wrong. (#48)
- **[Task]** **Create troubleshooting guides** — Preparing step-by-step guides for handling common operational issues. (#49)
- **[Task]** **Review an old stats process** — Checking whether a legacy stats job is still needed or can be retired. (#33)
- **[Task]** **Weekly parity scorecard** — An automated weekly report that tracks how closely the new platform matches the old one. (#323)
- **[Feature]** **Turn conversations into tracked tasks** — A helper that reads team conversations and automatically files them as tracked work items. (#272)
- **[Task]** **Run automated UI tests automatically** — Making the automated admin tests run on every update so issues are caught early. (#376)
- **[Task]** **Make automated tests more reliable** — Isolating test data and cleanup so automated tests don't clash with shared data. (#377)
- **[Task]** **Automated test suite review** — Findings and fixes from a review of the admin automated test suite. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
