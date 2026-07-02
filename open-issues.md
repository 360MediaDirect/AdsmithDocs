# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 16:35:04 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a start-and-end date picker so you can view Dashboard data for any range you like, with the chosen dates shown right on the filter button. (#58)
- **[Feature]** **Pick report dates without editing the web address** — New date controls will live in the Dashboard toolbar so you can pull daily or custom-range reports directly, instead of hand-editing the address bar. The link still updates so you can share or bookmark it. (#268)
- **[Task]** **Data-matching check between the new and legacy reports** — We're comparing report numbers in New Adsmith Frontend against the old system to find and explain any differences, so you can trust that the figures line up. (#271)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example to a spreadsheet). (#286)
- **[Task]** **Dashboard polish: logo, full offer names, cleaner rows** — The header will show the brand logo, long offer names will no longer be cut off, and table rows will get tidy alternating shading for easier reading. (#283)

## Surveys
- **[Bug]** **Design settings that don't yet change the live survey** — Many look-and-feel options on the Placement Design tab (colors, continue button, question text, header, legal text) currently have no effect on what visitors see. This work makes those settings actually change the live survey widget. (#290)
- **[Feature]** **Make sure every Design-tab option really works** — We'll confirm that each customization on the Design tab is reflected in the survey view, and audit form options across all entity screens so there are no settings that quietly do nothing. (#288)
- **[Bug]** **Missing voucher code and info links on the live survey** — For certain Data Clients, the configured voucher-code question and the privacy/terms/details links aren't showing on the survey page even though they're saved. This fix makes them appear as they do in the legacy app, which matters for both leads and compliance. (#291)

## General / Across the App
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record to edit, others will see it as locked (with who has it and since when), and if a record changed while you had it open, you'll be prompted to reload instead of silently wiping out someone else's changes. Applies across all editable screens like Offers, Flows, Placements, Advertisers, and more. (#267)
- **[Feature]** **Searchable history of who changed what** — A new admin Audit Log will record every manual and automated change to your records — with the person or system, timestamp, and what changed — so you can look up "who changed this and when" and view a history right on each record. (#276)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you back on the Dashboard with no explanation. It will instead show a clear failure message so you know the link didn't work. (#239)

## Behind the Scenes
- **[Task]** **A safe practice environment with May & June data** — We're setting up a separate testing environment loaded with recent data so report checks and reviews can happen without touching live information. (#270)
- **[Feature]** **Turn conversations into tracked to-dos automatically** — An internal helper will read designated Slack discussions and file the resulting tasks as tracked issues (avoiding duplicates), saving manual copy-and-paste. (#272)

## Campaigns
- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — The Campaigns area from the old admin isn't here yet. This adds it back so you can view, create, and edit campaigns and manage offer groups, matching what you could do before. (#200)

## Placements
- **[Feature]** **Smarter defaults and filtering for the offer list** — Building on recent drag-to-reorder work, new placements can default to your manual offer order (so your arrangement is actually used), and you'll be able to filter the available offers list by category to find them faster. (#275)
- **[Feature]** **Preview placements and offers before saving** — A preview button on the placement and offer add/edit pages will show how things will look based on your current, unsaved entries. (#289)

## Users
- **[Task]** **Closing the gaps between the old and new Users screens** — A review comparing the legacy Users area to the new one is guiding work to bring back missing pieces (like bulk actions, password setup, and login/2FA details) so the new Users screen is as capable as the old one. (#80)

## Flows
- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form currently appear unstyled or awkwardly stacked. This tidies up textareas, color pickers, checkboxes, and side-by-side fields so the form matches the polish of the other screens. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: c297544c16901286038e0553d1205d4a4d2aff6095d33f2c18b5f7a831316cda -->
