# Open Issues — Plain-Language Overview

_Last updated 2026-07-01 23:28:55 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker** — Choosing "Custom" on the Dashboard date filter will finally open a proper start/end date picker, so you can view results for any range you like instead of only the preset options. (#58)
- **[Feature]** **Pick report dates without editing the web address** — New date controls will live right in the dashboard toolbar, so you can pull a specific day or range by clicking rather than hand-editing the address bar. Links will still update so you can share or bookmark a view. (#268)
- **[Task]** **Cleaner header, offer names, and table rows** — The header will show the logo instead of the "Adsmith" text, long offer names will no longer be cut off, and table rows will alternate white and light-gray for easier reading. (#283)
- **[Task]** **Update notes get their own table** — Update notes will be separated from optimizations and general notes so they're easy to spot and don't get lost among other note types. (#284)
- **[Task]** **Tidier offer names** — Offer names will drop the redundant text before the first colon, showing only the meaningful part. Names without a colon stay exactly as they are. (#285)
- **[Feature]** **Export the day-by-day breakdown** — A high-priority addition that lets you download the breakdown-by-day view (for example to a spreadsheet) so you can work with the data outside the app. (#286)

## Surveys

- **[Task]** **Survey images show in full** — Images in surveys will fit within their space instead of being cropped, so the whole image is always visible. (#287)
- **[Feature]** **Design settings that actually change the survey** — Every option on the Design tab will be checked to make sure it truly changes what visitors see, and this review will extend across all entity forms to catch any settings that currently do nothing. (#288)
- **[Bug]** **Turn on the remaining survey styling controls** — Many Design-tab settings (colors, continue button, question text, header, legal text) are saved today but don't affect the live survey. This work connects them so your customizations actually appear to visitors. (#290)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else is already editing a record, you'll see a clear "locked by" notice, and if a record changes while you have it open, you'll be prompted to reload instead of silently wiping out their changes. Works across offers, flows, placements, advertisers, and more. (#267)
- **[Feature]** **A searchable history of who changed what** — Every create, edit, delete, pause, and automated change will be recorded with a timestamp and the responsible person or system, viewable in a new searchable Audit Log and from each record's detail page. This makes it easy to answer "who changed this and when." (#276)
- **[Task]** **Filling the gaps in the Users area** — A review comparing the old and new Users screens to bring back missing capabilities like bulk selecting users, changing roles in bulk, last-login and two-factor details, and setting a password when adding a user. (#80)

## Behind the Scenes

- **[Task]** **A safe testing environment with real data** — A separate staging environment loaded with May and June data so report checking and testing can happen without ever touching live information. (#270)
- **[Task]** **Making sure the numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy system, to pinpoint the cause and confirm the new platform's numbers are correct. (#271)
- **[Feature]** **Turning conversations into tracked tasks automatically** — A helper that reads designated chat channels and files the action items as tracked work items, cutting out manual copy-and-paste. (#272)

## Placements

- **[Feature]** **Better control over the offer list** — Follow-up work so new placements can default to your manual offer order (rather than random), and so you can filter the available offers by category when building a placement. (#275)
- **[Feature]** **Preview before you save** — A preview button on the placement and offer add/edit pages will show how your placement or offer will look based on your current, unsaved changes. (#289)

## Reports

- **[Task]** **Sortable Offer Audit tables** — You'll be able to click any column heading in the Offer Performance Audit results (Leads, Conversions, conversion rates, and more) to re-sort, making outliers much easier to spot. (#281)

## Flows

- **[Task]** **Consistent, polished Flow form** — Remaining styling fixes so the Flow form matches the look of other forms, with properly styled text boxes, color pickers, and side-by-side field pairs instead of unstyled or stacked elements. (#152)

## Campaigns

- **[Feature]** **Bringing back the Campaigns module** — A high-priority effort to add campaign management to the new platform, letting you view, create, edit, and configure campaigns and their offer groups just like the previous system. (#200)

## Link Testing

- **[Bug]** **Clear error for invalid links** — Testing an invalid link will show a proper failure message instead of quietly sending you back to the dashboard. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 7cf2416479c6a006663477450a87c48f16726c5f92d204cab5941b3f0ca4624c -->
