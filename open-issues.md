# Open Issues — Plain-Language Overview

_Last updated 2026-07-04 23:20:48 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else already has a record open for editing, you'll see a clear "locked by {name}" notice and the form will stay read-only until they're done, so changes can no longer be silently wiped out. (#267)
- **[Feature]** **Searchable history of every change** — A new admin Audit Log will record who changed what and when — across offers, placements, advertisers, modals, and more — and let you look up an item's full history from its own screen. Great for answering "who changed this?" (#276)
- **[Feature]** **Clean up settings that don't actually do anything** — Several admin controls (Advertiser "Web Presence" fields, some user permission toggles, and a few Data Client and Pre-Ping options) currently save but have no effect. They'll be removed or hidden so the screens only show controls that really work. (#296)
- **[Task]** **Review of the old vs. new Users area** — A behind-the-scenes comparison of the legacy user management against New Adsmith Frontend, documenting which features still need to be brought over (like bulk actions and last-login details). (#80)
- **[Bug]** **Clear error when testing a bad link** — Entering an invalid link in Link Testing currently drops you onto the Dashboard with no explanation. Once fixed, you'll get a proper failure message instead. (#239)

## Surveys
- **[Feature]** **Make survey design options actually take effect** — A full sweep to ensure every choice on the Design tab is reflected in the live survey, with a wider check across all screens to catch any option that looks active but doesn't do anything yet. (#288)
- **[Bug]** **Turn on the rest of the survey styling options** — Most Design-tab settings (colors, continue button, question text, header, legal text) are saved but never appear on the live survey. This wires them up so what you set is what visitors see. (#290)
- **[Bug]** **Show the voucher code and info links on live surveys** — A configured voucher code line and the privacy/terms/details links aren't appearing on the new survey page even though they show in the old app. This restores them so visitors and compliance links display correctly. (#291)
- **[Feature]** **Finish the last few survey Design-tab settings** — A handful of remaining options (like survey height and display format) still don't reach the live widget. Each will either be wired up or removed so nothing on the form is misleading. (#293)

## Placements & Offers
- **[Feature]** **Better control over the offer list on placements** — New placements will default to your manual offer order (so drag-to-reorder actually sticks), and you'll be able to filter the available offers by category to find them faster. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit screens will show your current edits without forcing you to save first, so you can check a change before committing to it. (#292)
- **[Bug]** **Stop offer settings from being lost before they reach the live page** — Several saved offer options (including Modal-tab fields and "Force More Info Visible") never make it to the live widget today. Each will be carried through and used, or cleaned up if it isn't needed. (#295)

## Dashboard
- **[Task]** **Confirm Dashboard numbers match the old system** — An investigation into why some Dashboard report figures differed from the legacy app, to pin down the cause and confirm the numbers can be trusted. (#271)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example as a spreadsheet) for your own reporting. High priority. (#286)

## Behind the Scenes
- **[Task]** **A safe staging environment for testing** — Setting up a look-but-don't-touch copy of the system against realistic data, so changes can be verified before they reach live. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels, spots action items, and files them automatically (avoiding duplicates) so nothing from meetings slips through the cracks. (#272)

## Campaigns
- **[Feature]** **Bring the Campaigns module into New Adsmith Frontend** — Campaign management from the old admin isn't available yet in the new platform. This adds the ability to view, create, edit, and configure campaigns and their offer groups. High priority. (#200)

## Modals
- **[Feature]** **Make the Modal Design tab count** — The Modal Design tab's settings (header text, colors, progress bar) currently save but never show on the visitor modal. They'll either be wired up to display or removed so the tab isn't misleading. (#294)

## Flows
- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unfinished, with plain textareas, unstyled color pickers, and paired fields stacking awkwardly. This tidies up the layout to match the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
