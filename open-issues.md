# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 15:45:51 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard** — Picking "Custom" from the date filter will finally open a start-and-end date picker, so you can view Dashboard data for any specific range instead of just the preset options. (#58)
- **[Feature]** **Change report dates without touching the address bar** — New date controls will live right in the Dashboard toolbar, letting you pull a specific day or range by clicking, not by editing the web address. Shareable links still update behind the scenes. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example, to a spreadsheet). (#286)
- **[Task]** **Visual polish on the Dashboard** — The header will show the logo instead of the "Adsmith" text, long offer names will no longer be cut off, and table rows will get cleaner alternating shading for easier reading. (#283)

## Surveys

- **[Feature]** **Design settings that actually show in the survey** — We're making sure every customization you set on the Design tab is reflected in the live survey, and reviewing all entity form options to remove any settings that currently have no effect. (#288)
- **[Bug]** **Survey styling options that don't work yet** — Many Design-tab settings (colors, continue button, question text, header, legal text) are saved but don't currently change what visitors see. This fix connects them so your choices actually appear in the survey. (#290)

## Placements

- **[Feature]** **Better control over placement offers** — New placements will default to your manual offer order (so the order you set is respected), and you'll be able to filter the available offers list by category to find offers faster. (#275)
- **[Feature]** **Preview before you save** — A preview button on the placement and offer edit pages will show how things will look based on your current, unsaved changes. (#289)

## Reports

- **[Task]** **Sortable Offer Audit tables** — You'll be able to click column headers in the Offer Performance Audit to sort results by any measure (leads, conversions, rates, and more), making outliers much easier to spot. (#281)
- **[Task]** **Confirming report numbers match the old system** — We're investigating why some Dashboard report figures differed from the legacy system, pinpointing the cause, and confirming the numbers can be trusted. (#271)

## General / Across the App

- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, the app will warn you if someone else is already editing or has changed it since you opened it, so no one's work gets silently lost. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when across offers, placements, and other records (including automated changes), making it easy to answer "who edited this?" (#276)

## Campaigns

- **[Feature]** **Campaigns module coming to the new platform** — The Campaigns feature from the legacy system isn't in New Adsmith Frontend yet. This high-priority work brings back creating, editing, and managing campaigns and their offer groups. (#200)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned. This cleanup brings its layout in line with the Placement and Modal forms for a consistent, polished experience. (#152)

## Users

- **[Task]** **Closing the gap on the Users screen** — A review comparing the new Users area to the legacy version identifies missing capabilities (like bulk actions and extra columns) so we can prioritize bringing them over. (#80)

## Link Testing

- **[Bug]** **Clearer results when testing a bad link** — Testing an invalid link currently dumps you back on the Dashboard with no explanation. This fix will show a proper error message instead. (#239)

## Behind the Scenes

- **[Task]** **A safe testing environment with real data** — We're setting up a separate staging area loaded with May and June data so reports and features can be validated without ever touching live information. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — A new assistant will read meeting and chat notes and file the resulting to-dos for the team automatically, reducing manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 489aad45c20d9ecda33940890a8015fca7f7c2f3338ebef7bafa545710c16e38 -->
