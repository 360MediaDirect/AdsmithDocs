# Open Issues — Plain-Language Overview

_Last updated 2026-09-15 06:07:29 UTC · 35 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Review an older stats job for retirement** — We're checking whether an aging background job that tracks certain stats is still needed or can be safely retired. No visible change for you. (#33)
- **[Feature]** **Faster, more reliable historical stats** — We're setting up automatic daily summarizing of performance data so historical reports stay quick and accurate. (#35)
- **[Task]** **Safely test the new lead-checking system** — The new lead pre-check system is being run side-by-side with the old one to confirm they agree before we switch over. (#40)
- **[Task]** **Speed boost for surveys** — We're adding a behind-the-scenes fast-access layer so survey pages load more quickly. (#42)
- **[Task]** **Run new background jobs in parallel** — New automated background jobs are being run alongside the current ones to make sure they behave identically before we rely on them. (#43)
- **[Task]** **Retire an older survey-stats job** — An older survey stats job is being switched off now that its replacement has proven reliable. (#44)
- **[Task]** **Retire a batch of older stats jobs** — Several more older background stats jobs are being switched off after their replacements proved stable. (#45)
- **[Task]** **Retire the most critical background jobs** — The most important background jobs (like lead processing and offer cap resets) are being moved to their new versions, with careful monitoring and a quick way to revert. (#46)
- **[Task]** **Document how to undo changes** — We're writing clear steps for quickly reverting each system if something goes wrong. (#48)
- **[Task]** **Create troubleshooting guides** — Step-by-step guides are being written so common issues can be resolved faster. (#49)
- **[Feature]** **Turn conversations into tracked work automatically** — An internal helper that captures action items from team chats and files them as tracked tasks, cutting manual copy-paste. (#272)
- **[Task]** **Weekly "match the old system" report** — An automated weekly scorecard tracks how closely New Adsmith Frontend matches the older system, so gaps are spotted early. (#323)
- **[Bug]** **Prevent lead submissions from timing out** — When a lead submission triggers several outside checks at once, we're making sure it still completes cleanly instead of failing. (#367)
- **[Bug]** **Fix campaign offer-group data loading** — Correcting a data-reading issue so campaign offer groups always load reliably. (#372)
- **[Task]** **Run automated tests on every update** — Our full automated test suite will run automatically after each release, catching admin-area problems earlier. (#376)
- **[Task]** **Keep test data tidy** — Improving how automated tests clean up leftover test records so shared test environments stay reliable. (#377)
- **[Task]** **Tune up our automated testing setup** — A broader review of the automated testing framework, with several improvements already underway. (#379)

## Offers

- **[Bug]** **Some saved offer options weren't taking effect** — A number of saved offer settings weren't reaching the live offer. This fix makes sure every option you set is actually applied (or is cleaned up if it does nothing). (#295)
- **[Bug]** **Auto-register offers now respect duplicate and conflict rules** — Auto-registering offers will properly skip cases that duplicate or conflict with other offers, matching the older system's behavior. (#355)
- **[Bug]** **"Conflicting Offers" rules now actually enforced** — Offers whose conflicting-offer list was set in the new admin will now correctly block conflicting offers instead of silently ignoring the rule. (#358)
- **[Bug]** **Manually selected offers now carry over correctly** — For Manual-delivery placements, your hand-picked offer list (and its order) will display correctly instead of showing the wrong or empty set. (#370)
- **[Feature]** **Preview your unsaved edits** — On placement and offer edit pages, Preview will show your current in-progress changes rather than only the last saved version, so you no longer have to save first to see them. (#292)
- **[Feature]** **Predict how a new offer might perform** — An exploratory tool to estimate a new offer's likely performance from your historical offer data, giving a data-based gut-check at intake. (#322)
- **[Feature]** **Decide the future of the HubSpot List ID field** — The HubSpot List ID field currently does nothing behind the scenes; we're deciding whether to build the full integration or remove the unused field. (#362)

## General / Across the App

- **[Task]** **Compare the Users area to the old system** — A thorough review of the Users admin screen versus the legacy system to identify missing features and prioritize what to add back. (#80)
- **[Feature]** **Remove admin controls that do nothing** — Certain admin settings currently save but have no effect; we're hiding or removing them (or wiring them up) so the interface only shows controls that actually work. (#296)
- **[Task]** **Track overall progress toward matching the old system** — A single, high-level view that rolls up all the work needed to reach and hold parity with the legacy system until it's retired. (#319)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — Bringing back the "after success" delivery steps some clients relied on, so post-conversion handoffs work as they did before. (#327)
- **[Feature]** **Port custom lead-validation checks** — Restoring the custom, per-client lead pre-checks from the old system so those clients' validation rules run again on the new platform. (#338)
- **[Bug]** **Real lead validation for manually processed leads** — Leads processed through the manual/broker path will be checked against the real validation service instead of always being marked valid. (#366)

## Dashboard & Reports

- **[Feature]** **Accurate "today" figures on the Dashboard** — The Dashboard's "today" view will show up-to-date impressions, clicks, leads, and revenue for the current day. (#34)
- **[Task]** **Investigate report numbers that don't match the old system** — We're comparing report figures against the legacy system on a fixed date range to find and fix any differences. (#271)

## Surveys

- **[Feature]** **Design-tab settings that fully carry through to surveys** — Every customization option on the Design tab will show up in the actual survey view, and we're auditing all entity form options to make sure none are left disconnected. (#288)

## Advertisers

- **[Feature]** **Verify lead pre-checks for each advertiser** — Confirming that each active advertiser's lead pre-check works correctly, with the right field mapping, before switching over. (#41)

## Modals

- **[Feature]** **Refreshed "voucher" style visitor modal** — The visitor modal will get the legacy voucher look: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with clear "Claim Offer" and "No Thanks" options, and a trusted footer. (#386)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
