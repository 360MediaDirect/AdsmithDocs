# Open Issues — Plain-Language Overview

_Last updated 2026-07-05 21:23:10 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's work** — When two team members open the same record at the same time, New Adsmith Frontend will warn you (or make the record read-only) so one person's changes can't silently erase another's. Expect a clear "someone else is editing this" message. (#267)
- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every create, edit, delete, and status change (by people and automated jobs) with a timestamp, so you can finally answer "who changed this and when" from a filterable screen and from each record's history. (#276)
- **[Feature]** **Tidy up settings that don't actually do anything** — Several controls that look active but have no effect (like the Advertiser Web Presence fields, some user permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden so the screens only show settings that truly work. (#296)
- **[Bug]** **Clearer result when testing an invalid link** — Entering an invalid link during Link Testing will show a proper error instead of quietly dropping you on the Dashboard. (#239)
- **[Task]** **Review of the Users area versus the old system** — A behind-the-scenes comparison documenting which Users features from the legacy admin still need to be brought over, to guide upcoming work. (#80)

## Surveys

- **[Feature]** **Make Design tab choices actually show up in the survey** — Every customization in the Design tab will be carried all the way through to what visitors see, and all form options across entities will be checked to make sure none are "dead ends." (#288)
- **[Bug]** **Most survey styling settings will finally take effect** — Today only a couple of the ~30 Design tab settings (like colors, buttons, headers, and legal text) change the live survey; this fixes the rest so what you configure is what visitors actually see. (#290)
- **[Bug]** **Voucher code and info links restored on the live survey** — The custom voucher-code question and the privacy/terms/details links that are set up in the Data Client will render on the survey page again, matching the old app (important for passing leads and compliance). (#291)
- **[Feature]** **Finish connecting the last few Design tab settings** — A follow-up to wire up the remaining survey settings (such as height and display format) or remove any that aren't needed, so nothing in the form is misleading. (#293)

## Placements

- **[Feature]** **Smarter offer ordering and filtering when building a placement** — New placements will default to your manual offer order (so drag-to-reorder actually sticks), and you'll be able to filter the available offers list by category/vertical instead of only searching by text. (#275)
- **[Feature]** **Preview your unsaved changes before saving** — The Preview button on Placement and Offer edit screens will show your current in-progress edits, so you no longer have to save first just to see how a change looks. (#292)

## Dashboard

- **[Task]** **Confirming Dashboard numbers match the old system** — An investigation into why some report figures differed from the legacy app, to pinpoint the cause and confirm the new numbers can be trusted. (#271)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example to a spreadsheet). High priority. (#286)

## Offers & Modals

- **[Bug]** **Saved offer settings that weren't reaching the live widget** — Several offer options were being dropped on the way to the live experience; each will either be properly connected or removed from the form so nothing you save quietly does nothing. (#295)
- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The Modal Design tab's fields currently have no effect on the visitor modal; this will either wire them up to actually display or remove them so the screen isn't misleading. (#294)

## Behind the Scenes

- **[Task]** **A staging environment for safe testing** — Setting up a test copy of New Adsmith Frontend using production-like data in read-only mode, so teams can verify things without any risk to live data. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — An internal helper that reads team chat and files or updates work items, reducing manual copy-paste when capturing action items. (#272)

## Flows

- **[Task]** **Cleaning up the look of the Flow form** — Fixing styling gaps so the Flow form's text boxes, color pickers, checkboxes, and paired fields display neatly and consistently with the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bringing the Campaigns area to New Adsmith Frontend** — The Campaigns module from the old admin isn't in the new platform yet; this adds it so you can create, edit, and manage campaigns and their offer groups (titles, questions, CTAs, offer handling, marketing partners, and more). A core, high-priority addition. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
