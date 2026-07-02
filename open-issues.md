# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 17:32:55 UTC · 17 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will finally open a proper start-and-end date picker, so you can view Dashboard data for any range you like instead of only the preset options. (#58)
- **[Feature]** **Pick report dates without editing the web address** — New date controls will live right in the Dashboard toolbar, so you can pull a specific day or range with a click rather than hand-typing anything into the address bar (links will still stay shareable). (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example to a spreadsheet) for your own reporting. (#286)

## Surveys

- **[Feature]** **Make every Design tab option actually take effect** — Design customizations you set will be reliably carried through to what visitors see, and we'll review all form options across every screen to make sure none are just for show. (#288)
- **[Bug]** **Survey styling settings that currently do nothing will work** — Right now most of the ~30 Design tab settings (colors, buttons, headers, legal text, and more) are saved but ignored on the live survey. This fix connects them so your choices genuinely change how the survey looks and behaves. (#290)
- **[Bug]** **Voucher codes and info links will show on the live survey** — Custom questions (like a voucher code) and privacy/terms/details links configured for a Data Client aren't appearing on the new survey page even though they show in the legacy app. This restores them, which matters for both leads and compliance. (#291)

## Placements

- **[Feature]** **Better control over the offer list on placements** — New placements will default to using your manual offer order (so the order you set is actually respected), and you'll be able to filter the available offers by category to find them faster. (#275)
- **[Feature]** **Preview button on placement and offer pages** — You'll be able to preview how a placement or offer will appear using your current, unsaved edits before committing them. (#289)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else is already editing a record, you'll see a clear "locked by" notice, and if a record changes while you have it open you'll be prompted to reload rather than silently wiping out their work. This protection will apply across all editable screens. (#267)
- **[Feature]** **A searchable history of who changed what** — Every change to offers, placements, advertisers, and other records (whether made by a person or an automated process) will be recorded with a timestamp, and administrators will get a searchable Audit Log plus per-record history. Great for answering "who changed this and when?" (#276)

## Behind the Scenes

- **[Task]** **A safe testing environment with recent data** — We're setting up a separate staging environment loaded with May and June data so testing and report checks can happen without ever touching live information. (#270)
- **[Feature]** **Turn conversations into tracked to-dos automatically** — A new helper will read designated chat channels and file the action items as tracked work items on its own, cutting out manual copy-and-paste. (#272)

## Campaigns

- **[Feature]** **Bring the Campaigns area into New Adsmith Frontend** — The Campaigns module from the older system isn't here yet. This high-priority work adds it back so you can view, create, edit, and configure campaigns and their offer groups directly in the new product. (#200)

## Users

- **[Task]** **Closing the gaps in the Users area** — A detailed review compared the older Users screens to the new ones and highlighted missing pieces (like bulk actions and extra columns). This work tracks bringing those capabilities into New Adsmith Frontend. (#80)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Some parts of the Flow form appear unstyled or awkwardly stacked. This cleanup restores proper styling and side-by-side field layouts so the form looks consistent with the rest of the product. (#152)

## Reports & Data

- **[Task]** **Confirm report numbers match the legacy system** — During testing, Dashboard report totals didn't line up with the older system. We're investigating where the difference comes from and will either fix it or confirm the numbers are correct, so you can trust the reports. (#271)

## Link Testing

- **[Bug]** **Clear error when a link is invalid** — Testing an invalid link currently dumps you back on the Dashboard with no explanation. This fix shows a proper error message instead, so you know the test failed and why. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: b7f987d297111c564a35e8760801ad27f22b7c308e48310ee46a3058a3fdf0e9 -->
