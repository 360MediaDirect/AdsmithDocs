# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 01:41:03 UTC · 32 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Feature]** **Up-to-the-hour numbers for "today"** — Lays the groundwork for the Dashboard to show today's impressions, clicks, leads, and revenue as they happen, in the correct (Eastern) time zone. (#34)
- **[Feature]** **Reliable historical reporting totals** — Behind-the-scenes work to roll up daily figures so longer-range reports load accurately and consistently. (#35)
- **[Task]** **Review of an older statistics job** — Checking whether a legacy reporting process is still needed or can be retired to keep things tidy. (#33)
- **[Task]** **Safety testing of the new lead pre-check system** — Running the new and old systems side by side to confirm the new one matches before any switchover. (#40)
- **[Feature]** **Advertiser-by-advertiser pre-check validation** — Confirming each active advertiser's lead pre-check works correctly before going live. (#41)
- **[Task]** **Faster Surveys through added caching** — A high-priority performance improvement so survey pages and offer rules load more quickly. (#42)
- **[Task]** **Parallel running of new scheduled jobs** — Running new and existing automated jobs together to confirm they produce the same results before relying on the new ones. (#43)
- **[Task]** **Phased switchover of scheduled jobs (lower-risk batch)** — Retiring the least-critical legacy survey-stats job once its replacement proves stable. (#44)
- **[Task]** **Phased switchover of scheduled jobs (mid-tier batch)** — Retiring several reporting and stats jobs after a week of stable monitoring. (#45)
- **[Task]** **Phased switchover of scheduled jobs (critical batch)** — Carefully retiring the most important lead-processing and offer-cap jobs last, with the ability to roll back instantly. (#46)
- **[Task]** **Written rollback procedures** — Documenting how to safely revert each major system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Step-by-step guides so the team can quickly resolve lead, stats, offer-cap, and connection problems. (#49)
- **[Task]** **A safe staging environment with May & June data** — Sets up a separate testing area loaded with real-world data so reports can be verified without touching live information. (#270)
- **[Task]** **Investigation into report number differences vs. the legacy system** — Comparing old and new reporting on the same data to find and explain any mismatches, so you can trust the figures. (#271)

## Dashboard

- **[Task]** **Restore missing Dashboard sections** — A high-priority fix to bring back campaign stats, top offers, and watch lists so the Dashboard shows the full picture again, with the date range driving the data. (#240)
- **[Task]** **Custom date range on the Dashboard** — Choosing "Custom" will open a date picker with start and end dates, so you can view data for any specific period instead of just preset ranges. (#58)
- **[Feature]** **Light and dark mode toggle** — You'll be able to switch between dark and light themes to suit your environment and preferences, with your choice remembered next time. (#59)
- **[Feature]** **New "Other Dashboard" views and activity log** — Adds an "Offers with Legs" view and a CLP performance view (highlighting offers converting under 30%), plus a searchable log of who changed what and when. (#256)
- **[Feature]** **Change report dates without editing the web address** — Adds proper date controls to the Dashboard toolbar so you no longer have to hand-edit the address bar to pull a specific day or range. (#268)
- **[Feature]** **Dashboard links open in a new tab** — Clicking a Dashboard link will open it in a new tab so you don't lose your place or current view. (#269)

## Offers & Placements

- **[Feature]** **Bring back the Campaigns module** — A high-priority addition to restore creating, editing, and managing campaigns and their offer groups, matching what's available in the legacy system. (#200)
- **[Bug]** **Hidden offers no longer slip through as leads** — Fixes a high-priority issue where an offer hidden by its pre-check could still be auto-submitted and recorded as a successful lead. (#274)
- **[Feature]** **Enforce required fields before a lead is pushed** — When a pre-ping is set to run before sending data, leads missing required information will be stopped up front rather than relying on the advertiser to catch it. (#218)
- **[Feature]** **Reorder and filter offers on Placements** — You'll be able to set offers to manual order, drag them into the sequence you want, remove one with an "X," and filter the offer list by taxonomy. (#235)
- **[Task]** **Quick action links beneath each offer** — Adds familiar links like Edit, Quick Edit, Trash, View, Preview, Trends, and Details, with Trends opening an offer activity page showing lead and revenue trends over time. (#252)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When you open a record to edit, others will see it's locked, and saving will warn you if someone changed it first, so no one's work gets silently lost. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will show a proper failure message instead of unexpectedly sending you to the Dashboard. (#239)
- **[Task]** **Users screen review against the legacy version** — A review of the Users area to identify which features (like bulk actions and login details) are still missing compared to the old system. (#80)
- **[Task]** **Stronger brand guidelines to improve AI output** — Establishing a single, detailed brand guide so AI-generated content stays consistent and on-brand. (#264)
- **[Feature]** **Automatic issue creation from team chats** — A helper that turns action items from conversations into tracked tasks automatically, reducing manual copy-and-paste. (#272)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The setting will get a plain-language label and helpful inline text explaining what it controls, so you no longer have to guess what it does. (#226)
- **[Task]** **Tidy up the Flow form's appearance** — Cleans up styling issues so text boxes, color pickers, checkboxes, and paired fields look polished and lay out correctly, like the other forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: faecd53a4dfcde97e324518cd3e13868b7519c0b955be87856fa9ce778878ae6 -->
