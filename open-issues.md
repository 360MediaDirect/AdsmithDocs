# Open Issues — Plain-Language Overview

_Last updated 2026-06-26 13:40:17 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker on the date filter** — When you choose "Custom" in the Dashboard date filter, you'll get start and end date pickers (with validation and an Apply button) so you can view results for any range you like, not just the preset options. (#58)
- **[Task]** **Bring back the missing Dashboard sections** — A high-priority fix to restore the campaign stats, top offers, and watch list sections that aren't loading today, with the date range filter properly updating them. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds "Offers with Legs" and "CLP Performance" views (flagging low-converting offers under 30%) plus a searchable log of changes like pausing offers or adjusting caps, so you can monitor performance and see who changed what and when. (#256)
- **[Task]** **Consistent dashboard colors** — A defined color palette will be applied across the Dashboard to make charts and figures easier to read at a glance. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole Admin between dark and light themes from your user menu, with your choice remembered next time you sign in. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, the app will warn you if someone else is already editing it and prevent one person's save from silently wiping out another's changes. (#267)
- **[Bug]** **Invalid links should show a clear error** — Testing a bad link currently dumps you on the Dashboard; once fixed, you'll see a clear failure message in the Link Testing screen instead. (#239)
- **[Task]** **Brand guidelines to improve AI output** — Establishing a thorough brand guidelines document to feed the AI, so generated content comes out more on-brand and consistent. (#264)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Fixes unstyled text boxes, color pickers, checkboxes, and fields that stack vertically instead of sitting side by side, so the Flow form looks polished and matches the Placement and Modal forms. (#152)
- **[Feature]** **Make the "Step order" setting understandable** — Adds a clear label and inline help explaining what Step order controls and what its values mean, so you no longer have to guess what the field does. (#226)

## Offers & Placements

- **[Feature]** **Manually arrange offers on a Placement** — Selected offers will default to manual order with drag-and-drop reordering, a clear "X" to remove an offer, and the ability to filter the offer list by category, giving you full control over offer ordering. (#235)
- **[Feature]** **Enforce required fields before sending a lead** — For pre-pings that run before a data push, missing required fields will stop the lead right away instead of letting an incomplete lead slip through. (#218)

## Campaigns

- **[Feature]** **Add the Campaigns module** — A high-priority addition that brings campaign management into New Adsmith Frontend, letting you view, create, edit, and configure campaigns and offer groups just as you can in the legacy system. (#200)

## Users

- **[Task]** **Users screen comparison and gap review** — A documentation review comparing the new Users area to the legacy version, identifying missing pieces (like bulk actions and extra columns) to guide upcoming improvements. (#80)

## Behind the Scenes

- **[Feature]** **Faster, accurate "today" stats** — Behind-the-scenes work so the Dashboard's "today" figures (impressions, clicks, leads, revenue) are pulled and totaled correctly in Eastern Time. (#34)
- **[Feature]** **Reliable historical reporting** — A new background process rolls up daily totals so historical reports stay accurate and quick to load. (#35)
- **[Feature]** **Pre-ping checks verified for every advertiser** — Confirming each advertiser's pre-ping works correctly before switching over, so lead validation behaves as expected. (#41)
- **[Task]** **Reviewing an older stats job** — Checking whether a legacy stats process is still needed or can be retired, with the decision documented. (#33)
- **[Task]** **Side-by-side pre-ping testing** — Running the new pre-ping system alongside the existing one to compare results and catch any differences before the switch. (#40)
- **[Task]** **Speed improvements for surveys** — Adding a caching layer so survey placements, offers, and caps load faster in real time. High priority. (#42)
- **[Task]** **Running new background jobs in parallel** — Deploying the new scheduled jobs to run alongside the current ones and monitoring daily for any discrepancies. (#43)
- **[Task]** **Phased switch-over of survey stats jobs** — Retiring the older survey-stats job once its replacement is proven stable, with the ability to revert if needed. (#44)
- **[Task]** **Phased switch-over of stats and reporting jobs** — Retiring several stats aggregation and reporting jobs after a monitoring period, ready to revert if issues appear. (#45)
- **[Task]** **Phased switch-over of critical lead and cap jobs** — Carefully retiring the most critical lead-processing and offer-cap jobs last, with close monitoring and instant rollback on standby. (#46)
- **[Task]** **Documented recovery steps** — Writing and testing clear rollback procedures for each major system so issues can be reversed quickly and safely. (#48)
- **[Task]** **Troubleshooting guides for the support team** — Creating step-by-step guides for handling common issues like lead processing or stats problems, for faster resolution. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
