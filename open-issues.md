# Open Issues — Plain-Language Overview

_Last updated 2026-06-27 14:32:19 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

These are infrastructure and reliability updates. Most won't change what you see day to day, but they keep New Adsmith Frontend fast, accurate, and dependable.

- **[Feature]** **Faster "today" numbers** — Behind-the-scenes work to pull up-to-the-minute impressions, clicks, leads, and revenue for the current day so the Dashboard's "today" view stays current and correct. (#34)
- **[Feature]** **Reliable historical reporting totals** — Daily and hourly figures will be rolled up automatically so longer-term reports load accurate totals. (#35)
- **[Task]** **Speeding up Surveys with caching** — High priority work to make survey and offer information load faster during live traffic. (#42)
- **[Task]** **Reviewing an older background job** — Checking whether an existing stats routine is still needed or can be retired to keep things tidy. (#33)
- **[Task]** **Safety testing for pre-ping** — The new pre-ping process will run alongside the old one and be compared, so nothing changes for advertisers until results match. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Each active advertiser's pre-ping setup will be verified before switching over, preventing surprises. (#41)
- **[Task]** **Rolling out new scheduled jobs in parallel** — New automated routines run side by side with the old ones, watched daily for any differences before fully switching. (#43)
- **[Task]** **Switching over lower-risk scheduled jobs** — Retiring an older survey-stats routine after its replacement proves stable. (#44)
- **[Task]** **Switching over mid-tier scheduled jobs** — Retiring several stats and reporting routines once confirmed stable, with close monitoring. (#45)
- **[Task]** **Switching over the most critical scheduled jobs** — Carefully retiring the core lead-processing and offer-cap routines last, with the ability to roll back instantly. (#46)
- **[Task]** **Documented recovery steps** — Clear, tested procedures to quickly restore each system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides for support staff** — Step-by-step guides for handling common issues like lead-processing or stats problems. (#49)

## Dashboard

- **[Task]** **Restore missing Dashboard sections** — High priority fix to bring back campaign stats, top offers, and watch lists, with the date range properly updating them. Right now only the system overview loads. (#240)
- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open a start/end date picker so you can view Dashboard data for any specific range, not just the preset options. (#58)
- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the interface between dark and light themes to suit your environment and preference, with your choice remembered next time. (#59)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds views for "Offers with Legs" and CLP offer performance (flagging offers converting under 30%), plus a searchable record of who changed what and when. (#256)
- **[Task]** **Consistent Dashboard color scheme** — A defined set of colors will be applied across the Dashboard for cleaner, easier-to-read screens. (#263)

## General / Across the App

- **[Feature]** **Prevent two people overwriting each other's edits** — When someone opens a record for editing, others will see it's locked and by whom, and you'll be warned if a record changed while you had it open — so no one's work gets silently lost. Works across offers, flows, placements, advertisers, and more. (#267)
- **[Task]** **Users area feature review** — A documentation review comparing the old Users area to the new one to identify what still needs to be added, such as bulk actions and extra columns. (#80)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper error message instead of unexpectedly sending you to the Dashboard. (#239)
- **[Task]** **Brand guidelines for AI output** — Establishing a thorough brand-guidelines document to use as the main input for AI-generated content, improving the quality of results. (#264)

## Flows

- **[Task]** **Fix the look of the Flow form** — Cleans up styling on the Flow form so text boxes, color pickers, checkboxes, and paired fields display properly instead of looking unstyled or misaligned. (#152)
- **[Feature]** **Make the "Step order" setting understandable** — A clearer label and inline help will explain what "Step order" controls and what its values do, so it's no longer confusing. (#226)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — A critical, high-priority addition to recreate campaign management in New Adsmith Frontend, letting you view, create, edit, and configure campaigns and offer groups as you could in the old system. (#200)

## Placements

- **[Feature]** **Better offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter offers by taxonomy. (#235)

## Pre-Pings

- **[Feature]** **Enforce required fields before sending leads** — When a pre-ping runs before pushing data, leads missing required fields will be stopped right away rather than sent on, helping keep out incomplete or malformed leads. (#218)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
