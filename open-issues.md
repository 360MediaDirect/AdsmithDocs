# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 09:02:57 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard** — When you pick "Custom" from the date filter, you'll get a proper start-and-end date picker so you can view results for any exact range you choose, with the selected dates shown right on the filter button. (#58)
- **[Feature]** **Change report dates without touching the address bar** — You'll be able to pull daily or any-range reports using simple controls in the dashboard toolbar, instead of manually editing the web address. Links will still stay shareable. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example, to a spreadsheet) for your own analysis. (#286) *(high priority)*
- **[Task]** **Cleaner dashboard look** — The header will show the logo instead of the "Adsmith" text, long offer names will no longer be cut off, and table rows will use tidy alternating shading for easier reading. (#283)
- **[Task]** **Update notes get their own table** — Update notes will be separated from optimizations and general notes so they stand out clearly instead of getting lost in the mix. (#284)
- **[Task]** **Tidier offer names** — Offer names that contain a colon will show only the meaningful part after it, trimming redundant prefix text. Names without a colon stay as they are. (#285)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is already editing a record (an offer, flow, placement, advertiser, and so on), you'll see a clear "locked by" notice, and the app will warn you if a record changed while you had it open — so no one's work gets silently wiped out. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when across the whole platform, including automated updates, so you can easily trace the history of any record. (#276)
- **[Bug]** **Clearer results when testing an invalid link** — Testing a bad link will show a proper error message instead of quietly sending you back to the dashboard. (#239)
- **[Task]** **Bringing the Users area up to par** — A review of the older Users management screens is underway to identify missing capabilities (like bulk actions and additional user details) and bring the new Users area in line. (#80)

## Surveys

- **[Bug]** **Survey design settings that actually take effect** — Many survey styling and layout options (colors, buttons, header text, legal text, and more) are currently saved but don't change what visitors see. This work makes those settings truly control the live survey. (#290)
- **[Feature]** **Design choices reflected in the survey** — Every option on the Design tab will be connected end-to-end so your customizations show up in the actual survey, and all entity forms will be checked to confirm no setting is left disconnected. (#288)
- **[Task]** **Survey images shown in full** — Survey images will display completely instead of being cropped, so the whole image is always visible. (#287)

## Behind the Scenes

- **[Task]** **A safe testing environment with recent data** — A dedicated staging area loaded with May and June data will let the team validate reports and features without ever touching live information. (#270)
- **[Task]** **Confirming report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy system, to pinpoint and resolve any discrepancies so you can trust the numbers. (#271)
- **[Feature]** **Turning conversations into tracked work automatically** — A behind-the-scenes assistant that captures action items from team chats and logs them as tracked tasks, reducing manual note-shuffling. (#272)

## Placements

- **[Feature]** **Better offer ordering and filtering on Placements** — Continuing recent improvements, this sets a sensible default order for offers and adds the ability to filter the available offers list by category, making it faster to build the right offer stack. (#275)
- **[Feature]** **Preview placements and offers before saving** — A preview button on the placement and offer add/edit pages will let you see how things will look based on your current, unsaved settings. (#289)

## Campaigns

- **[Feature]** **Campaigns management in New Adsmith Frontend** — The Campaigns area from the older system is being rebuilt so you can create, edit, and manage campaigns and their offer groups directly in the new platform. This is a high-priority, core capability. (#200)

## Reports

- **[Task]** **Sortable Offer Audit results** — The Offer Performance Audit tables (Sources, Gender, Age, States, Email Domains) will let you click any column to sort, making it much easier to spot standout results instead of being stuck with a single fixed order. (#281)

## Flows

- **[Task]** **Polishing the Flow form's appearance** — Ongoing cleanup to fix unstyled elements and misaligned fields on the Flow form so it looks consistent with the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 7cf2416479c6a006663477450a87c48f16726c5f92d204cab5941b3f0ca4624c -->
