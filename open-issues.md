# Open Issues — Plain-Language Overview

_Last updated 2026-06-26 11:57:41 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a start- and end-date picker so you can view results for any specific range, with the selected dates shown right on the filter button. (#58)
- **[Task]** **Restore missing Dashboard sections** — High priority. The campaign stats, top offers, and watch list sections will come back to the Dashboard, and they'll update when you change the date range, instead of only the system overview loading. (#240)
- **[Feature]** **New "Other Dashboard" views and a change history** — Adds dedicated views for monitoring long-running offers and CLP offer performance (flagging those converting under 30%), plus a searchable log of who paused offers, changed caps, or updated settings and when. (#256)
- **[Feature]** **Light mode option for the Admin** — A theme switcher will let you choose between the current dark mode and a new light mode across the whole Admin, with your choice remembered next time you log in. (#59)
- **[Task]** **Consistent Dashboard colors** — A defined color palette will be applied across the Dashboard so charts and sections are easier to read at a glance. (#263)

## General / Across the App

- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, you'll see a clear "locked by" notice and a warning if someone changed it since you opened it, so one person's save can no longer silently wipe out another's. This will apply to every editable screen (offers, flows, placements, advertisers, and more). (#267)
- **[Bug]** **Invalid link tests now show an error** — Testing a bad link will return a clear failure message in Link Testing instead of quietly sending you back to the Dashboard. (#239)
- **[Task]** **Users screen feature review** — A review comparing the older Users area to the new one, identifying missing pieces (like bulk actions and extra columns) to guide upcoming improvements. (#80)
- **[Task]** **Stronger brand guidelines for AI output** — A complete brand-guidelines document will be used as the main reference for AI-generated content, improving the quality and consistency of results. (#264)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The Step order field on the Flow form will get a plain-language label and helpful explanation so you can tell exactly what it controls and what its values do. (#226)
- **[Task]** **Polish the Flow form's appearance** — Cleans up styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields look consistent with the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bring back the Campaigns area** — Critical, high priority. The Campaigns module from the older system will be added so you can create, edit, and manage campaigns and offer groups directly in New Adsmith Frontend. (#200)

## Placements

- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and a filter to narrow the offer list by category. (#235)

## Pre-Pings

- **[Feature]** **Enforce required fields on pre-pings** — When a pre-ping runs before pushing data, leads missing required information will be stopped right away rather than being sent on and judged only by the advertiser's response. (#218)

## Behind the Scenes

- **[Feature]** **Faster "today" stats** — Behind-the-scenes work so the Dashboard's "today" view reflects up-to-the-hour impressions, clicks, leads, and revenue in the correct time zone. (#34)
- **[Feature]** **Reliable historical reporting totals** — Maintenance to roll up daily figures accurately so historical reports stay correct and quick to load. (#35)
- **[Task]** **Speed improvements for surveys** — Behind-the-scenes caching to make survey and offer lookups respond faster. (#42)
- **[Task]** **Review an old stats job** — Behind-the-scenes check to confirm whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Safety testing for pre-pings** — Running the new pre-ping process alongside the old one to confirm the results match before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each active advertiser's pre-ping behaves correctly ahead of the switchover. (#41)
- **[Task]** **Prepare new scheduled tasks for launch** — Running the new automated background tasks in parallel with the existing ones and watching for any differences. (#43)
- **[Task]** **Phased switchover of background tasks (group 3)** — Retiring the first set of older background jobs once their replacements prove stable. (#44)
- **[Task]** **Phased switchover of background tasks (group 2)** — Retiring the next set of older background jobs after a monitoring period. (#45)
- **[Task]** **Phased switchover of background tasks (group 1)** — Critical. Carefully retiring the most important older background jobs last, with the ability to roll back immediately if needed. (#46)
- **[Task]** **Rollback plans** — Documenting and testing step-by-step recovery procedures for each system in case something needs to be reversed. (#48)
- **[Task]** **Troubleshooting guides** — Creating reference guides so the team can quickly resolve common issues like stalled lead processing or stats problems. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
