# Open Issues — Plain-Language Overview

_Last updated 2026-07-01 18:38:15 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker on the Dashboard** — When you choose "Custom" in the date filter, you'll get start and end date pickers with Apply and Cancel buttons, so you can view Dashboard data for any range you like. (#58)
- **[Feature]** **Pick report dates without editing the web address** — New date controls will live right in the Dashboard toolbar, so you can pull daily or custom-range reports directly instead of hand-editing the address bar. Shareable links still update automatically. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example, as a spreadsheet) for your own analysis. This is a high-priority addition. (#286)
- **[Task]** **Separate table for update notes** — Update notes will get their own dedicated table instead of being mixed in with optimizations and general notes, so important updates are easier to spot. (#284)
- **[Task]** **Cleaner offer names on the Dashboard** — Offer names will show only the meaningful part after the first colon and will no longer be cut off, making them easier to read at a glance. (#285, #283)
- **[Task]** **Dashboard visual polish** — The header will show the logo instead of the "Adsmith" text, and table rows will get cleaner alternating background shading across the Dashboard and Admin area. (#283)

## General / Across the App

- **[Feature]** **Campaigns module in the new platform** — The Campaigns feature from the old admin system is being rebuilt here, so you'll be able to view, create, edit, and configure campaigns and their offer groups. This is a critical, high-priority piece of core functionality. (#200)
- **[Feature]** **Editing lock so two people don't overwrite each other** — When you open a record to edit, others will see it's locked and by whom, preventing one person's changes from silently wiping out another's. Administrators can take over an in-use record when needed. (#267)
- **[Feature]** **Searchable history of who changed what** — Every change to records across the app (and automated changes too) will be recorded with a timestamp and the person or system responsible, viewable in a new searchable Audit Log and on each record's history. (#276)
- **[Task]** **Bring User Management features up to par** — A review of the old versus new user management screens is underway to close gaps, such as bulk actions, additional columns, and sign-in details, so managing users feels complete. (#80)

## Surveys

- **[Feature]** **Design choices show up in the live survey** — Every customization option on the Design tab will be fully connected to what appears in the survey view, and form options across all entities will be checked to make sure none are ignored. (#288)
- **[Task]** **Survey images display in full** — Survey images will fit within their space instead of being cropped, so the whole image is always visible. (#287)

## Placements

- **[Feature]** **Preview button for placements and offers** — A preview button on the add and edit pages will show how a placement or offer will actually look, based on your current unsaved changes. (#289)
- **[Feature]** **Smarter offer ordering and filtering on Placements** — You'll be able to filter the available offers list by category, and we're confirming whether new placements should default to your manually set offer order so your arrangement is respected at serve time. (#275)

## Reports

- **[Task]** **Sortable Offer Audit tables** — You'll be able to click any column header in the Offer Performance Audit tables (Sources, Gender, Age, States, Email Domains) to sort by it, making outliers easy to find. It still defaults to Opt-Ins, highest first. (#281)
- **[Task]** **Confirming report numbers match the old system** — An investigation is comparing report totals between the old and new platforms over a fixed date range to find and explain any differences, so you can trust the numbers. (#271)

## Behind the Scenes

- **[Task]** **A safe testing environment with real sample data** — A separate staging setup loaded with May and June data is being created so reports and features can be verified without ever touching live information. (#270)
- **[Feature]** **Automatic issue capture from team chats** — A helper that reads designated conversations and files the action items as tracked tasks automatically, reducing manual copying. (#272)

## Flows

- **[Task]** **Fix unstyled areas of the Flow form** — Remaining styling issues on the Flow form (text boxes, color pickers, checkboxes, and side-by-side fields) are being cleaned up so it matches the polished look of the Placement and Modal forms. (#152)

## Link Testing

- **[Bug]** **Clear error when testing an invalid link** — Instead of quietly sending you to the Dashboard, entering an invalid link will show a proper error result so you know the test failed. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: a33ed35aa2195122cb77d15a76dfdaa79cc9c77eee698e6378dd048b0e094371 -->
