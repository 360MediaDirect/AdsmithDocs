# Open Issues — Plain-Language Overview

_Last updated 2026-07-03 22:21:13 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make every Design-tab option actually change the survey** — Right now the survey Design settings all save, but many don't visibly affect the live survey. This work confirms each design customization flows through end-to-end so what you set is what visitors see, and audits every entity's form options to catch any that quietly do nothing. (#288)
- **[Bug]** **Turn on the survey styling options that were doing nothing** — About 30 survey styling and behavior settings (colors, continue button, answer style, header, legal text) were being saved but ignored on the live survey. Once fixed, these controls will genuinely change how the survey widget looks and behaves for visitors. (#290)
- **[Bug]** **Show voucher codes and info links on the live survey** — A configured custom question (like a voucher code) and the privacy/terms/details links currently appear in the old system but are missing on the new survey page. This restores them so visitors see the required voucher code and compliance links. (#291)
- **[Feature]** **Finish connecting the last few survey Design settings** — A handful of remaining Design-tab settings (such as survey height and question display format) still don't reach the live survey. Each will either be wired up to work or removed from the form so nothing misleads you. (#293)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record, one could unknowingly wipe out the other's changes on save. This adds an editing lock plus a warning if a record changed while you had it open, so no work is silently lost. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will get an audit log that records who changed what and when across offers, placements, and other records, including automated updates. This makes it easy to answer "who changed this and when" when troubleshooting. (#276)
- **[Feature]** **Clean up admin controls that don't do anything** — Several settings (like the Advertiser Web Presence fields, some user permission toggles, and a few Data Client and Pre-Ping options) are shown but have no effect. They'll be removed or hidden so the admin only shows controls that actually work. (#296)
- **[Bug]** **Show a clear error for invalid links when testing** — Testing an invalid link currently just dumps you back on the dashboard with no explanation. This is a nearly-finished fix so you'll get a clear failure message instead. (#239)

## Placements

- **[Feature]** **Better control over the offer list on placements** — Following earlier drag-and-drop improvements, this adds the ability to filter available offers by category and revisits whether manually ordered offers should be respected by default, so your chosen offer order actually takes effect. (#275)
- **[Feature]** **Preview your unsaved changes before saving** — On placement and offer edit pages, Preview currently only shows the last-saved version. This upgrade lets Preview reflect your current, unsaved edits so you can check changes without saving first. (#292)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A high-priority addition of an export button to the breakdown-by-day view, so you can download that data (for example as a spreadsheet) instead of only viewing it on screen. (#286)
- **[Task]** **Confirm dashboard numbers match the old system** — During testing, some dashboard report figures didn't line up with the legacy system. This investigation compares the two over the same dates to find and explain any differences and confirm the numbers are trustworthy. (#271)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the product using production-like data for testing and verification, locked to read-only so testing can't change real data. (#270)
- **[Feature]** **Turn Slack conversations into tracked to-dos automatically** — An internal helper that reads designated Slack channels and files the resulting action items as tracked work items, reducing manual copy-and-paste for the team. (#272)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly and plain-looking text boxes and color pickers. This tidies up the form so it matches the polished look of the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bring back Campaign management** — The Campaigns area from the old admin isn't in the new platform yet, so campaigns and offer groups can't be created or edited. This high-priority work adds a Campaigns module so you can view, create, configure, and update campaigns as before. (#200)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — Every field on the Modal Design tab currently saves but has no effect on the modal visitors see. Each field will either be wired up to actually work or removed so the tab isn't misleading. (#294)

## Offers

- **[Bug]** **Stop losing offer settings before they reach visitors** — Several saved offer options (including the Modal-tab fields, Display URL, and some data-client flags) never make it to the live widget. Each will be connected so it takes effect, or removed from the form if it isn't needed. (#295)

## Admin / Users

- **[Task]** **Review the Users area against the old system** — A detailed comparison of the Users screens in the new admin versus the legacy version, identifying missing pieces (like bulk actions and login/2FA details) and prioritizing what to add so the new Users area reaches full parity. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
