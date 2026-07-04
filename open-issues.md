# Open Issues — Plain-Language Overview

_Last updated 2026-07-04 13:30:53 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Survey

- **[Feature]** **Make every survey design setting actually work** — Right now many of the styling and behavior options you set on a survey are saved but don't change what visitors see. This work confirms every design-tab option flows all the way through to the live survey, with any unused options fixed or removed. (#288)
- **[Bug]** **Connect the rest of the survey Design-tab settings to the live widget** — Around 30 look-and-feel controls (colors, buttons, headers, legal text, progress bar) currently have no effect once saved. After this fix, those choices will appear on the survey visitors actually see. (#290)
- **[Bug]** **Show the voucher code and info links on the live survey** — A configured custom question (voucher code) and the privacy/terms/details links are set up in the admin but aren't showing on the new survey page like they did before. This restores them, which matters for both lead processing and compliance. (#291)
- **[Feature]** **Finish wiring the last few Placement design settings** — A handful of remaining survey settings (such as height and display format) still don't reach the widget. Each will either start working or be removed so nothing in the form is misleading. (#293)

## Placements & Offers

- **[Feature]** **Better default ordering and filtering for offers on a Placement** — New placements will default to your manual offer order (so the order you set is actually used), and you'll be able to filter the available offers list by category to find them faster. (#275)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — When editing a placement or offer, the Preview will reflect the changes you're making right now instead of only the last saved version, so you can check your work before saving. (#292)
- **[Bug]** **Stop offer settings from being lost before they reach the live widget** — Several saved offer options (including modal fields and display URL) currently never make it to the live experience. This ensures each option either takes effect or is cleanly removed so it's not misleading. (#295)

## Admin & Users

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else is already editing a record, you'll see a clear "locked by" notice, and you'll be warned if a record changed while you had it open — preventing accidental lost changes across all entity screens. (#267)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings (like Advertiser Web Presence fields, some user permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no real effect. These will be hidden or removed so the admin only shows controls that actually work. (#296)
- **[Task]** **Review the Users area against the previous system** — A detailed comparison of the old and new Users screens to spot missing capabilities (like bulk actions and last-login info) and plan what to bring over. This is groundwork to guide upcoming improvements. (#80)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — You'll get an export button on the breakdown-by-day view so you can download that data (for example as a spreadsheet) for your own reporting. This is a high-priority addition. (#286)
- **[Task]** **Confirm dashboard report numbers match the old system** — Some dashboard figures didn't line up with the previous platform during testing. This investigation pins down where the difference comes from and either fixes it or confirms the numbers are correct. (#271)

## General / Across the App

- **[Feature]** **A searchable history of every change** — A new admin Audit Log will record who changed what and when across the platform (both manual edits and automated updates), so you can easily answer "who changed this and when." (#276)
- **[Bug]** **Show a clear error for an invalid link when testing** — Testing an invalid link currently drops you back on the dashboard with no explanation. After this fix you'll see a proper failure message so you know the link didn't work. (#239)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only testing environment** — A staging copy of the product connected to realistic data, locked to read-only so testing can happen safely without changing anything. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — An internal helper that reads team conversations and files the resulting to-dos automatically, reducing manual note-taking. This is an internal workflow tool with no direct effect on your screens. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — Every field on the Modal Design tab currently has no effect on what visitors see. Each field will either start working on the visitor modal or be removed so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Fix the visual styling on the Flow form** — Parts of the Flow form look unpolished — plain text boxes, unstyled color pickers, and fields stacking oddly instead of sitting side by side. This tidies the form so it matches the look of the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bring back Campaign management** — The Campaigns area from the previous admin isn't in the new product yet, so campaigns and offer groups can't be created or managed here. This adds a full Campaigns module so you can view, create, configure, and edit campaigns again. This is a high-priority, core capability. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
