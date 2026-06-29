# Open Issues — Plain-Language Overview

_Last updated 2026-06-29 19:33:54 UTC · 27 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against two people overwriting the same record** — When two admins open the same item (an offer, flow, placement, advertiser, and so on), the system will warn that someone else is editing it and prevent one person's changes from silently wiping out another's. You'll see a clear "locked by" notice and a prompt to reload if a record changed while you had it open. (#267)
- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole admin between dark and light appearance from your account menu or settings, and your choice will be remembered next time you log in. (#59)
- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link will show a proper error message instead of unexpectedly dropping you back on the dashboard. (#239)
- **[Task]** **Review of the Users area against the old system** — A documentation review comparing the new Users screens to the legacy version, so missing pieces (like bulk actions and extra columns) can be prioritized and added. (#80)
- **[Task]** **Adopt clear brand guidelines for AI-generated content** — A single, comprehensive brand guide will be used as the main reference for AI output, improving the quality and consistency of generated content. (#264)

## Dashboard

- **[Task]** **Restore missing dashboard sections** — Campaign stats, top offers, and watch lists will return to the dashboard, and the date range selector will update them, so you see your full performance picture again instead of just the system overview. (#240)
- **[Feature]** **New monitoring views and an activity log** — A new "Other Dashboard" area will add "Offers with Legs" and a CLP offers report that highlights offers converting under 30%, plus a searchable log of changes (like pausing offers or adjusting caps) showing who changed what and when. (#256)
- **[Task]** **Custom date range on the dashboard** — Choosing "Custom" in the date filter will open a start/end date picker so you can view dashboard data for any range you need, not just preset options. (#58)
- **[Task]** **A consistent dashboard color scheme** — A defined set of colors will be applied across the dashboard for better, more consistent readability. (#263)

## Offers & Campaigns

- **[Feature]** **Bring back the Campaigns module** — Campaign management, currently missing from the new platform, will be added so you can create, edit, and configure campaigns and their offer groups just like in the old admin. This is a high-priority gap. (#200)
- **[Feature]** **Block leads missing required pre-ping fields** — When a pre-ping runs before pushing data, leads missing required fields will be stopped right away instead of being sent out and relying on the advertiser to reject them. (#218)
- **[Task]** **Quick action links under each offer** — Each offer will show handy links like Edit, Quick Edit, Trash, View, Preview, Trends, and Details, with Trends opening an activity page showing lead and revenue trends over time. (#252)

## Flows

- **[Feature]** **Make the "Step order" setting understandable** — The Flow form's step order control will get a clear label and inline help explaining what it controls and what the values mean, so it's no longer confusing. (#226)
- **[Task]** **Fix the look of the Flow form** — Remaining styling issues on the Flow form (textareas, color pickers, checkboxes, and side-by-side field layouts) will be cleaned up so it matches the polished look of the Placement and Modal forms. (#152)

## Placements

- **[Feature]** **Easier offer ordering on placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by category, making it much simpler to arrange offers exactly how you want. (#235)

## Behind the Scenes

- **[Feature]** **Faster, accurate "today" stats** — Behind-the-scenes work to show up-to-the-hour figures for impressions, clicks, leads, and revenue in the dashboard's "today" view, with correct Eastern Time handling. (#34)
- **[Feature]** **Reliable historical reporting totals** — Maintenance to roll up day-by-day numbers automatically so historical reports stay accurate and quick to load. (#35)
- **[Feature]** **Per-advertiser pre-ping checks** — Each active advertiser's pre-ping setup will be validated to confirm fields and success rules work correctly before the new system takes over. (#41)
- **[Task]** **Side-by-side testing of the new pre-ping system** — The new and old pre-ping systems will run together and be compared to catch any differences before switching over. (#40)
- **[Task]** **Faster survey performance** — Behind-the-scenes caching will speed up surveys by keeping frequently used placement, offer, and cap information readily available. High priority. (#42)
- **[Task]** **Review an older stats job** — Checking whether a legacy statistics job is still needed or can be retired. (#33)
- **[Task]** **Run new scheduled jobs alongside the old ones** — The new automated jobs will run in parallel with the existing ones in production, with daily monitoring to confirm they match. (#43)
- **[Task]** **Phased switch-over of scheduled jobs (lower risk)** — Gradually retiring the least critical legacy jobs once their replacements prove stable. (#44)
- **[Task]** **Phased switch-over of scheduled jobs (medium risk)** — Retiring the next group of legacy jobs after the first group runs cleanly. (#45)
- **[Task]** **Phased switch-over of scheduled jobs (critical)** — Carefully retiring the most important legacy jobs last, with close monitoring and the ability to revert immediately. (#46)
- **[Task]** **Documented recovery steps** — Writing and testing clear rollback procedures for each major system in case something needs to be reverted. (#48)
- **[Task]** **Troubleshooting guides for support** — Creating step-by-step guides for handling common issues like lead processing or stats problems, so they can be resolved quickly. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 94900cccf9a7b3acb25443bbab588922c2cc2bff276c4d8ebadf6793ca8025fe -->
