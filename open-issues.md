# Open Issues — Plain-Language Overview

_Last updated 2026-06-26 05:25:58 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Decide the future of an older stats job** — A review to confirm whether one of the older background processes that tracks certain performance numbers is still needed or can be retired, so reporting stays accurate without duplicate work. (#33)
- **[Feature]** **Up-to-the-minute numbers for "today"** — Behind-the-scenes work so the Dashboard's "today" view can show current impressions, clicks, leads, and revenue in near real time, with correct Eastern Time handling. (#34)
- **[Feature]** **Faster historical reporting** — Daily and hourly totals will be rolled up automatically in the background, making it quicker to pull up past performance. (#35)
- **[Task]** **Safety testing for pre-ping before switchover** — The new pre-ping system will run side-by-side with the old one and the results compared, so any differences are caught and fixed before it goes fully live. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Each active advertiser's pre-ping setup will be verified for correct field mapping and pass/fail rules before the switchover, reducing the chance of surprises. (#41)
- **[Task]** **Speed boost for the Survey engine** — A new caching layer will make survey-related lookups faster, improving responsiveness when offers and targeting rules are loaded. This is high priority. (#42)
- **[Task]** **Run new scheduled jobs alongside the old ones** — The replacement background jobs will run in parallel with the current ones and be monitored daily, so nothing is missed during the transition. (#43)
- **[Task]** **Retire lower-risk scheduled jobs (Tier 3)** — Once their replacements are proven stable, the least critical legacy background jobs will be switched off, with monitoring in place to revert if needed. (#44)
- **[Task]** **Retire mid-tier scheduled jobs (Tier 2)** — Several stats-related legacy jobs will be turned off after the lower tier is confirmed stable, monitored for a week to be safe. (#45)
- **[Task]** **Retire the most critical scheduled jobs (Tier 1)** — The most important legacy jobs (lead processing and offer-cap reset) will be switched off last, with close monitoring and a fast rollback option. This is critical work. (#46)
- **[Task]** **Documented rollback steps** — Clear instructions for safely reverting each major system if something goes wrong, so issues can be resolved quickly. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Step-by-step guides for resolving things like lead-processing or stats problems, helping support respond faster when issues arise. (#49)

## Dashboard

- **[Task]** **Custom date range on the Dashboard** — Choosing "Custom" in the date filter will open a start/end date picker, so you can view Dashboard data for exactly the period you want instead of only preset ranges. (#58)
- **[Task]** **Bring back missing Dashboard sections** — Campaign stats, top offers, and watch lists will be restored to the Dashboard, and the date-range selector will update them so you see complete, current data again. This is high priority. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds views for offers with sustained performance and CLP offer performance (flagging those converting under 30%), plus a searchable log of every offer change and who made it, for easier monitoring and auditing. (#256)
- **[Task]** **Consistent Dashboard color scheme** — A defined color palette will be applied across the Dashboard for cleaner, more readable visuals. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the entire Admin between dark and light themes, with your choice remembered next time you sign in. (#59)
- **[Feature]** **Prevent two people from overwriting each other** — When you open a record to edit, others will see it's being edited, and you'll be warned if someone changed it since you opened it, so edits no longer get silently lost. (#267)
- **[Bug]** **Clear error for invalid links in Link Testing** — Testing an invalid link will show a proper error message instead of unexpectedly sending you to the Dashboard. (#239)
- **[Task]** **Brand guidelines to improve AI output** — A complete brand-guidelines document will be created and used as the main reference for AI-generated content, improving the quality and consistency of results. (#264)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Cleans up the Flow form so text boxes, color pickers, checkboxes, and paired fields display correctly instead of looking unstyled or stacked awkwardly. (#152)
- **[Feature]** **Make the "Step order" setting understandable** — The Step order control will get a clearer label and inline help explaining what it does and what its values mean, so it's no longer confusing. (#226)

## Campaigns

- **[Feature]** **Add the Campaigns module** — Brings the Campaigns area into New Adsmith Frontend so you can view, create, edit, and configure campaigns and their offer groups, matching what's available in the legacy system. This is high priority. (#200)

## Placements

- **[Feature]** **Better control over offer order in Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by category, making it much easier to manage. (#235)

## Pre-Pings

- **[Feature]** **Enforce required fields before sending** — When a pre-ping runs before a data push, leads missing required fields will be stopped right away instead of being sent on, helping prevent incomplete leads from slipping through. (#218)

## Users

- **[Task]** **Review of the Users area vs. the legacy system** — A documented comparison identifying which Users features still need to be added (such as bulk actions and certain columns), guiding what to build next. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
