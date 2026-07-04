# Open Issues — Plain-Language Overview

_Last updated 2026-07-04 06:59:35 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make every survey design setting actually take effect** — The Design tab lets you customize a survey's look and behavior, but many of those choices don't currently change what visitors see. This work connects all the design options end-to-end and reviews every entity's settings to make sure nothing is left disconnected. (#288)
- **[Bug]** **Survey styling options that don't reach visitors** — Around 30 survey styling and behavior settings (colors, continue button, question text, header, legal text) are saved but only two currently affect the live survey. This fix wires the rest through so what you configure is what visitors actually see. (#290)
- **[Bug]** **Voucher code and info links missing on the live survey** — A configured custom question (like a voucher code) and the privacy/terms/details links show in the old app but not the new one. This restores them on the live survey page, which matters for passing leads and staying compliant. (#291)
- **[Feature]** **Finish connecting the last few survey design settings** — A follow-up to the survey styling work: a handful of remaining options (such as widget height and display format) still need to be either made functional or removed so nothing in the form is misleading. (#293)

## General / Across the App

- **[Feature]** **Warn when two people edit the same record** — If a colleague changes a record while you have it open, this prevents your save from silently wiping out their work. You'll see a clear "someone else changed this — please reload" message and a note when a record is being edited by another user. (#267)
- **[Feature]** **A searchable history of every change** — A new admin Audit Log will record who changed what and when across the product, including automated updates, so you can easily answer "who changed this?" and view a history right from each record. (#276)
- **[Feature]** **Clean up buttons and toggles that do nothing** — Several admin controls (Advertiser Web Presence fields, some user permission toggles, and a few Data Client and Pre-Ping options) look active but have no effect. These will be removed or hidden so the interface only shows controls that actually work. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Testing an invalid link currently dumps you on the Dashboard with no explanation. After this fix you'll get a proper error message instead. (#239)

## Placements

- **[Feature]** **Better control over offer order and filtering** — Building on recent drag-to-reorder work, this makes new placements respect your manual offer order and lets you filter the available offers list by category so it's easier to find the right ones. (#275)
- **[Feature]** **Preview your unsaved changes** — On placement and offer edit pages, the Preview button will show the changes you're currently making instead of the last saved version, so you can check your work before committing. (#292)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example as a spreadsheet) for your own analysis. High priority. (#286)
- **[Task]** **Confirm dashboard numbers match the old system** — Reviewers noticed dashboard report figures didn't line up with the legacy system. This investigation pins down where the difference comes from and confirms the numbers can be trusted. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab do something** — Every field on the Modal Design tab currently has no effect on the visitor-facing modal. This work either connects those fields so they work or removes them if the modal is meant to stay simple. (#294)

## Offers

- **[Bug]** **Offer settings that never reach the live experience** — A number of saved offer options (including the Modal-tab fields, Display URL, and several backend flags) are being dropped before they reach visitors. Each will be either fully connected or removed so the form reflects reality. (#295)

## Flows

- **[Task]** **Fix the Flow form's broken styling** — Parts of the Flow form look unstyled or misaligned compared to other forms — plain text boxes, unstyled color pickers, and fields that stack awkwardly instead of sitting side by side. This tidies up the appearance. (#152)

## Campaigns

- **[Feature]** **Bring back the Campaigns area** — The Campaigns module from the old admin isn't in the new product yet, so campaigns and offer groups can't be managed here. This adds it back with the same abilities to view, create, configure, and edit campaigns. High priority. (#200)

## Users

- **[Task]** **Review what's missing in the new Users area** — A side-by-side comparison of the old and new Users screens to catalog which features (like bulk actions, extra columns, and additional filters) still need to be brought over. This is planning groundwork. (#80)

## Behind the Scenes

- **[Task]** **Set up a safe testing environment with real-like data** — Standing up a read-only staging copy of the product against production-like data so testing and verification can happen without any risk of changing live records. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads team chat and files the resulting to-dos automatically, reducing manual copy-paste when capturing action items. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
