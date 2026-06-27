# Open Issues — Plain-Language Overview

_Last updated 2026-06-27 20:23:50 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Review an old scheduled stats job** — We're checking whether a legacy background job that tracks certain traffic stats is still needed or can be retired, so the system stays lean. (#33)
- **[Feature]** **Automatic rollup of stats into history** — Behind-the-scenes work to roll up live activity into daily historical totals, keeping long-term reports accurate and fast. (#35)
- **[Task]** **Safety testing for pre-ping checks** — We'll run the new lead pre-screening process alongside the existing one and compare results, so we can switch over with confidence that nothing breaks. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — We're verifying the lead pre-screening setup works correctly for each active advertiser before going live, preventing surprises after the switch. (#41)
- **[Task]** **Faster Survey Engine performance** — High-priority groundwork to cache frequently used survey and offer settings so surveys load and respond more quickly. (#42)
- **[Task]** **Run new scheduled jobs alongside the old ones** — We'll operate the new and existing background jobs in parallel and watch for any differences, ensuring a smooth, low-risk transition. (#43)
- **[Task]** **Retire older background jobs (group 3)** — Once the replacements are proven stable, we'll turn off a set of lower-risk legacy survey-stats jobs, with the ability to switch back if needed. (#44)
- **[Task]** **Retire mid-tier background jobs (group 2)** — Turning off another set of legacy stats jobs after the previous group is confirmed stable, monitored closely for a week. (#45)
- **[Task]** **Retire the most critical background jobs (group 1)** — The final, most sensitive jobs (lead processing and offer cap resets) will be switched over last, with close monitoring and instant rollback ready. (#46)
- **[Task]** **Document how to roll back safely** — Writing clear step-by-step recovery procedures for each major system, so any issue can be reversed quickly. (#48)
- **[Task]** **Create troubleshooting guides** — Preparing practical guides for handling common issues (lead processing, stats, offer caps, and more), so problems get resolved faster. (#49)

## Dashboard

- **[Task]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will be back on the Dashboard, and the date-range selector will update them. This is high priority since only the system overview currently loads. (#240)
- **[Feature]** **"Today" figures powered by live data** — The Dashboard's "today" view will show up-to-the-hour impressions, clicks, leads, and revenue, with correct Eastern Time handling. (#34)
- **[Feature]** **New "Other Dashboard" views and an activity log** — You'll get dedicated views for offers with sustained performance and for CLP offer performance (flagging anything converting under 30%), plus a searchable log of changes like pausing offers or editing caps. (#256)
- **[Task]** **Custom date range on the Dashboard** — Selecting "Custom" in the date filter will open a start/end date picker so you can view data for exactly the range you want. (#58)
- **[Task]** **Consistent, easier-to-read color scheme** — The Dashboard will adopt a defined color palette applied consistently across views for better readability. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole Admin between dark and light themes, with your choice remembered for next time. A nice comfort and accessibility improvement. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, the app will warn you if someone else changed it and prevent accidental overwrites, with a clear "locked by" notice while another user is editing. (#267)
- **[Task]** **Users area: closing the gap with the old system** — A review of the Users screens against the legacy version to identify missing capabilities (like bulk actions and extra columns) and plan what to bring over. (#80)
- **[Task]** **Brand guidelines to improve AI output** — We'll establish a thorough brand-guidelines document and use it as the main input for AI-generated content, improving quality and consistency. (#264)

## Flows

- **[Task]** **Fix unstyled areas on the Flow form** — Parts of the Flow form currently look broken or unstyled (plain text boxes, unstyled color pickers, fields stacking awkwardly). This cleans up the form's appearance to match other screens. (#152)
- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain-language label and inline help explaining what it controls, so it's no longer confusing to use. (#226)

## Placements

- **[Feature]** **Better control of selected offers** — Selected offers will default to manual ordering with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — A high-priority addition so you can view, create, edit, and configure campaigns and offer groups in New Adsmith Frontend, matching what the old admin offered. (#200)

## Pre-Pings

- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping runs before pushing data, leads missing required fields will be stopped right away instead of being sent and relying on the advertiser to catch them. (#218)

## Link Testing

- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will show a proper error message in the Link Testing screen instead of sending you to the Dashboard. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
