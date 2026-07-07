# Open Issues — Plain-Language Overview

_Last updated 2026-07-07 23:20:47 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, New Adsmith Frontend will show that it's already being edited and warn you if it changed while you had it open, so no one's work gets silently overwritten. (#267)
- **[Feature]** **Searchable history of changes** — A new Audit Log will record who changed what and when across the app (including automated changes), so you can trace exactly how a record got to its current state. (#276)
- **[Feature]** **Remove settings that don't actually do anything** — Several admin controls (some Advertiser Web Presence fields, certain user-permission and Data Client options, a Pre-Ping setting) currently look active but have no effect. They'll be hidden or removed so the screens only show controls that really work. (#296)
- **[Task]** **Users screen gap review** — A review comparing the old Users area with the new one to catch missing pieces like bulk actions, last-login and two-factor status, so the new Users screen reaches full parity. (#80)
- **[Task]** **Decide the future of the old file-share page** — Confirm whether the legacy file-share page is still needed and either rebuild it in the new admin or formally retire it. (#328)
- **[Bug]** **Clear error when testing an invalid link** — Testing an invalid link currently dumps you back on the Dashboard. It will instead show a clear failure message so you know the link didn't work. (#239)

## Surveys & Modals

- **[Bug]** **Survey Design settings that finally take effect** — Many of the survey widget's styling and behavior options (colors, buttons, header, legal text and more) are saved but currently do nothing for visitors. They'll actually change what the survey looks like and how it behaves. (#290)
- **[Feature]** **Finish wiring the remaining Design settings** — The last few survey Design options that were left incomplete will either work as intended or be removed if they're not needed, so nothing on the screen is misleading. (#293)
- **[Bug]** **Voucher code and info links back on the live survey** — For affected Data Clients, the voucher code line and the privacy/terms/details links weren't showing on the new survey page like they did in the old system. They'll appear again, which matters for both leads and compliance. (#291)
- **[Feature]** **Design tab that matches what visitors see** — A full check to make sure every option on Design and other forms is truly connected end-to-end, so what you configure is what actually shows up. (#288)
- **[Feature]** **Fix or remove the Modal Design tab** — The Modal Design tab's fields currently have no effect on the modal visitors see. They'll either be made to work or removed so the tab isn't misleading. (#294)

## Offers & Campaigns

- **[Feature]** **Campaigns module in the new admin** — The Campaigns feature from the old system isn't in New Adsmith Frontend yet. It will be rebuilt so you can create, edit and manage campaigns and their offer groups. (#200)
- **[Feature]** **Preview your unsaved changes** — On Placement and Offer edit pages, Preview will show the changes you've just made rather than only the last saved version, so you can check your work without saving first. (#292)
- **[Bug]** **Offer settings that reach the live page** — Some saved offer options never made it through to what visitors see. This fix ensures those fields are either delivered and used, or clearly removed if they're not needed. (#295)
- **[Feature]** **Performance projection for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical offer data, giving Kurt a data-driven gut-check in place of the manual review that's being retired. (#322)
- **[Task]** **Auto-register offers should respect targeting** — Auto-register offers currently fire for every visitor, ignoring age, gender, state, zip and device targeting. This will confirm the correct behavior and make sure these offers don't fire for visitors they should exclude. (#333)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Standing up a staging setup that mirrors real data for testing and verification, locked to read-only so nothing can be accidentally changed. (#270)
- **[Task]** **Checking report numbers match the old system** — Investigating why some Dashboard report figures didn't line up with the legacy system, to pin down the cause and confirm the numbers can be trusted. (#271)
- **[Feature]** **Turning conversations into tracked work automatically** — An internal helper that reads team conversations and files the resulting to-dos as tracked issues, cutting out manual copy-paste. (#272)

## Data Clients & Pre-Pings

- **[Feature]** **Bring over "after-success" delivery steps** — The old system's post-conversion delivery and redirect steps for certain clients haven't been carried over yet. This will map each one to the new platform or confirm it's retired. (#327)
- **[Feature]** **Restore legacy pre-ping coverage** — The older file-based pre-ping used by some offers isn't in the new platform. This will port the missing behavior (or confirm the new pre-ping fully covers it) so no offer loses coverage. (#330)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form don't display with the right styling, so some fields and pickers look unfinished. This cleans up the appearance to match the other forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: db2e2e32afdf249c2931b9305c5b4e9f6e133e4b3e0fdf0fc98b37cd3f75c917 -->
