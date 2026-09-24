# Open Issues — Plain-Language Overview

_Last updated 2026-09-24 06:08:08 UTC · 34 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Manually selected offers now show correctly** — On placements set to "Manual" delivery, the offers you handpicked (and their order) weren't carrying over, so visitors saw the wrong offers or none. This ensures your selected offers display exactly as chosen. (#370)
- **[Bug]** **"Conflicting Offers" rule will be enforced again** — For offers edited in the current admin, the conflicting-offers setting was being silently ignored, letting mutually exclusive offers appear together. This restores that protection. (#358)
- **[Bug]** **Auto-registering offers will respect all eligibility rules** — Auto-register offers were skipping duplicate, group-conflict, and address de-duplication checks. This makes them follow the same rules as every other offer, so they won't fire when they shouldn't. (#355)
- **[Bug]** **Saved offer options will actually take effect** — Several options you can set on an offer weren't reaching what visitors see. Each of these will now either work as expected or be cleaned up so nothing misleading remains. (#295)
- **[Bug]** **Fix campaign offer groups showing as empty** — Corrects a data-reading issue that could make a campaign's offer groups appear empty. Counts and lists will show correctly. (#372)
- **[Feature]** **Preview your unsaved edits on Offers and Placements** — The Preview button will reflect the changes you're currently making, so you can check them before saving instead of having to save first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — New offers will get an estimated performance outlook based on your own historical data, replacing the manual review step. (#322)
- **[Feature]** **Decide the future of the HubSpot List ID field** — This field currently does nothing behind the scenes. This work will either build a real HubSpot connection or remove the unused field so it isn't misleading. (#362)

## Reports

- **[Task]** **Confirm report numbers match the legacy system** — A high-priority investigation into why some dashboard report figures differed from the old app, so you can fully trust the numbers. (#271)
- **[Feature]** **Live "today" numbers on the Dashboard** — The current day's impressions, clicks, leads, and revenue will show in real time in the "today" view. (#34)
- **[Feature]** **Keep historical report data fast and accurate** — Behind-the-scenes rollup of daily totals so historical reports load quickly and stay correct. (#35)

## Data Clients

- **[Feature]** **Restore legacy validation checks (pre-ping)** — A high-priority effort to bring back per-client lead-validation checks that ran in the old system, so leads are screened the same way before delivery. (#338)
- **[Feature]** **Restore post-conversion delivery steps** — The after-conversion delivery behaviors used by certain clients will be brought over to the new platform so those hand-offs keep working. (#327)
- **[Bug]** **Real lead validation for manually entered leads** — Leads entered outside the survey flow will be checked against the real validation service instead of always being marked valid. (#366)

## Admin

- **[Feature]** **Remove admin controls that do nothing** — Several settings (some user permission toggles and unused data-client and pre-ping options) currently look active but have no effect. These will be hidden or removed to avoid confusion. (#296)
- **[Task]** **Users screen gap review** — A documented comparison of the old Users management against the new one, mapping out missing capabilities (like bulk actions, last-login, and 2FA status) to plan what to add. (#80)

## Surveys

- **[Feature]** **Design tab settings fully applied to surveys** — Every customization option on the Design tab will be reflected in the live survey, with a check to catch any option that isn't wired through. (#288)
- **[Bug]** **Prevent survey lead submissions from timing out** — When several outside checks run during a submission, they could add up and cause a failure. This reworks the timing so submissions complete reliably. (#367)

## Advertisers

- **[Feature]** **Verify pre-checks for each advertiser** — Before switching over, each active advertiser's lead pre-check will be tested to confirm it maps fields correctly and behaves as expected. (#41)

## General / Across the App

- **[Task]** **Track full parity with the legacy system** — A high-priority umbrella effort to make sure the new platform matches everything the old admin does before the old one is retired. (#319)

## Behind the Scenes

- **[Task]** **Trial run of the new pre-check system** — Running the new lead pre-check alongside the old one to compare results before switching over. (#40)
- **[Task]** **Add caching to speed up surveys** — Introduces a faster data layer so surveys and offers load more quickly under heavy traffic. (#42)
- **[Task]** **Run new scheduled jobs alongside the old ones** — The new automated background jobs will run in parallel with the existing ones to confirm they match before any switch. (#43)
- **[Task]** **Retire low-risk background jobs** — Turning off older, lower-risk scheduled jobs once their replacements prove stable. (#44)
- **[Task]** **Retire mid-tier background jobs** — Switching off the next set of older stats jobs after the low-risk ones are confirmed working. (#45)
- **[Task]** **Retire the most critical background jobs** — Carefully switching off the most important legacy jobs last, with close monitoring and a quick fallback if needed. (#46)
- **[Task]** **Review an outdated stats job** — Checking whether an old stats-tracking job is still needed or can be safely retired. (#33)
- **[Task]** **Document rollback procedures** — Writing clear, tested steps to safely revert each system if something goes wrong. (#48)
- **[Task]** **Create troubleshooting guides** — Preparing step-by-step guides for the support team to handle common issues quickly. (#49)
- **[Task]** **Weekly parity progress scorecard** — An automated weekly report tracking how close the new platform is to matching the legacy one. (#323)
- **[Feature]** **Slackbot to file tasks from conversations** — A helper that turns action items from team chats into tracked work items automatically. (#272)
- **[Task]** **Run automated screen tests automatically** — Wiring the existing automated checks into the release process so admin-screen issues are caught before they reach you. (#376)
- **[Task]** **Improve test data cleanup and isolation** — Preventing leftover test data and conflicts so automated checks stay reliable. (#377)
- **[Task]** **Follow-ups from the automated-testing review** — A short list of improvements identified while auditing the automated test setup. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
