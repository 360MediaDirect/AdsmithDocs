# Open Issues — Plain-Language Overview

_Last updated 2026-06-28 22:22:24 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole admin experience between the current dark look and a new light theme, with your choice remembered the next time you log in. (#59)
- **[Task]** **Restore the missing dashboard sections** — The Dashboard will once again show campaign stats, top offers, and watch lists (not just the system overview), and the date range selector will update them. This is a high-priority fix. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — You'll get dedicated views for offers with sustained performance ("Offers with Legs") and CLP offer performance, with low-converting CLP offers (under 30%) flagged for attention, plus a searchable record of changes like pausing offers or adjusting caps. (#256)
- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a start/end date picker so you can view dashboard data for any period you like, instead of only preset ranges. (#58)
- **[Task]** **Consistent dashboard colors** — A defined color palette will be applied across the Dashboard for cleaner, easier-to-read screens. (#263)

## General / Across the App

- **[Feature]** **Protection against two people overwriting the same record** — When you open an entity (like an offer, flow, placement, or advertiser) to edit, others will see it's being worked on, and you'll be warned before saving over someone else's recent changes. This prevents work from being silently lost. (#267)
- **[Bug]** **Invalid link tests now show an error** — When you test a link that isn't valid, you'll get a clear failure message instead of being unexpectedly dropped onto the dashboard. (#239)
- **[Task]** **Users area review** — A behind-the-scenes comparison of the older Users screens against the new ones, to make sure important capabilities aren't missing as the new Users area is built out. (#80)
- **[Task]** **Brand guidelines for AI output** — A single, thorough brand-guidelines document will be created and used to steer AI-generated content, improving the quality and consistency of results. (#264)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The Step order field on the Flow form will get a plain-language label and helpful inline text explaining exactly what it controls, so you don't have to guess what it does. (#226)
- **[Task]** **Tidy up the Flow form's appearance** — Remaining styling issues on the Flow form (such as plain-looking text boxes, color pickers, and fields that stack instead of sitting side by side) will be cleaned up to match the polished look of the Placement and Modal forms. (#152)

## Offers & Campaigns

- **[Feature]** **Bring back the Campaigns module** — You'll be able to view, create, edit, and configure campaigns and their offer groups in New Adsmith Frontend, matching what's available today in the older admin. This is a high-priority, core feature. (#200)
- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping runs before pushing data, leads missing required fields will be stopped right away rather than relying on the advertiser's system to catch them, helping prevent incomplete leads from slipping through. (#218)

## Placements

- **[Feature]** **Better control over offer ordering on Placements** — Selected offers will default to manual order, with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by category, making it much easier to arrange exactly the offers you want. (#235)

## Behind the Scenes

- **[Task]** **Performance boost for Surveys** — Adding a caching layer so survey-related screens and offer checks respond faster. High priority. (#42)
- **[Feature]** **Up-to-the-moment "today" numbers** — Work to make the Dashboard's "today" figures (impressions, clicks, leads, revenue) reflect the current day's activity in real time. (#34)
- **[Feature]** **Faster historical reporting** — Behind-the-scenes work to roll up daily totals so historical stats load reliably. (#35)
- **[Task]** **Review of an older scheduled job** — Checking whether a legacy stats job is still needed or can be retired. (#33)
- **[Task]** **Safety testing for the new pre-ping system** — Running the new system alongside the old one to confirm results match before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each active advertiser's pre-ping works correctly before the switch. (#41)
- **[Task]** **Run new and old scheduled jobs side by side** — Bringing the new background jobs online alongside the existing ones and monitoring for any differences. (#43)
- **[Task]** **Gradual switch-over of background jobs (lower risk)** — Retiring the first set of older background jobs once the replacements prove stable. (#44)
- **[Task]** **Gradual switch-over of background jobs (mid-tier)** — Retiring the next set of older stats jobs after the first batch is stable. (#45)
- **[Task]** **Gradual switch-over of background jobs (most critical)** — Carefully retiring the most important jobs last, with close monitoring and the ability to revert immediately. (#46)
- **[Task]** **Documented recovery steps** — Writing and testing clear procedures to quickly roll back each system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides** — Creating step-by-step guides for handling common operational issues. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
