# Open Issues — Plain-Language Overview

_Last updated 2026-07-06 20:37:20 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When two team members open the same record at once, you'll see a clear "locked by someone else" note and a prompt to reload if it changed, so one person's work can no longer silently erase another's. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when across the whole platform — manual edits and automatic updates alike — so you can finally answer "who changed this offer and when." (#276)
- **[Feature]** **Cleaning up settings that don't actually do anything** — Several admin controls (Advertiser Web Presence fields, some user permission toggles, and a few Data-Client and Pre-Ping options) currently look active but have no effect. They'll be removed or hidden so what you see reflects what really works. (#296)
- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link currently dumps you back on the dashboard with no explanation; instead you'll get a clear error message telling you the link failed. (#239)

## Surveys

- **[Feature]** **Make sure Design-tab options actually change the survey** — We're checking that every styling and behavior option on the Design tab is truly reflected in the live survey, with no settings that appear to work but quietly do nothing. (#288)
- **[Bug]** **Survey styling settings that finally take effect** — Many Design-tab options (colors, continue button, header text, legal text and more) are saved but don't yet reach visitors. This wires them through so what you configure is what people actually see. (#290)
- **[Feature]** **Finishing the remaining survey styling settings** — A follow-up to complete the last few Design-tab options (like survey height and question display format) so every one either changes the widget or is removed if unused. (#293)
- **[Bug]** **Voucher code and info links showing on the live survey** — A configured voucher code line and the privacy/terms/details links don't appear on the new survey page even though they show in the legacy app. This restores them, which matters for both compliance and passing the lead. (#291)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button lets you download the breakdown-by-day data (for example to a spreadsheet) instead of only viewing it on screen. (#286)
- **[Bug]** **Offer Detail page failing for "Last Month"** — Opening an Offer Detail page with the date filter set to "Last Month" currently times out and shows an error. This fix gets that data loading reliably. (#318)
- **[Task]** **Confirming report numbers match the legacy system** — We're investigating why some dashboard report figures didn't line up with the old system, so you can trust the numbers are consistent. (#271)

## Placements

- **[Feature]** **Preview your unsaved changes before saving** — The Preview button on placement and offer edit pages will show your current in-progress changes, so you no longer have to save first just to see how an edit looks. (#292)
- **[Feature]** **Better defaults and filtering for the offer list** — Following earlier drag-to-reorder work, we're deciding whether new placements should default to Manual Order (so your chosen order is respected) and adding a way to filter available offers by category. (#275)

## Offers

- **[Bug]** **Saved offer options that weren't reaching the live widget** — Several saved offer settings (including Modal-tab fields and Display URL) never made it to the live experience. Each will be properly connected or removed so nothing looks active while doing nothing. (#295)

## Modals

- **[Feature]** **Making the Modal Design tab do something** — All six fields on the Modal Design tab are currently saved but have no effect on what visitors see. They'll either be wired up to the visitor modal or removed to avoid confusion. (#294)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacking oddly). This tidies up the layout to match the polished look of other forms. (#152)

## Campaigns

- **[Feature]** **Bringing Campaigns into the new platform** — The Campaigns area from the older admin isn't in New Adsmith Frontend yet. This adds it back so you can create, edit, and manage campaigns and their offer groups. High priority. (#200)

## Users

- **[Task]** **Reviewing what's missing from the Users area** — A review comparing the older Users screens to the new ones, so we know which features (like bulk actions and login/2FA details) still need to be brought over. (#80)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging version that mirrors real data for testing, with writing locked off so nothing can be changed by accident. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — A new helper will read team chat and file the resulting to-dos as tracked issues automatically, cutting out manual copy-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6c27af732f3641fd9b535e157afcb427a79ad241cf9415444c675c49de3c7588 -->
