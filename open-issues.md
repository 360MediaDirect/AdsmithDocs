# Open Issues — Plain-Language Overview

_Last updated 2026-07-03 20:25:05 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make every survey design setting actually take effect** — Right now many of the survey Design-tab customizations you set (colors, fonts, header text, and more) don't change what visitors see, even though the screen suggests they do. This work connects every design option end-to-end so what you configure is what shows, and audits all entity forms to confirm nothing is left unwired. (#288)
- **[Bug]** **Survey styling settings that don't reach the live widget** — About 30 look-and-feel options on the Placement Design tab are saved but ignored by the live survey, so only a couple currently work. This fix wires the rest through so colors, buttons, question text, headers, and legal text all display as chosen. (#290)
- **[Feature]** **Finish the last few Placement survey settings** — A follow-up to the survey styling work: a handful of settings (like iFrame height and display format) are still not reaching the live widget. Each remaining option will either be made to work or removed so the form only shows controls that do something. (#293)
- **[Bug]** **Missing voucher code and info links on the live survey** — For certain data clients, the custom voucher-code question and the privacy/terms/details links appear in the old app but not the new survey page, even though they're set up correctly. This restores both so visitors see the required voucher code and compliance links. (#291)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record, one person's save can silently wipe out the other's changes. This adds an editing lock that shows when someone else is already editing, plus a warning if a record changed while you had it open, across all entity screens. (#267)
- **[Feature]** **A searchable history of who changed what** — There's currently no way to see who paused an offer, edited a placement, or changed a setting and when. This adds a complete, searchable audit log of every manual and automated change, with a history view on each record's detail page. (#276)
- **[Feature]** **Tidy up admin controls that don't do anything** — Several settings across Advertisers, Users, Data Clients, and Pre-Pings are saved but have no effect, which is confusing and misleading. These will be removed or hidden (or properly implemented), so every control you see actually works. (#296)

## Placements & Offers

- **[Feature]** **Preview your unsaved changes before saving** — On placement and offer edit pages, Preview currently shows the last-saved version, so you have to save first to see a change. This upgrade makes Preview reflect your current, unsaved edits. (#292)
- **[Feature]** **Better control over the offer list on placements** — Building on the drag-to-reorder work, this makes manual ordering the default for new placements (so your chosen order is actually used) and adds a way to filter the available offers by category. (#275)
- **[Bug]** **Saved offer options that never reach the live widget** — A number of offer settings, including the Modal-tab fields, Display URL, and several data-client flags, are saved but dropped before they reach the live experience. Each will be either wired up and used or removed from the form so nothing is misleading. (#295)

## Dashboard

- **[Feature]** **Export your day-by-day breakdown** — A high-priority addition that puts an export button on the breakdown-by-day view, so you can download that data (for example as a spreadsheet). (#286)
- **[Task]** **Confirm new report numbers match the old system** — During testing, some dashboard figures didn't line up with the legacy app. This investigation compares the two over the same dates, pinpoints any differences, and either fixes them or confirms the numbers are correct. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — The entire Modal Design tab (header title, subtitle, colors, progress bar) is currently saved but never shown to visitors. Each field will either be made to display in the visitor modal or removed from the form. (#294)

## Users

- **[Task]** **Bringing the Users area up to par with the old system** — A detailed review comparing the old and new Users screens found gaps like bulk actions, two-factor status, last-login info, and a few form fields. This documents what's missing and prioritizes it so the new Users area matches what you're used to. (#80)

## Flows

- **[Task]** **Fix the visual styling on the Flow form** — Parts of the Flow form look unstyled or broken, with plain textareas, unpolished color pickers, and paired fields stacking vertically instead of side by side. This cleanup makes the Flow form look consistent with the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — Campaigns from the old admin haven't been rebuilt yet, so there's currently no way to create or manage campaigns and offer groups in New Adsmith Frontend. This high-priority work adds a Campaigns area matching the legacy features. (#200)

## Link Testing

- **[Bug]** **Show a clear error when a link is invalid** — Testing a bad link currently just sends you to the dashboard with no explanation. This fix makes Link Testing display a clear failure message so you know the link didn't pass. (#239)

## Behind the Scenes

- **[Task]** **A safe, look-only test environment** — Setting up a staging copy of the product connected to production-like data for review and testing, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels and automatically creates or updates tracked issues from action items, replacing today's manual copy-paste process. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
