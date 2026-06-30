# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 16:43:11 UTC · 13 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Task]** **Custom date range on the Dashboard date filter** — Choosing "Custom" will open a proper start- and end-date picker so you can view dashboard data for any range you want, with your selected dates shown right on the filter button. (#58)
- **[Task]** **Bring back the full set of dashboard sections** — High priority. Beyond the current system overview, you'll see campaign performance stats, top offers, a placements watchlist, recent notes, and alerts for offers converting under 30%, all responding to your chosen date range — plus a searchable history of changes to offers and settings. (#240)
- **[Feature]** **Pick report dates without editing the web address** — You'll get easy date controls right in the dashboard toolbar, so you no longer have to hand-edit the address bar to pull a specific day or range. Shareable links still update automatically. (#268)

## Behind the Scenes
- **[Task]** **A safe testing environment with recent data** — A dedicated staging area loaded with May and June data so the team can validate reports without ever touching live information. (#270)
- **[Task]** **Confirming report numbers match the old system** — An investigation into why some dashboard figures differed from the legacy app, so you can trust that the new reports are accurate. (#271)
- **[Feature]** **Auto-create tasks from team conversations** — A behind-the-scenes assistant that turns action items from team chats into tracked work items, helping the team capture and follow up on requests more reliably. (#272)

## General / Across the App
- **[Feature]** **Protection against two people overwriting the same record** — When someone opens a record for editing, others will see it's locked and won't accidentally erase each other's changes. If a record was changed while you had it open, you'll be prompted to reload before saving. (#267)
- **[Bug]** **Clear error when testing an invalid link** — A bug fix so that entering a bad link shows a proper error message instead of unexpectedly sending you back to the dashboard. (#239)

## Campaigns
- **[Feature]** **Add the Campaigns area to the new app** — Critical, high priority. The Campaigns capability from the older system is being rebuilt so you can create, edit, and manage campaigns, offer groups, and their settings directly in New Adsmith Frontend. (#200)

## Offers
- **[Task]** **Quick action links under each offer** — Familiar shortcuts (Edit, Quick Edit, Trash, View, Preview, Trends, Details) will appear beneath each offer title, with Trends opening a performance page showing leads, revenue, and a daily breakdown. (#252)

## Flows
- **[Task]** **Tidy up the Flow form's appearance** — Ongoing styling fixes so text boxes, color pickers, checkboxes, and paired fields look consistent and properly laid out instead of appearing plain or stacked incorrectly. (#152)

## Placements
- **[Feature]** **Better defaults and filtering for offer ordering** — Continuing earlier work, this looks at making new placements respect your manual offer order by default and adds a category filter to the available offers list so you can find offers faster. (#275)

## Users
- **[Task]** **Closing gaps between the old and new Users area** — A review of features from the previous Users screens (such as bulk actions, extra columns, and login details) to guide what's added next for managing users. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 1c4684153aa2793a3569392a2111eafd6091b6e9722a9360e6e862edd51a7607 -->
