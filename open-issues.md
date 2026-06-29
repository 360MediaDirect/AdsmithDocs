# Open Issues — Plain-Language Overview

_Last updated 2026-06-29 17:56:16 UTC · 27 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Restore the missing dashboard sections** — High priority. Right now only the system overview loads. This brings back the campaign stats, top offers, and watch list sections from the previous system, and makes them respond to the date range you pick. (#240)
- **[Task]** **Custom date range on the dashboard filter** — Choosing "Custom" in the date filter will open a date picker with start and end dates, so you can view dashboard data for any period you like instead of only the preset options. (#58)
- **[Feature]** **New "Other Dashboard" monitoring views** — Adds dedicated views for "Offers with Legs" (offers with sustained performance) and CLP offer performance, with low-converting offers (under 30%) flagged for quick action. Also introduces a searchable history of changes so admins can see who paused an offer, adjusted caps, or updated settings, and when. (#256)
- **[Task]** **A consistent dashboard color scheme** — The dashboard will adopt a defined set of colors for cleaner, easier-to-read screens. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole admin between dark and light themes from your user menu, and your choice will stick between visits. Helpful for different lighting and personal comfort. (#59)
- **[Feature]** **Protection against two people overwriting the same record** — When two users open the same offer, flow, placement, or other record, the app will show a clear "locked by someone else" notice and warn you if the record changed while you had it open, so edits can no longer be silently lost. (#267)
- **[Task]** **Adopt comprehensive brand guidelines for AI output** — A single, detailed brand guide will be used as the main reference for AI-generated content, improving the quality and consistency of what's produced. (#264)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain-language label and inline help explaining what it controls and what its values mean, so it's no longer confusing to use. (#226)
- **[Task]** **Tidy up the Flow form's appearance** — A styling fix so the Flow form's text boxes, color pickers, checkboxes, and paired fields look polished and consistent with the Placement and Modal forms. (#152)

## Offers

- **[Task]** **Quick action links under each offer** — Adds handy links beneath each offer title (Edit, Quick Edit, Trash, View, Preview, Trends, Details). The Trends link opens an offer activity page with lead and revenue trends, date filtering, and a daily performance breakdown. (#252)
- **[Feature]** **Enforce required fields before a lead is pushed** — When a pre-ping is set to run before pushing data, leads that are missing required information will be stopped right away instead of being sent on and relying on the advertiser to reject them. (#218)

## Placements

- **[Feature]** **Better control over selected offers** — Selected offers will default to manual ordering, with drag-and-drop reordering, an "X" to remove an offer (so clicking is reserved for dragging), and the ability to filter the offer list by category. (#235)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — Critical, high priority. The Campaigns area from the previous system isn't yet available in New Adsmith Frontend. This adds it back so you can view, create, edit, and configure campaigns and their offer groups. (#200)

## Link Testing

- **[Bug]** **Show a proper error for invalid links** — Testing an invalid link currently dumps you onto the dashboard. This fix will instead show a clear failure message right in Link Testing. (#239)

## Users

- **[Task]** **Review of the Users area against the previous system** — A behind-the-scenes comparison documenting which Users features (such as bulk actions, last-login info, and password options) are still missing, so they can be prioritized and added. (#80)

## Behind the Scenes

- **[Feature]** **Up-to-the-minute "today" stats** — Lays the groundwork for showing current-day impressions, clicks, leads, and revenue (in Eastern Time) on the dashboard. (#34)
- **[Feature]** **Reliable historical stats** — Behind-the-scenes work to roll up daily totals so historical reporting stays accurate and fast. (#35)
- **[Task]** **Faster survey performance** — Adds a caching layer so survey-related data loads more quickly. High priority. (#42)
- **[Task]** **Safety testing of the new pre-ping system** — Runs the new and old pre-ping systems side by side to confirm results match before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Confirms each advertiser's pre-ping works correctly before the switchover. (#41)
- **[Task]** **Deploy new scheduled jobs alongside the old ones** — The new background jobs will run in parallel with the existing ones and be monitored for any differences. (#43)
- **[Task]** **Gradual switch-over of background jobs (first group)** — Retires a lower-risk set of older scheduled jobs once their replacements prove stable. (#44)
- **[Task]** **Gradual switch-over of background jobs (second group)** — Retires the next set of older stats-related jobs after a monitoring period. (#45)
- **[Task]** **Gradual switch-over of background jobs (critical group)** — Carefully retires the most important jobs (lead processing and offer cap resets) last, with close monitoring and the ability to roll back. (#46)
- **[Task]** **Review of an older stats job** — Assesses whether a legacy stats job is still needed or can be retired. (#33)
- **[Task]** **Documented rollback steps** — Prepares clear recovery procedures for each system in case something needs to be reversed. (#48)
- **[Task]** **Troubleshooting runbooks** — Creates step-by-step guides for handling common operational issues quickly. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 94900cccf9a7b3acb25443bbab588922c2cc2bff276c4d8ebadf6793ca8025fe -->
