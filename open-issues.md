# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 09:04:59 UTC · 14 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker for the dashboard filter** — Choosing "Custom" on the date filter will finally open a calendar where you can set your own start and end dates and apply them, instead of being limited to presets like Today or This Month. (#58)
- **[Task]** **Bring back the missing dashboard sections** — The dashboard will once again show campaign stats, top offers, and watch lists, not just the system overview, and the date range will update these sections with real data. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — You'll get dedicated views for offers with sustained performance ("Offers with Legs") and for CLP offer performance, with low-converting offers flagged, plus a searchable record of changes like pausing offers or adjusting caps. (#256)
- **[Feature]** **Change report dates without editing the address bar** — Date and day selection will move into the dashboard toolbar, so you can pull a specific day's report through simple controls while links stay shareable. (#268)
- **[Task]** **Confirm dashboard numbers match the legacy system** — A review is underway to compare report figures between the old and new platforms and resolve any differences, so you can trust that the dashboard totals are accurate. (#271)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit, the app will let others know it's being worked on and warn you if someone changed it before you save, so changes are no longer accidentally lost. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will show a proper failure message in the Link Testing screen instead of quietly sending you back to the dashboard. (#239)

## Behind the Scenes

- **[Task]** **Dedicated testing environment with May and June data** — A separate practice environment will be set up with real-looking data so reports can be checked and verified without ever touching live information. (#270)
- **[Feature]** **Automatically turn Slack discussions into tracked tasks** — A helper will read designated Slack channels and file action items as tracked issues automatically, reducing manual copy-and-paste and keeping requests from slipping through the cracks. (#272)

## Offers

- **[Task]** **Quick action links under each offer** — Each offer will show handy shortcuts like Edit, Quick Edit, Trash, View, Preview, Trends, and Details, with Trends opening an activity page covering lead and revenue performance over time. (#252)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on placements** — New placements will respect the order you arrange offers in by default, and you'll be able to filter the available offers list by category to find what you need faster. (#275)

## Flows

- **[Task]** **Fix the unstyled Flow form layout** — The Flow form will get proper styling so text boxes, color pickers, checkboxes, and paired fields display cleanly and side-by-side, matching the polished look of the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — A high-priority addition will let you view, create, edit, and configure campaigns and offer groups in New Adsmith Frontend, matching the capabilities of the old admin system. (#200)

## Users

- **[Task]** **Review of missing Users features from the old system** — A side-by-side comparison is being documented to identify gaps in the Users area, such as bulk actions and login details, to guide what gets added next. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8829154e1612d904d34214ce9b90f4489589545ee2e2d3b48335d954aee90f97 -->
