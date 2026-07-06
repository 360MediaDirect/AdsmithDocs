# Open Issues — Plain-Language Overview

_Last updated 2026-07-06 01:34:40 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit it, the app will hold it for you and warn if a colleague already has it open, so nobody's changes get silently wiped out. If someone changed a record while you had it open, you'll be prompted to reload instead of losing their work. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when, across offers, placements, advertisers, modals, flows and more — including automated changes. You'll be able to search by record, person, action or date and see a "history" on each item, making it easy to answer "who changed this and when?" (#276)
- **[Feature]** **Clean up controls that don't actually do anything** — Several settings currently look like they work but have no effect (the Advertiser "Web Presence" tab, certain user permission toggles, some Data Client and Pre-Ping options). These will either be made functional or removed so the screens only show controls that genuinely do something. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you back on the Dashboard with no explanation. This fix will show a proper error result so you know the link failed. This one is nearly finished. (#239)

## Surveys
- **[Feature]** **Make survey design settings actually change the survey** — An end-to-end review to ensure every option on the Design tab is truly reflected in the live survey a visitor sees, with any "dead" options fixed or removed. (#288)
- **[Bug]** **Turn on the rest of the survey styling options** — Today only a couple of the ~30 survey styling and behavior settings (colors, buttons, header text, legal text, progress bar and more) actually affect what visitors see. This work connects the remaining settings so what you configure is what gets shown. This one is well underway. (#290)
- **[Feature]** **Finish connecting a few remaining survey settings** — A follow-up to the styling work above that wires up the last handful of Design-tab options (like widget height and display format) and cleans up any that aren't used. (#293)
- **[Bug]** **Show voucher codes and info links on the live survey** — For affected data clients, the custom voucher-code question and the privacy/terms/details links are set up in the admin but don't appear on the live survey page (they do in the legacy app). This fix restores them, which matters for both the visitor experience and compliance. (#291)

## Placements
- **[Feature]** **Better control over offer order and filtering** — Building on the earlier drag-to-reorder work, this sets new placements to use your manual offer order by default (so your arrangement is actually respected) and adds a way to filter the available offers list by category. (#275)
- **[Feature]** **Preview your unsaved changes** — On placement and offer edit pages, the Preview button will show your current edits before you save, instead of only the last saved version — so you can check changes without saving first. (#292)

## Dashboard
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (e.g. to a spreadsheet) for your own reporting and analysis. (#286)
- **[Task]** **Confirm dashboard numbers match the old system** — An investigation into why some Dashboard report figures differed from the legacy app, to pin down the cause and confirm the numbers can be trusted. (#271)

## Offers
- **[Bug]** **Stop offer settings from getting lost before the live widget** — Several saved offer options (including the Modal-tab fields and other flags) currently never make it through to the live experience. This work ensures each saved option is either delivered and used, or removed if it isn't needed. (#295)

## Modals
- **[Feature]** **Make the Modal Design tab do something (or remove it)** — Right now none of the six Modal Design tab fields (header title, subtitle, colors, progress bar, etc.) affect the modal visitors see. They'll either be connected so they work or removed so the tab isn't misleading. (#294)

## Flows
- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned — plain text boxes, unstyled color pickers, and paired fields stacking vertically instead of side by side. This tidies up the form so it matches the polished look of the Placement and Modal forms. Partly done, with the rest handled carefully to avoid disrupting other tabs. (#152)

## Campaigns
- **[Feature]** **Bring the Campaigns area to the new platform** — The Campaigns module from the old admin isn't available yet in New Adsmith Frontend. This high-priority work adds it back so you can create, edit and manage campaigns and offer groups — including titles, questions, CTA text, offer handling and marketing partners — just like in the legacy system. (#200)

## Users
- **[Task]** **Compare the Users area to the old system** — A detailed review of the Users screens against the legacy version to spot missing capabilities (like bulk role changes, two-factor status, and last-login info) and prioritize what to add next. (#80)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the product against realistic data for verification and user testing, locked to read-only so testing can't accidentally change real records. Nearly complete. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads team chat discussions and files the resulting to-dos as tracked issues automatically, so action items don't get lost. This has no direct effect on the product screens. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
