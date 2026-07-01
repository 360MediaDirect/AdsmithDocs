# Open Issues — Plain-Language Overview

_Last updated 2026-07-01 20:34:31 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker on the dashboard** — Choosing "Custom" in the date filter will open a proper calendar so you can pick your own start and end dates, and the dashboard will update to show just that range. (#58)
- **[Feature]** **Pick report dates without touching the address bar** — Date and day selection will move into the dashboard's toolbar, so you can pull a specific day or range from the screen itself instead of editing the web address. Shareable links will still reflect what you selected. (#268)
- **[Task]** **Cleaner dashboard header and offer names** — The header will show the logo in place of the "Adsmith" text, long offer names will no longer be cut off, and table rows will get clearer alternating shading for easier reading. (#283)
- **[Task]** **Update notes get their own table** — Update notes will be separated from optimizations and general notes so they stand out and are easy to find. (#284)
- **[Task]** **Tidier offer names on the dashboard** — Offer names will drop the repetitive text before the first colon, showing only the meaningful part. Names without a colon stay exactly as they are. (#285)
- **[Feature]** **Export the day-by-day breakdown** — A high-priority addition of an export button lets you download the breakdown-by-day data for use in a spreadsheet. (#286)

## Behind the Scenes

- **[Task]** **A safe testing environment with May and June data** — A dedicated staging setup loaded with real May and June figures so testing and report checks can happen without any risk to live data. (#270)
- **[Task]** **Confirming report numbers match the old system** — An investigation into why some dashboard report totals differed from the legacy system, so we can pinpoint the cause and ensure the numbers you see are trustworthy. (#271)
- **[Feature]** **Automatic issue capture from team chat** — A behind-the-scenes helper that turns action items raised in team conversations into tracked work items, so requests are less likely to slip through the cracks. (#272)

## Surveys

- **[Task]** **Survey images display in full** — Survey images will fit within their space instead of being cropped, so the whole image is always visible. (#287)
- **[Feature]** **Design choices always show up in the survey** — Every styling option in the design tab will be reflected in the live survey, and we'll review the form options across all screens to make sure nothing you set is quietly ignored. (#288)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on placements** — The list of available offers will gain a category filter, and we're reviewing whether new placements should default to your manual offer order so the order you arrange is actually used. (#275)
- **[Feature]** **Preview placements and offers before saving** — A preview button on the add/edit pages will show how a placement or offer will look based on your current, unsaved changes. (#289)

## General / Across the App

- **[Feature]** **No more accidentally overwriting each other's edits** — When two people open the same record, you'll see who's already editing it and be protected from silently overwriting their changes, with a clear prompt to reload if something changed while you had it open. Applies across all the main entity screens. (#267)
- **[Feature]** **A searchable history of who changed what** — Every change to offers, placements, advertisers and other records (whether made by a person or an automated process) will be recorded with a timestamp, and a searchable Audit Log page will let you trace exactly who changed something and when. (#276)

## Campaigns

- **[Feature]** **Campaigns module coming to New Adsmith Frontend** — A high-priority build to bring the Campaigns feature over from the old system, so you can create, edit, and manage campaigns and their offer groups directly in the new platform. (#200)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Cleanup of the Flow form's appearance so text boxes, color pickers, and paired fields display neatly and consistently, matching the other forms in the app. (#152)

## Users

- **[Task]** **Reviewing the Users screen against the old system** — A detailed comparison of the new Users area with the legacy version to identify missing capabilities (such as bulk role changes and last-login details) and prioritize what to add next. (#80)

## Reports

- **[Task]** **Sortable Offer Audit tables** — The breakdown tables in the Offer Performance Audit will get clickable column headers, so you can sort by leads, conversions, or conversion rates to spot outliers instead of being stuck with a single fixed order. (#281)

## Link Testing

- **[Bug]** **Clear error when a link is invalid** — Testing an invalid link will show a proper error message instead of unexpectedly sending you to the dashboard. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: a33ed35aa2195122cb77d15a76dfdaa79cc9c77eee698e6378dd048b0e094371 -->
