# Open Issues — Plain-Language Overview

_Last updated 2026-07-06 17:01:15 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Protection against two people overwriting each other's edits** — When someone opens a record you already have open, you'll see a clear "locked by [name]" notice, and you'll be warned before a save could accidentally undo someone else's changes. This keeps edits from silently disappearing. (#267)
- **[Feature]** **A searchable activity log for every change** — Administrators will get a new Audit Log where you can see who changed what and when, across offers, placements, advertisers, modals, flows, and more — including automated changes. This makes "who touched this and when" easy to answer. (#276)
- **[Feature]** **Clean up controls that don't actually do anything** — Several settings that look editable but have no effect today (some Advertiser web-presence fields, certain user permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden so the screens only show controls that truly work. (#296)
- **[Bug]** **Invalid links should show an error, not send you to the Dashboard** — When you test a link that isn't valid, you'll get a clear failure message instead of being unexpectedly dropped on the Dashboard. A bug fix from testing. (#239)
- **[Task]** **Review of the Users area against the older system** — A behind-the-scenes comparison of the new Users screens versus the legacy version to identify any missing capabilities and plan how to close the gaps. (#80)

## Surveys
- **[Feature]** **Make every survey design option actually take effect** — A full review to ensure the customizations you set on the Design tab truly show up in the live survey, with any options that currently do nothing being fixed or removed. (#288)
- **[Bug]** **Turn on the many survey styling options that are being ignored** — Colors, buttons, question text, headers, legal text, and other survey settings you configure will finally appear on the live survey widget instead of being saved but unused. (#290)
- **[Bug]** **Show the voucher code and info links on the live survey** — Custom questions (like a voucher code) and the privacy/terms/details links configured for a Data Client will display on the survey page as they do in the older app. Important because these carry required and compliance information. (#291)
- **[Feature]** **Finish connecting the last few survey design settings** — The remaining Placement Design-tab options that #290 didn't cover will either be made to work on the live survey or removed if unused, so nothing on the tab is misleading. (#293)

## Offers
- **[Feature]** **Bring back the Campaigns module** — A high-priority addition that lets you view, create, edit, and configure campaigns and their offer groups in New Adsmith Frontend, matching what the older admin system offered. (#200)
- **[Feature]** **Preview offers and placements with your unsaved edits** — The Preview button on Offer and Placement edit pages will reflect the changes you've just made, so you no longer have to save first to see how they'll look. (#292)
- **[Bug]** **Stop dropping saved offer settings before they reach the live page** — Several offer options that are saved today never make it to what visitors actually see; this fixes them so they either display correctly or are removed if not needed. (#295)

## Dashboard
- **[Feature]** **Export the day-by-day breakdown** — A high-priority addition of an export button so you can download the breakdown-by-day data (for example to a spreadsheet) instead of only viewing it on screen. (#286)
- **[Task]** **Confirm Dashboard report numbers match the older system** — An investigation into why some report figures differed from the legacy app, so you can trust the Dashboard numbers are accurate. (#271)

## Behind the Scenes
- **[Task]** **A safe, view-only test environment using real-world data** — Setting up a separate space for reviewing and verifying the product against production-like data, with edits blocked so nothing can be changed by accident. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items automatically** — A helper that reads designated Slack channels, spots action items, and files them for the team without manual copy-and-paste. (#272)

## Flows
- **[Task]** **Fix the look of the Flow form** — Cleaning up styling issues so text boxes, color pickers, checkboxes, and paired fields on the Flow form appear neat and consistent with the Placement and Modal forms instead of looking unstyled. (#152)

## Modals
- **[Feature]** **Make the Modal Design tab meaningful** — The Modal Design tab's settings currently have no effect on what visitors see; they'll either be wired up to actually change the modal or removed so the tab isn't misleading. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: c980c506fbcd382110d038cce5f603588b1cc09d9e6eb33443e6941589c75595 -->
