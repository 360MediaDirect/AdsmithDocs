# Open Issues — Plain-Language Overview

_Last updated 2026-07-04 15:24:24 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Survey

- **[Feature]** **Make every survey design setting actually change the survey** — Right now many styling and behavior options on the Placement Design tab are saved but don't affect what visitors see. This work connects those settings end-to-end so what you configure is what appears, and audits every entity's form options to catch any that aren't fully wired. (#288)
- **[Bug]** **Turn on the survey styling options that currently do nothing** — Around 30 survey styling and behavior settings (colors, continue button, answer style, header, legal text) can be set today but only two actually reach the live survey. This makes the rest work, so your customizations show up for visitors. (#290)
- **[Bug]** **Show voucher codes and info links on the live survey again** — For affected data clients, the custom voucher-code line and the privacy/terms/details links are configured but not appearing on the new survey page, though they show in the legacy app. This restores them, which matters for passing leads and staying compliant. (#291)
- **[Feature]** **Finish connecting the last few Placement design settings** — A follow-up to the survey styling work that wires up the remaining settings (like survey height and display format) or cleanly removes any that won't be used, so no option in the form is a dead end. (#293)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record, one person's save can silently wipe out the other's changes. This adds an editing lock and a warning so you'll see "being edited by {name}" and won't lose work. (#267)
- **[Feature]** **A searchable history of who changed what and when** — Every manual and automated change to your entities will be recorded, and admins will get a searchable Audit Log page plus a history view on each record, making it easy to answer "who changed this?" (#276)
- **[Feature]** **Clean up admin controls that don't actually do anything** — Several settings across Advertisers, Users, Data Clients, and Pre-Pings are saved but have no effect. These will be removed or hidden (or properly implemented) so the admin only shows controls that really work. (#296)
- **[Bug]** **Show a clear error when a tested link is invalid** — Testing an invalid link currently just sends you to the dashboard with no explanation. After this fix you'll get a clear failure message instead. (#239)

## Placements

- **[Feature]** **Better offer ordering and filtering on Placements** — Building on recent drag-to-reorder work, this makes new placements default to Manual Order (so your arranged order is respected) and adds a way to filter the available offers list by category. (#275)
- **[Feature]** **Preview your unsaved changes before saving** — On placement and offer edit pages, Preview currently shows the last-saved version. This upgrade lets the preview reflect your in-progress edits, so you can check changes without saving first. (#292)

## Dashboard

- **[Task]** **Confirm dashboard numbers match the legacy system** — During testing, some dashboard report figures didn't line up with the old system. This investigation pins down where any differences come from and confirms the numbers can be trusted. (#271)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (for example, as a spreadsheet) instead of only viewing it on screen. (#286)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a test copy of the product using production-like data that can't be changed, so the team can verify things against realistic data without touching anything live. (#270)
- **[Feature]** **Turn meeting conversations into tracked tasks automatically** — A helper that reads designated chat channels and files the action items as tracked work items, cutting out manual copy-and-paste and reducing missed follow-ups. (#272)

## Offers

- **[Bug]** **Stop losing saved offer settings before they reach visitors** — Several saved offer options (including all Modal-tab fields and other flags) currently get dropped on their way to the live widget. This makes sure each option either reaches visitors or is clearly documented as storage-only. (#295)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — Every field on the Modal Design tab is currently saved but has no effect on the visitor modal. This will either connect those fields so they display or remove the tab if the modal is meant to be header-less. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or broken, with fields stacking oddly and plain-looking textareas and color pickers. This tidies the layout so it matches the polished look of the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns area into New Adsmith Frontend** — The Campaigns feature from the legacy admin isn't in the new platform yet. This adds it back so you can view, create, edit, and configure campaigns and their offer groups — a high-priority, core capability. (#200)

## Users

- **[Task]** **Close the gap between the old and new Users area** — A review comparing the legacy Users management with the new one, identifying missing pieces (like bulk actions and login/2FA details) so the new Users area reaches full parity. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
