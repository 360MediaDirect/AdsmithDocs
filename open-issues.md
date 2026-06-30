# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 12:38:55 UTC · 14 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Task]** **Custom date range picker on the Dashboard** — When you choose "Custom" in the date filter, you'll get start and end date pickers with Apply and Cancel buttons, so you can view dashboard data for any specific range you like. (#58)
- **[Task]** **Bring back missing Dashboard sections** — Right now only the system overview loads. This restores the campaign stats, top offers, and watch list sections from the previous system, and makes them respond to the date range you pick. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds dedicated views for monitoring long-running ("Offers with Legs") and CLP offers, with under-30% performers clearly flagged, plus a searchable record of every offer change (pauses, cap changes, status updates) and who made them. (#256)
- **[Feature]** **Choose report dates without editing the web address** — Today you have to hand-edit the address bar to pull a specific day's report. This adds proper date controls right in the dashboard toolbar, while still keeping links shareable. (#268)

## Behind the Scenes
- **[Task]** **A safe testing environment with May and June data** — Sets up a separate space loaded with real-world data so the team can validate reports and test changes without ever touching live information. (#270)
- **[Task]** **Confirming report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy system, so we can pin down the cause and make sure the numbers you see are accurate. (#271)
- **[Feature]** **A Slack helper that turns discussions into tracked tasks** — A behind-the-scenes assistant that reads team conversations and automatically logs follow-up items, helping make sure requests don't slip through the cracks. (#272)

## General / Across the App
- **[Feature]** **Protection against two people overwriting the same record** — When someone is already editing a record, you'll see a clear "locked by" notice, and you'll be warned if a record changed while you had it open — so edits can no longer be accidentally wiped out by a co-worker. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Currently, testing a bad link quietly sends you to the dashboard. This fixes it so you'll get a proper error message telling you the link didn't work. (#239)

## Campaigns
- **[Feature]** **Add the Campaigns module to the new platform** — A high-priority addition that brings back full campaign management — viewing, creating, and editing campaigns, configuring settings, and managing offer groups and their offers — matching what's available in the legacy admin. (#200)

## Flows
- **[Task]** **Tidy up the Flow form's appearance** — Cleans up styling issues on the Flow form so textareas, color pickers, checkboxes, and paired fields display neatly and consistently, instead of looking unstyled or stacked awkwardly. (#152)

## Offers
- **[Task]** **Quick action links under each offer** — Adds handy shortcuts (Edit, Quick Edit, Trash, View, Preview, Trends, Details) beneath every offer title, with Trends opening an activity page showing lead and revenue performance over time. (#252)

## Placements
- **[Feature]** **Smarter offer ordering and filtering on Placements** — Follows up on earlier reordering work by considering a "Manual Order" default (so your chosen order actually takes effect) and adding a category filter to the available offers list, making it easier to find the offers you want. (#275)

## Users
- **[Task]** **Review of the Users area against the old system** — A documentation effort comparing the new Users screens to the legacy version, identifying missing pieces (like bulk actions and last-login info) so they can be prioritized for future work. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8829154e1612d904d34214ce9b90f4489589545ee2e2d3b48335d954aee90f97 -->
