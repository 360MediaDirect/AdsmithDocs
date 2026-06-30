# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 14:51:13 UTC · 14 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard** — Picking "Custom" in the date filter will open a proper start-and-end date picker, so you can view dashboard data for any range you choose instead of only the preset options. (#58)
- **[Task]** **Bring back the missing dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and choosing a date range will update them. Right now only the system overview loads. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — You'll get dedicated views for offers with sustained performance and for CLP offer performance (with low-converting offers under 30% flagged), plus a searchable record of every change — like pausing offers or adjusting caps — for easy auditing. (#256)
- **[Feature]** **Date controls built into the Dashboard** — You'll no longer need to hand-edit the web address to pull a specific day's report. Easy-to-find date controls will live right in the dashboard toolbar, while still keeping links shareable. (#268)

## Behind the Scenes

- **[Task]** **A dedicated testing environment with May & June data** — A separate practice environment loaded with recent data, so report checking and testing can happen safely without ever touching live information. (#270)
- **[Task]** **Confirming report numbers match the old system** — A review comparing dashboard report figures against the legacy system to find and explain any differences, so you can trust the numbers you see. (#271)
- **[Feature]** **Automatic issue logging from team chats** — Behind-the-scenes tooling that turns action items from team conversations into tracked work items automatically, helping the team capture and address needs faster. (#272)

## General / Across the App

- **[Feature]** **Safeguard against two people overwriting each other** — When you open a record to edit, others will see it's in use, and you'll be warned if someone changed it before you save — preventing accidental loss of each other's work across offers, flows, placements, advertisers, and more. (#267)
- **[Bug]** **Clear error when a link test fails** — Testing an invalid link will show a proper error message instead of quietly sending you back to the dashboard. (#239)

## Campaigns

- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — A high-priority addition that lets you view, create, edit, and manage campaigns and their offer groups — matching what's available in the legacy admin, where this is currently missing. (#200)

## Offers

- **[Task]** **Quick action links under each offer** — Each offer will show handy links like Edit, Quick Edit, Trash, View, Preview, Trends, and Details, with Trends opening an offer performance page covering leads, revenue, and daily breakdowns. (#252)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Polishing the Flow form so text boxes, color pickers, checkboxes, and paired fields display cleanly and consistently, matching the look of the Placement and Modal forms. (#152)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on Placements** — Building on the recent drag-to-reorder work: new placements would default to honoring your manual offer order, and you'll be able to filter the available offers list by category to find offers faster. (#275)

## Users

- **[Task]** **Review of the Users area against the old system** — A documentation review comparing the current Users screens with the legacy version to identify missing features — like bulk actions and extra columns — and prioritize what to add next. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8829154e1612d904d34214ce9b90f4489589545ee2e2d3b48335d954aee90f97 -->
