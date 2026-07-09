# Open Issues — Plain-Language Overview

_Last updated 2026-07-09 07:10:57 UTC · 24 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Protection against two people overwriting each other's work** — When another admin is already editing a record, you'll see who has it open and be warned before your save can wipe out their changes. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will be able to see who changed what and when across the platform, including automated changes, making it easy to answer "who touched this record?" (#276)
- **[Feature]** **Clean up settings that don't actually do anything** — Controls that currently have no effect (such as the Advertiser Web Presence fields, certain user-permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden so screens only show settings that truly work. (#296)
- **[Task]** **Decide the future of the old file-share page** — A review to determine whether the legacy file-share page is still needed in the new platform or can be retired. (#328)
- **[Task]** **Consistent colors for alerts and banners** — Warning, info, success, and error banners will look the same on every page instead of drifting slightly from screen to screen. (#341)
- **[Bug]** **Clear error when testing an invalid link** — Instead of being dropped onto the dashboard, you'll get a clear failure message when a tested link is invalid. (#239)

## Surveys
- **[Feature]** **Make every survey design option actually work** — Customizations chosen on the design tab will reliably appear in the live survey, with a full check that no option is left disconnected. (#288)
- **[Bug]** **Restore the missing voucher code and legal links** — A high-priority fix so the voucher code line and the privacy/terms/details links show up on the live survey page, just as they did in the old system. (#291)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Settings like survey height and display format will take effect on the live survey instead of being saved but ignored. (#293)

## Offers
- **[Bug]** **Saved offer options will reach the live page** — Several offer settings that were being saved but never applied (including modal fields and "force more info visible") will actually take effect on the live experience. (#295)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical offer data, replacing today's manual gut-check review. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — A high-priority fix so auto-register offers no longer fire for visitors they should exclude by age, gender, state, zip, or device. (#333)

## Placements
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show the changes you're currently making, so you don't have to save first just to see them. (#292)
- **[Feature]** **Offer impressions in historical placement reports** — Older placement reports will show real offer-impression numbers instead of always showing zero. (#339)

## Pre-Pings
- **[Feature]** **Real-time offer checks at display time** — A high-priority change so that offers rejected by an advertiser's live check are hidden from the visitor right away. (#337)
- **[Feature]** **Bring legacy custom pre-ping checks into the new platform** — A high-priority effort to carry over the custom serve-time validation used by hundreds of data clients, so their checks keep running as before. (#338)

## Data Clients
- **[Feature]** **Restore post-conversion delivery behavior** — The legacy "after success" delivery and redirect steps for affected clients will be brought into the new platform so nothing is lost after a conversion. (#327)

## Reports
- **[Task]** **Confirm report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy app, so you can trust the numbers you see. (#271)

## Flows
- **[Task]** **Fix the look of the Flow form** — Textareas, color pickers, and checkboxes will be properly styled, and paired fields will sit side by side instead of stacking, matching the other forms. (#152)

## Modals
- **[Feature]** **Make the Modal design settings work — or remove them** — The Modal design tab (header text, colors, and progress bar) will either take effect on the visitor modal or be removed so it isn't misleading. (#294)

## Campaigns
- **[Feature]** **Bring the Campaigns module to the new platform** — A critical, high-priority addition so you can view, create, edit, and configure campaigns and their offer groups, matching what the old admin offered. (#200)

## Admin / Users
- **[Task]** **Review of the Users screen against the old system** — A behind-the-scenes comparison to catalog which Users features are still missing (such as bulk actions, last-login, and two-factor status) and prioritize them. (#80)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging version of the product against production-like data for verification, with saving locked off so testing can't change real records. (#270)
- **[Feature]** **Turn Slack conversations into tracked to-dos automatically** — A helper that reads designated Slack chats and files action items as tracked issues, reducing manual note-taking. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: e97c0c87fd1c264309b547c86ecde9d1b7abd3cebd9c6dc642ac728d6283da48 -->
