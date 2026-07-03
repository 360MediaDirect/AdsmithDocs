# Open Issues — Plain-Language Overview

_Last updated 2026-07-03 17:30:47 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When you open a record to edit it, the app will hold your place and warn if someone else is already editing it, and it will stop a save from quietly wiping out a colleague's changes. You'll see a clear "someone else changed this — please reload" message instead of silently losing work. (#267)
- **[Feature]** **Campaigns management, brought into New Adsmith Frontend** — The Campaigns area from the older admin isn't in the new platform yet. This adds it back so you can view, create, edit, and configure campaigns and their offer groups just like before. High priority, since campaign management is a core task. (#200)
- **[Feature]** **A searchable history of who changed what** — Every manual and automated change to your records (offers, placements, advertisers, and more) will be logged with a timestamp and the person or system that made it, viewable in a new searchable Audit Log and on each record's history. This makes it easy to answer "who changed this and when." (#276)
- **[Feature]** **Clean up settings that don't actually do anything** — Some admin options (certain Advertiser web-presence fields, a few user-permission toggles, and some Data Client and Pre-Ping settings) are shown but currently have no effect. These will be removed or hidden so the screens only show controls that genuinely work. (#296)
- **[Bug]** **Invalid links in Link Testing now show a proper error** — Testing a bad link currently dumps you onto the dashboard with no explanation. After this fix you'll get a clear failure message right in the Link Testing screen. Nearly complete. (#239)
- **[Task]** **Users area feature review** — A documentation exercise comparing the older Users screens with the new ones to catch anything missing (like bulk role changes, last-login, and two-factor status). This guides what gets added next; no immediate change on screen. (#80)

## Surveys

- **[Feature]** **Make every survey design option actually take effect** — A review across all entity screens to confirm each design/customization setting you configure is truly reflected in the live survey, with any "dead" options fixed or removed. You'll be able to trust that what you set is what visitors see. (#288)
- **[Bug]** **More survey styling controls will finally work** — Around thirty color, button, header, and layout settings on the Placement Design tab are saved today but don't reach the live survey. This wires them through so your customizations actually change what visitors see. Well underway. (#290)
- **[Feature]** **Finish connecting the remaining Placement Design settings** — A follow-up that hooks up the last few survey settings (such as height and display format) or removes ones that were never intended to do anything, so nothing on the Design tab is misleading. (#293)
- **[Bug]** **Voucher codes and info links will show on the live survey again** — For affected Data Clients, the custom voucher-code line and the privacy/terms/details links are configured but not appearing on the survey page (they do in the older app). This restores them, which matters for both the customer experience and compliance. High priority. (#291)

## Dashboard

- **[Feature]** **Pick report dates right from the dashboard** — Instead of hand-editing the web address to change the reporting range, you'll get date and day controls built into the dashboard toolbar. The link still updates so reports stay shareable. Nearly complete. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (for example, to a spreadsheet) for your own analysis. High priority. (#286)
- **[Task]** **Confirm dashboard numbers match the older system** — An investigation into why some dashboard report figures differ from the legacy app, to pinpoint the cause and confirm the numbers can be trusted. Behind-the-scenes work that supports report accuracy. (#271)

## Offers

- **[Bug]** **Success pixels will fire as intended** — Conversion/postback pixels set up on an offer currently never fire because of a format mismatch, meaning lost tracking with no warning. This fixes it so a configured success pixel actually fires. High priority. (#297)
- **[Bug]** **Saved offer options will reach the live offer** — Several saved offer settings (including Modal-tab fields and Force More Info Visible) are being dropped before they reach the live widget. This ensures each saved option either takes effect or is clearly removed so nothing is misleading. (#295)

## Placements

- **[Feature]** **Preview your unsaved placement and offer edits** — Today the Preview button only shows the last-saved version, so you must save before you can see a change. This upgrade makes Preview reflect your current, in-progress edits. (#292)
- **[Feature]** **Better default order and filtering for offers on a placement** — Follow-up work to set new placements to use your manual offer order by default and to let you filter the available-offers list by category, so building an offer stack is faster and behaves as expected. (#275)

## Modals

- **[Feature]** **Make the Modal Design tab do something — or remove it** — The Modal Design tab's header and progress-bar fields are saved but currently have no effect on what visitors see. This either wires them into the live modal or removes the tab, so the screen no longer promises settings that don't work. (#294)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or stack awkwardly compared with other forms (text boxes, color pickers, and paired fields). This gives it a careful cleanup to match the rest of the app. Partly done. (#152)

## Properties

- **[Bug]** **Domain restrictions on Properties will actually apply** — Domain settings you save on a Property currently have no effect at runtime because of a mismatch between how they're saved and read. This makes domain allow-listing work again and updates existing records. (#300)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the platform using production-like data for verification, locked to read-only so testing can't change real data. No visible change in the product. (#270)
- **[Feature]** **Automatic issue capture from team chats** — An internal helper that turns action items mentioned in Slack into tracked work items automatically, reducing manual note-taking. This is an internal workflow tool, not part of the product screens. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 2ee3b9cbbc0f628c54f8d6c070246ea2ff85e92e5bc8c06cb62d5065d1d2eb4c -->
