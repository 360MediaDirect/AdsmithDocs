# Open Issues — Plain-Language Overview

_Last updated 2026-07-07 18:40:06 UTC · 23 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Warn when two people edit the same record** — When you open a record to edit, New Adsmith Frontend will let you know if someone else already has it open, and will stop a save from silently overwriting their changes. You'll see a clear "locked by" message and a prompt to reload if the record changed while you were working. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when across offers, placements, advertisers, modals, flows, and more — including automated changes — so you can look up "who edited this and when" and view a history right from an entity's detail page. (#276)
- **[Feature]** **Tidy up settings that don't do anything** — Several controls that currently save but have no effect (an advertiser's Web Presence links, certain user permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden so the screens only show settings that actually work. (#296)
- **[Bug]** **Invalid link tests now show a real result** — When you test a link that isn't valid, you'll get a clear error message instead of being unexpectedly bounced to the Dashboard. A small fix, nearly done. (#239)
- **[Task]** **Decide the future of the old file-share page** — We're confirming whether the legacy file-share page is still needed and, if so, where it belongs in New Adsmith Frontend — otherwise it will be formally retired. (#328)

## Surveys

- **[Feature]** **Make every Design tab setting actually work** — We're reviewing all customization options across the product to ensure each one you set is truly reflected in the live survey, with no dead settings that look active but do nothing. (#288)
- **[Bug]** **Survey styling settings that currently have no effect** — Many Design tab options (colors, continue button, question text, header, legal text) are saved but don't yet change what visitors see. This work connects them so your styling choices appear on the live survey. (#290)
- **[Feature]** **Finish connecting the remaining Design tab settings** — A follow-up to make the last few survey styling and behavior options (such as widget height, display format, and skip settings) take effect on the live widget — or remove them if they're not needed. (#293)
- **[Bug]** **Voucher code and info links missing on the live survey** — A configured custom question (like a voucher code) and the privacy/terms/details links are saved in the admin but not showing on the live survey page as they did before. This restores them for visitors. (#291)

## Offers

- **[Bug]** **Some saved offer settings never reach the live page** — Several saved offer options (including Modal-tab fields and a few backend flags) are being dropped before they reach visitors. This makes sure each saved option either works end-to-end or is cleaned up if it's not needed. (#295)
- **[Task]** **Auto-register offers should respect visitor targeting** — Auto-register offers currently fire for every visitor, ignoring age, gender, state, ZIP, and device targeting. We're confirming the correct behavior and making these offers honor targeting so they don't reach people they should exclude. (#333)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical offer data, replacing the informal manual review and giving a helpful gut-check at intake. (#322)

## Placements

- **[Feature]** **Preview your unsaved changes** — The Preview button on Placement and Offer edit pages will show the changes you're currently making, so you can check your edits without having to save first. (#292)
- **[Feature]** **Bring back the banner placement template** — The older banner placement style isn't available in New Adsmith Frontend yet. We're confirming whether it's still in use and, if so, restoring it. (#326)

## Behind the Scenes

- **[Task]** **Staging environment for safe testing** — Setting up a testing environment that uses production-like data in a read-only, safe way, so changes can be verified against realistic data without any risk of altering live records. (#270)
- **[Feature]** **Automatic issue capture from Slack** — A helper that reads designated Slack conversations and turns action items into tracked work items automatically, cutting out manual copy-and-paste. (#272)

## Reports

- **[Task]** **Confirm report numbers match the legacy system** — Testing found dashboard report figures that didn't line up with the old system. We're comparing the two over a fixed date range to find any differences, explain them, and confirm the numbers are accurate. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — Every field on the Modal Design tab currently saves but has no effect on the visitor's modal. We'll either connect these fields so they display, or remove the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or awkwardly laid out (plain text boxes, unstyled color pickers, fields stacked instead of side-by-side). This brings its appearance in line with the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — Campaign management (creating and editing campaigns, configuring settings, and managing offer groups and their offers) isn't available yet in the new platform. This high-priority work adds it to match the legacy system. (#200)

## Users

- **[Task]** **Close the gaps in the Users area** — A review comparing the old Users management screens with the new ones, so missing capabilities (like bulk actions, extra columns, and additional filters) can be prioritized and added. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 0f0dc75345ae083c3f2607503afd91bf3b9663925bf97592fab1f9e589c4ec62 -->
