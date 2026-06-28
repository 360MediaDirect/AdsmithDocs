# Open Issues — Plain-Language Overview

_Last updated 2026-06-28 14:34:50 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

These items are infrastructure and maintenance work. They keep New Adsmith Frontend fast and reliable, but won't change how the screens look day to day.

- **[Feature]** **Up-to-date "today" numbers** — Lays the groundwork for showing current-day impressions, clicks, leads, and revenue in near real time, with the correct Eastern Time handling. (#34)
- **[Feature]** **Daily history roll-ups** — Bundles live activity into clean daily totals so historical reports stay accurate and quick to load. (#35)
- **[Task]** **Faster survey loading** — Adds a high-priority speed-up layer for the Survey engine so placements, offers, and caps respond more quickly. (#42)
- **[Task]** **Side-by-side test of the new pre-ping system** — Runs the new and old systems together to confirm the new one behaves identically before it takes over. (#40)
- **[Task]** **Run new scheduled jobs alongside the old ones** — Operates the new automated background jobs in parallel so they can be checked daily for any differences. (#43)
- **[Task]** **Switch over low-risk background jobs** — Retires the first group of older automated tasks once their replacements have proven stable. (#44)
- **[Task]** **Switch over mid-tier background jobs** — Retires the next group of stats-related automated tasks after a monitoring period. (#45)
- **[Task]** **Switch over the most critical background jobs** — Carefully retires the highest-importance automated tasks, with a quick way to undo if anything looks off. (#46)
- **[Task]** **Review of an older statistics job** — Decides whether a legacy sub-ID tracking process is still needed or can be safely retired. (#33)
- **[Task]** **Safe rollback steps** — Documents how to quickly reverse each system change if a problem appears. (#48)
- **[Task]** **Troubleshooting guides** — Creates step-by-step guides for handling common issues like lead processing, stats, and offer cap resets. (#49)

## General / Across the App

- **[Feature]** **Bring back the Campaigns module** — A high-priority gap: you'll be able to create, edit, and manage campaigns and offer groups in New Adsmith Frontend, matching what the old admin offered. (#200)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record you're already editing, you'll see a clear "locked by" notice, and saves will warn you if the record changed since you opened it — so no one's work is silently lost. This will apply across all entity screens. (#267)
- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, a clear "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)
- **[Bug]** **Link testing should show a real error** — Testing an invalid link currently dumps you on the dashboard; instead you'll get a clear failure message right in the Link Testing screen. (#239)
- **[Task]** **Users screen gap review** — A documentation exercise comparing the old and new Users management screens to plan which missing pieces (like bulk actions and extra columns) to bring over. (#80)
- **[Task]** **Brand guidelines as the main AI input** — Establishing a single, thorough brand-guidelines document to improve the quality of AI-generated output. (#264)

## Dashboard

- **[Task]** **Restore the missing dashboard sections** — A high-priority fix to bring back campaign stats, top offers, and watch lists so the dashboard shows full reporting again — and so the date range has data to update. (#240)
- **[Task]** **Custom date range on the dashboard** — Choosing "Custom" will open a start/end date picker so you can view dashboard data for any range you like, not just the preset options. (#58)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds an "Offers with Legs" view, a CLP offers performance view that flags offers converting under 30%, and a searchable log of changes like pausing offers or adjusting daily caps. (#256)
- **[Feature]** **Dark and light mode** — You'll be able to switch the whole admin between dark and light themes, with your choice remembered between visits. (#59)
- **[Task]** **Consistent dashboard colors** — Adopts a defined color palette across dashboard views for cleaner, more readable screens. (#263)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The Flow form's step-order control will get a plain-language label and inline help so you can understand what it does and what its values mean, without outside documentation. (#226)
- **[Task]** **Polish the Flow form's appearance** — Cleans up styling on the Flow form so text boxes, color pickers, checkboxes, and paired fields look consistent with the Placement and Modal forms. (#152)

## Pre-Pings

- **[Feature]** **Block leads missing required fields at push time** — When a pre-ping runs before pushing data, leads missing required fields will be stopped right away instead of being sent on, matching how required fields already work before an offer displays. (#218)
- **[Feature]** **Per-advertiser pre-ping check** — Confirms each active advertiser's pre-ping is mapped and working correctly before the new system takes over. (#41)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
