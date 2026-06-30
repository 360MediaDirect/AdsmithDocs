# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 17:34:54 UTC · 13 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker** — When you choose "Custom" on the Dashboard's date filter, you'll get start and end date selectors plus Apply/Cancel buttons, so you can view data for any specific span instead of only the preset options. (#58)
- **[Task]** **Bring back the full Dashboard with richer stats** — Restores the missing Dashboard sections so you'll see impressions, clicks, leads, and revenue (with an hourly breakdown), top performing offers, a placements watch list, recent notes, and alerts for offers converting under 30%. It also adds a searchable log of system and offer changes so admins can see who changed what and when. (#240)
- **[Feature]** **Filter reports without editing the web address** — You'll be able to pick a day or date range right from the Dashboard toolbar instead of manually changing the URL, while shareable links still update automatically. (#268)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is already editing a record, you'll see a clear "locked by" notice and be kept in read-only mode, and you'll be warned if a record changed since you opened it — so nobody's work gets silently lost. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper failure message instead of unexpectedly sending you back to the Dashboard. (#239)

## Behind the Scenes

- **[Task]** **Dedicated testing environment with May & June data** — A separate staging area loaded with recent data so the team can verify reports and features without touching live information. (#270)
- **[Feature]** **Auto-create tasks from Slack conversations** — A helper that turns action items from team chats into tracked work items automatically, reducing manual copying. (#272)

## Offers

- **[Task]** **Quick action links under each offer** — Each offer will show handy shortcuts (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening a performance page showing lead and revenue trends, date filtering, and a daily breakdown. (#252)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Fixes unstyled and misaligned parts of the Flow form so text boxes, color pickers, checkboxes, and paired fields look consistent with the rest of the app. (#152)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on Placements** — Builds on the recent drag-to-reorder work by considering a Manual Order default (so your chosen order is actually used) and adding a category filter to the available offers list, making it easier to find the right offers. (#275)

## Campaigns

- **[Feature]** **Add the Campaigns module** — A high-priority addition bringing campaign management into New Adsmith Frontend, letting you view, create, edit, and configure campaigns and their offer groups just like the legacy system. (#200)

## Users

- **[Task]** **Review of Users screen against the old system** — A documentation effort comparing the new Users area to the previous one to spot missing capabilities (like bulk actions and certain columns) and guide what to build next. (#80)

## Reports

- **[Task]** **Confirm report numbers match the legacy system** — An investigation into why some Dashboard report figures differed from the old system, so we can pinpoint and correct any discrepancies and give you numbers you can trust. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cca77278b68a1af565a4068f905447a1264979af969fc4cba7b7fdc40416e95f -->
