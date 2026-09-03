# Open Issues — Plain-Language Overview

_Last updated 2026-09-03 06:07:54 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Review an older stats job** — We're checking whether a legacy automated stats routine is still needed or can be safely retired. Purely behind-the-scenes housekeeping with no visible change for you. (#33)
- **[Feature]** **Automatic daily stats roll-ups** — A new background process will summarize activity into daily totals so historical reports load quickly and reliably. (#35)
- **[Task]** **Faster surveys** — We're adding a caching layer so survey settings and offers load faster for visitors. (#42)
- **[Task]** **Run new automated jobs alongside the old ones** — The new background jobs will run in parallel with the current ones so we can confirm they produce matching results before switching over. (#43)
- **[Task]** **Retire older background jobs (group 3)** — Turning off a first, low-risk set of legacy automated jobs once their replacements prove stable. (#44)
- **[Task]** **Retire background jobs (group 2)** — Turning off the next set of legacy stats jobs after a monitoring period. (#45)
- **[Task]** **Retire the most critical background jobs (group 1)** — Carefully switching off the last and most important legacy jobs, with the ability to roll back immediately if anything looks off. (#46)
- **[Task]** **Recovery procedures** — Writing clear step-by-step instructions for safely undoing changes if a problem appears, so issues can be resolved quickly. (#48)
- **[Task]** **Troubleshooting guides** — Creating quick-reference guides for common issues so problems get diagnosed and fixed faster. (#49)
- **[Feature]** **Turn Slack conversations into tracked tasks** — A helper that reads designated Slack channels and automatically files the action items as tracked issues, saving manual copy-and-paste. (#272)
- **[Task]** **Weekly progress scorecard** — An automated weekly report that tracks how close the new platform is to matching the legacy system, so nothing slips through the cracks. (#323)
- **[Task]** **Automated testing before release** — We're wiring the full automated test suite into the release process so admin-area problems get caught before they reach you. (#376)
- **[Task]** **Cleaner test data handling** — Improving how automated tests clean up after themselves, which reduces false alarms and keeps testing reliable. (#377)
- **[Task]** **Testing review follow-ups** — A tracked list of improvements from a review of our automated tests, aimed at making our safety net more trustworthy. (#379)

## Offers

- **[Bug]** **Saved offer settings that weren't reaching live ads** — Several offer options were being saved but never applied to what visitors actually saw. This fix makes those settings take effect. (#295)
- **[Feature]** **Automatic performance projections for new offers** — When a new offer comes in, you'll get a data-driven estimate of how it's likely to perform based on your own history, replacing today's manual gut-check. (#322)
- **[Bug]** **Auto-register offers now respect the rules** — Automatically-firing offers were skipping duplicate and conflict checks. This fix makes them follow the same eligibility rules as regular offers. (#355)
- **[Bug]** **Conflicting Offers rule now enforced** — For offers whose "Conflicting Offers" list was set in the current admin, that rule was silently doing nothing. This fix makes the exclusion actually work. (#358)
- **[Feature]** **Decide the fate of the HubSpot List ID field** — This offer field currently does nothing behind the scenes. We'll either build a real HubSpot connection or remove the field so it isn't misleading. (#362)

## General / Across the App

- **[Task]** **Users screen gap review** — A detailed comparison of the old and new user-management screens to identify missing pieces like bulk actions, last-login, and two-factor status, so we can close the gaps. (#80)
- **[Feature]** **Remove admin controls that do nothing** — Some settings look active but have no effect. We'll hide or remove them so the admin area only shows controls that actually work. (#296)
- **[Task]** **Overall legacy parity tracking** — A single master view that rolls up all the work needed to fully match the legacy system, so progress is visible in one place. (#319)
- **[Bug]** **Correct campaign offer counts** — A data-reading quirk could cause campaign offer-group counts to come back empty. This fix makes those counts reliable. (#372)

## Placements

- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show your current edits instead of only the last saved version, so you no longer have to save just to preview. (#292)
- **[Bug]** **Manually selected offers now show correctly** — On manual-delivery placements, the hand-picked offer list wasn't carrying over, so the wrong or no offers appeared. This fix restores the correct selected offers and their order. (#370)
- **[Bug]** **Tracking pixel placeholder fix** — Pixels set up with the example shown in the app were sending broken values to advertisers. This fix makes those placeholders resolve correctly so attribution data stays accurate. (#384)

## Data Clients

- **[Feature]** **Restore post-conversion delivery steps** — The legacy "after success" delivery actions for certain clients are being brought over so those clients keep receiving leads as before. (#327)
- **[Feature]** **Bring over custom pre-check validations** — Many clients rely on custom serve-time checks that don't yet run on the new platform. We're porting those so leads are validated the way they were before. (#338)
- **[Bug]** **Real lead validation in the manual/broker lead flow** — The manual and broker lead pipeline was reporting a validation result that wasn't actually being checked. This fix makes it perform the real check, matching the main flow. (#366)

## Reports

- **[Feature]** **Today's numbers on the Dashboard** — The Dashboard will show up-to-the-hour totals for today's impressions, clicks, leads, and revenue, correctly adjusted for Eastern Time. (#34)
- **[Task]** **Investigate report figures that don't match the old system** — We're comparing report numbers between the old and new platforms on the same date range to find and fix any discrepancies, so you can trust the figures. (#271)

## Surveys

- **[Feature]** **Design tab settings that actually apply** — We're making sure every option on the Design tab is reflected in the live survey, and auditing all form options across entities so nothing is a dead setting. (#288)
- **[Bug]** **Prevent lead submissions from timing out** — In rare cases, several checks running one after another could take too long and drop a submission. This fix ensures submissions finish cleanly instead of failing. (#367)

## Advertisers

- **[Task]** **Validate the new pre-ping before switching over** — We'll run the new pre-ping side by side with the old one to compare results and response times, fixing any differences before the switch. (#40)
- **[Feature]** **Check pre-ping for each advertiser** — We'll confirm every active advertiser's pre-ping works correctly and maps fields properly before going live. (#41)

## Modals

- **[Feature]** **Voucher-style visitor modal redesign** — The visitor modal will get the legacy "voucher" look: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with clear Claim and No Thanks options, and a trusted footer. (#386)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
