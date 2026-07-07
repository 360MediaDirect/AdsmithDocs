# Open Issues — Plain-Language Overview

_Last updated 2026-07-07 16:54:31 UTC · 23 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Survey
- **[Feature]** **Make every survey design option actually work** — We're checking that every customization on the Design tab (colors, buttons, header text, and more) flows all the way through to what visitors see, so no setting is left doing nothing. (#288)
- **[Bug]** **Design-tab styling settings not reaching the live survey** — Many survey styling and behavior settings you configure (colors, continue button, header, legal text) are saved but currently have no effect on the published survey. This work makes those settings take hold for visitors. (#290)
- **[Bug]** **Voucher code and info links missing on live surveys** — Custom questions like a voucher code, plus privacy/terms/details links set up on a Data Client, aren't showing on the new survey page even though they appear in the old app. They'll render correctly once fixed. (#291)
- **[Feature]** **Finish connecting the remaining survey design settings** — A handful of Design-tab settings (such as widget height and display format) still don't reach the survey; each will either be made to work or removed so the form only shows options that do something. (#293)

## General / Across the App
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record for editing, others will see it's locked and by whom, and you'll be warned if a record changed while you had it open — so changes are no longer silently lost. (#267)
- **[Feature]** **Searchable history of who changed what and when** — A new Audit Log will record every change to offers, placements, advertisers, and more (by people and by automated jobs), so administrators can look up who changed something and when. (#276)
- **[Feature]** **Remove admin controls that don't do anything** — Some settings across Advertisers, Users, Data Clients, and Pre-Pings are saved but have no real effect. These misleading controls will be removed or hidden so the admin only shows options that work. (#296)
- **[Task]** **Decide the future of the legacy file-share page** — The old file-share page has no equivalent yet; this is a decision on whether to rebuild it or formally retire it. (#328)

## Offers
- **[Bug]** **Saved offer options not reaching the live widget** — Several offer settings (including Modal-tab fields and "Force More Info Visible") are saved but never make it to what visitors see. Each will be connected or cleaned up so the form matches reality. (#295)
- **[Feature]** **Predict how a new offer will perform** — We're exploring an automated, data-driven estimate of a new offer's likely performance based on your historical offer data, to replace today's manual gut-check review. (#322)
- **[Task]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for every visitor, skipping age/gender/state/zip/device targeting rules that normal offers follow. This confirms and corrects the behavior so those offers only fire for the right visitors. (#333)

## Placements
- **[Feature]** **Rebuild the banner placement type** — The older banner placement style has no equivalent in the new platform yet. This confirms whether it's still needed and, if so, brings it back. (#326)
- **[Feature]** **Preview your unsaved changes** — On placement and offer edit screens, Preview will show your current edits before you save, instead of only the last-saved version — so you can check a change without saving first. (#292)

## Dashboard & Reports
- **[Bug]** **Invalid link test should show an error, not the dashboard** — When you test a bad link, you'll now get a clear failure message instead of being unexpectedly sent to the dashboard. (#239)
- **[Task]** **Confirm report numbers match the legacy system** — We're investigating why some dashboard report figures didn't line up with the old app, pinning down the cause, and confirming the numbers can be trusted. (#271)

## Flows
- **[Task]** **Fix the Flow form's appearance** — Parts of the Flow form look unstyled or out of place (plain text boxes, misaligned fields, unstyled color pickers). This tidies up the form so it matches the polished look of other screens. (#152)

## Campaigns
- **[Feature]** **Bring the Campaigns module to the new platform** — Campaign management from the legacy admin isn't available yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups — a core, high-priority capability. (#200)

## Modals
- **[Feature]** **Make the Modal Design tab work or remove it** — Every field on the Modal Design tab currently has no effect on the visitor modal. Each will either be made to work or removed so the tab isn't misleading. (#294)

## Data Clients
- **[Feature]** **Restore after-success delivery steps** — Certain post-conversion delivery and redirect behaviors from the old app haven't been carried over. This determines which are still needed and brings them back. (#327)

## Pre-Pings
- **[Feature]** **Restore legacy per-client pre-ping checks** — An older pre-ping method used by some offers hasn't been carried over, which could leave a gap for those offers. This is a high-priority effort to close that gap or confirm the new method fully covers it. (#330)

## Users
- **[Task]** **Compare the old and new Users areas** — A review documenting which features from the legacy Users management are still missing in the new admin (like bulk actions, last-login, and 2FA status), so the team can prioritize closing the gaps. (#80)

## Behind the Scenes
- **[Task]** **Set up a safe, read-only test environment** — A staging environment using prod-like data for verification, locked to read-only so testing can't change real records. (#270)
- **[Feature]** **Turn Slack conversations into tracked tasks** — A helper that reads designated Slack discussions and files the action items as tracked issues automatically, reducing manual copy-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 0f0dc75345ae083c3f2607503afd91bf3b9663925bf97592fab1f9e589c4ec62 -->
