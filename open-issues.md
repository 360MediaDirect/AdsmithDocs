# Open Issues — Plain-Language Overview

_Last updated 2026-07-01 16:48:45 UTC · 11 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Reliable test environment with recent data** — We're setting up a separate, safe testing space loaded with May and June data so we can validate reports without ever touching or risking live information. (#270)
- **[Task]** **Checking report numbers against the old system** — We're investigating why some dashboard report figures don't match the legacy system, so we can pin down the cause and make sure the numbers you see are accurate and consistent. (#271)
- **[Feature]** **Turn conversations into tracked work automatically** — We're building a helper that reads team chat discussions and files the resulting to-dos directly, so requests and fixes are captured without manual copying. (#272)

## Dashboard

- **[Task]** **Custom date range picker on the Dashboard** — Choosing "Custom" on the date filter will open a proper calendar with start and end dates, so you can view Dashboard data for any range you like instead of only preset periods. (#58)
- **[Feature]** **Pick report dates without touching the web address** — You'll be able to select any day or date range straight from the Dashboard toolbar, so pulling a specific day's report is simple and no longer requires editing the address bar. Shareable links will still work. (#268)

## General / Across the App

- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link will now show a clear error message instead of unexpectedly sending you back to the Dashboard, so you know right away that the link didn't work. This fix is nearly complete. (#239)
- **[Feature]** **A searchable history of who changed what** — We're adding an Audit Log that records every change across the app — by both people and automated processes — with a timestamp and who made it. Administrators will be able to search this history and see a change trail on each record, making "who changed this and when" easy to answer. (#276)

## Campaigns

- **[Feature]** **Bring the Campaigns module into New Adsmith Frontend** — This core feature from the old admin isn't in the new platform yet. Once added, you'll be able to view, create, and edit campaigns and manage offer groups and their offers, just as you could before. This is a high-priority addition. (#200)

## Users

- **[Task]** **Comparing the old and new Users area** — A detailed review of the legacy Users screens against the new ones, identifying which features still need to be brought over (like bulk actions and extra columns) so the new Users area reaches full parity. (#80)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Some parts of the Flow form currently appear plain or misaligned, with fields stacking vertically instead of sitting side by side. This work polishes the styling so the form looks consistent and clean, matching the Placement and Modal forms. (#152)

## Placements

- **[Feature]** **Better control over offer ordering and filtering** — Building on recent improvements, new placements will be able to respect the exact order you arrange offers in, and you'll be able to filter the available offers list by category to find what you need faster. (#275)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 18c895dd2d51d67625ab25b86c398b76285d058485c5365f84641d856758854b -->
