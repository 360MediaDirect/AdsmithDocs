# Open Issues — Plain-Language Overview

_Last updated 2026-07-04 21:19:40 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Task]** **Review of the Users area against the old system** — We're comparing today's Users screens with the previous version to spot capabilities worth bringing over, such as bulk role changes, two-factor status, and last-login details, so nothing important is lost in the move. (#80)
- **[Feature]** **Protection against two people overwriting each other's edits** — When you open a record to edit it, anyone else who opens the same record will see it's currently being edited (and by whom), and saves will warn you if the record changed while you had it open — preventing accidental lost changes. (#267)
- **[Feature]** **A searchable history/audit log** — A new admin page will record every change across the product — who made it, when, and what changed — including automated updates, so you can easily answer "who changed this and when?" (#276)
- **[Feature]** **Clean up settings that don't actually do anything** — Some controls (like the Advertiser "Web Presence" fields, certain user permission options, and a few Data-Client and Pre-Ping settings) currently save but have no effect. These will be removed or hidden so the screens only show options that truly work. (#296)
- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link will show a clear error message instead of quietly sending you back to the Dashboard. This fix is nearly complete. (#239)

## Surveys
- **[Bug]** **Design settings will finally change the live survey** — Many survey styling and behavior options (colors, buttons, header, legal text, and more) currently save but don't affect what visitors actually see. This work connects them so your choices appear on the live survey. (#290)
- **[Feature]** **Finish connecting the remaining survey Design settings** — A follow-up to the work above, making sure the last few settings (such as height and display format) either take effect on the live survey or are removed if unused. (#293)
- **[Feature]** **Make sure every Design option is reflected in the survey** — A full check of the customization options across all entity screens to confirm each one is truly wired through end-to-end, with no "dead" settings that appear to work but don't. (#288)
- **[Bug]** **Voucher code and info links restored on the survey page** — The custom voucher-code line and the privacy/terms/details links are configured in the admin but currently don't appear on the live survey. This fix brings them back, matching the older system. (#291)

## Placements
- **[Feature]** **Better ordering and filtering of offers** — New placements will default to your manual offer order (so hand-arranged offers actually show in that order), and you'll be able to filter the available offers list by category to find them faster. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit screens will show your current, unsaved edits instead of the last-saved version, so you can check a change before committing it. (#292)

## Dashboard
- **[Feature]** **Export the day-by-day breakdown** — A new export button lets you download the breakdown-by-day data (for example, to a spreadsheet) instead of only viewing it on screen. (#286)
- **[Task]** **Confirming Dashboard numbers match the old system** — We're investigating a case where Dashboard report figures didn't line up with the legacy app, to find any differences and confirm the numbers are accurate. (#271)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a testing environment loaded with production-like data where changes can't be saved, so the team can verify behavior without risk to live data. (#270)
- **[Feature]** **Turning conversations into tracked work items automatically** — A helper that reads team chat discussions and files the action items as tracked issues, cutting out manual copy-and-paste. (#272)

## Offers
- **[Bug]** **Saved offer options that weren't reaching the live page** — Several saved offer settings (including the Modal-tab options and a few others) are being dropped before they reach visitors. This fix ensures each option either shows up live or is cleanly removed if unused. (#295)

## Flows
- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacking instead of sitting side by side). This tidies up the layout to match the other forms. (#152)

## Modals
- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design tab's six settings currently have no effect on the visitor modal. They'll either be connected so they actually change the modal or removed to avoid confusion. (#294)

## Campaigns
- **[Feature]** **Bringing Campaigns management to the new product** — The Campaigns module from the older admin isn't available yet. This adds it back, letting you view, create, edit, and configure campaigns and their offer groups just like before. This is a high-priority addition. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
