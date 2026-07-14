# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 05:52:11 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit, others will see it's being worked on, and you'll be warned if someone changed it while you had it open — so no one's work gets silently lost. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will let administrators see who changed what and when across offers, placements, advertisers, and more, including automatic system changes — making it easy to track down "who edited this?" (#276)
- **[Feature]** **Clean up buttons and fields that do nothing** — Several controls that look active but have no effect (like the Advertiser Web Presence fields and certain user-permission toggles) will be removed or hidden, so what you see on screen reflects what actually works. (#296)
- **[Task]** **Bring the Users area up to the old system's capabilities** — A review comparing the new Users screens with the legacy version, identifying missing pieces like bulk actions, last-login info, and two-factor status so they can be added back. (#80)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will show a proper failure message instead of unexpectedly sending you to the Dashboard. (#239)
- **[Task]** **Decide the future of the legacy file-share page** — A quick review of whether the old file-share page is still needed or can be retired, so nothing useful is dropped by mistake. (#328)

## Offers
- **[Bug]** **Success tracking pixels now fire reliably** — Conversion pixels set up on offers currently never fire; this fix makes them work so attribution and revenue tracking are no longer silently lost. (#297)
- **[Bug]** **Saved offer settings actually reach the live experience** — A number of offer options are saved but never make it to what visitors see; this fix ensures each saved setting is either used or clearly removed. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently ignore age, gender, state, zip, and device targeting; this ensures they only fire for the right visitors (or the difference is documented as intentional). (#333)
- **[Feature]** **Preview your unsaved changes on placements and offers** — The Preview button will show your current edits instead of only the last-saved version, so you can check changes before committing them. (#292)
- **[Feature]** **Performance projections for new offers** — An automated, data-driven estimate of how a new offer is likely to perform based on past offers, replacing the informal manual gut-check. (#322)

## Data Clients
- **[Feature]** **Restore after-success delivery steps for clients** — Post-conversion delivery and redirect behavior from the old system will be brought over, so clients that rely on it keep working on the new platform. (#327)
- **[Feature]** **Bring over custom pre-ping checks for data clients** — Custom serve-time validation used by hundreds of data clients isn't running yet on the new platform; this restores those checks so lead qualification behaves as expected. (#338)

## Surveys
- **[Feature]** **Design-tab options fully carry through to the survey** — A sweep to make sure every design and customization option you set actually shows up in the live survey, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings** — Options like iframe height and display format will properly take effect in the survey widget, and any options that aren't wired up will be either connected or removed. (#293)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the product using production-like data for testing and verification, with safeguards so nothing can be accidentally changed. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads team chat and files the resulting to-dos as tracked issues, reducing manual copy-and-paste. (#272)

## Reports
- **[Task]** **Confirm report numbers match the old system** — An investigation into why some Dashboard report figures differ from the legacy app, so the numbers you rely on can be trusted and verified. (#271)

## Campaigns
- **[Feature]** **Add the missing Campaigns module** — Bring campaign management to the new platform, letting you view, create, and edit campaigns and manage offer groups just like the old admin system. (#200)

## Flows
- **[Task]** **Fix the look of the Flow form** — Cleaning up styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields display neatly instead of looking broken or misaligned. (#152)

## Modals
- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The modal header and progress-bar design fields currently have no visible effect; they'll either be connected to the visitor modal or removed so the tab isn't misleading. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
