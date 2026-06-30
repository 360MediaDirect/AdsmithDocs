# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 21:31:11 UTC · 11 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker for the dashboard** — Choosing "Custom" on the date filter will finally open a proper calendar with start and end dates, so you can view dashboard data for any period you like instead of being limited to preset options. (#58)
- **[Feature]** **Pick report dates right from the dashboard** — You'll be able to select a specific day or range using on-screen controls in the dashboard, with no need to edit the web address by hand. Links will still update so you can share or bookmark a view. (#268)
- **[Task]** **Make sure report numbers match the old system** — We're checking that dashboard report figures line up with the legacy system so you can trust the totals you see. This investigation will pin down and explain any differences. (#271)

## General / Across the App

- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper failure message instead of quietly sending you back to the dashboard, so you always know the result of a link test. (#239)
- **[Feature]** **Searchable history of changes across the platform** — A new Audit Log will record who changed what and when — across offers, placements, advertisers, and more — including automated changes. Administrators will be able to search this history and view a change trail on each record. (#276)

## Behind the Scenes

- **[Task]** **Safe testing environment with recent data** — We're setting up a separate practice environment loaded with May and June information so report checking and testing can happen without ever touching live data. (#270)
- **[Feature]** **Automatic issue creation from team chats** — A helper that turns action items mentioned in team conversations into tracked work items automatically, reducing manual copy-and-paste and helping requests get logged reliably. (#272)

## Campaigns

- **[Feature]** **Bring the Campaigns area into New Adsmith Frontend** — The Campaigns tools from the older admin aren't available yet. This work adds them back so you can create, edit, and manage campaigns and their offer groups — including titles, questions, CTAs, and offer handling — all in one place. (#200)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned, with fields stacking awkwardly. This polish pass brings text boxes, color pickers, checkboxes, and paired fields in line with the cleaner look used elsewhere. (#152)

## Placements

- **[Feature]** **Better control over offer order and filtering on Placements** — Building on the recent drag-to-reorder improvements, this lets new placements respect your manual offer order by default and adds a way to filter the available offers list by category, making it faster to find the right offers. (#275)

## Users

- **[Task]** **Closing the gaps in the Users area** — A review comparing the old and new Users screens to spot what's missing — like bulk actions, sign-in details, and password setup on new users — so the new Users area matches what people relied on before. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 18c895dd2d51d67625ab25b86c398b76285d058485c5365f84641d856758854b -->
