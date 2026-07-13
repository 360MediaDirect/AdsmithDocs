# Open Issues — Plain-Language Overview

_Last updated 2026-07-13 12:48:21 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Saved offer options aren't reaching the live experience** — Some settings you configure on an offer (like modal text, Display URL, and "Force More Info Visible") are currently saved but silently ignored on the live site. Once fixed, the options you set will actually take effect. (#295)
- **[Bug]** **Success tracking pixels never fire** — Conversion pixels set up under "Pixels to Fire on Success" aren't firing, so conversions go untracked. This fix makes your configured pixels fire as expected, restoring accurate attribution. (#297)
- **[Bug]** **Auto-register offers ignore targeting rules** — Auto-register offers are firing for everyone, even when you've set age, gender, state, zip, or device targeting. This high-priority fix makes them respect the same targeting rules as regular offers. (#333)
- **[Feature]** **Preview your unsaved edits on Offers and Placements** — The Preview button will show the changes you're currently making, so you no longer have to save first just to see how an edit looks. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An early, exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, replacing the informal manual gut-check. (#322)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else already has a record open for editing, you'll see a clear "locked by" notice, and you'll be warned before your save could wipe out their changes. Works across all entity screens. (#267)
- **[Feature]** **A searchable Audit Log** — A new admin page that records who changed what and when across the product (including automated changes), so you can finally answer "who edited this and when." (#276)
- **[Feature]** **Clean up controls that don't do anything** — Certain fields that look editable but have no effect (on Advertisers' Web Presence, some User permissions, and a few Data Client and Pre-Ping options) will be removed or hidden to avoid confusion. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you on the Dashboard with no explanation. After this fix you'll get a proper failure message right in the Link Testing screen. (#239)
- **[Task]** **Decide the future of the legacy File-Share page** — A quick review to confirm whether the old file-share page is still needed in the new product or can be retired. (#328)

## Surveys

- **[Feature]** **Design options that actually change the survey** — A thorough check to make sure every customization on the Design tab is reflected in what visitors see, with any "dead" options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Settings like iFrame height and display format will properly carry through to the live survey widget instead of being saved but ignored. (#293)

## Data Clients

- **[Feature]** **Restore after-success delivery behavior** — The post-conversion delivery and redirect steps from the old system are being brought over so client hand-offs after a successful lead work as before. (#327)
- **[Feature]** **Restore custom pre-ping validation** — Custom serve-time checks tied to hundreds of data clients aren't running in the new platform yet. This high-priority work brings that validation back so leads are screened as they were previously. (#338)

## Reports

- **[Task]** **Confirm report numbers match the legacy system** — An investigation into why some Dashboard report figures didn't line up with the old system, so you can trust the numbers you see. (#271)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — The Campaigns area from the old admin isn't in the new product yet. This high-priority work adds it back so you can create, edit, and manage campaigns and offer groups. (#200)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The Modal Design tab's fields currently save but don't affect what visitors see. This work will either wire those header and progress-bar settings through to the visitor modal or remove the tab. (#294)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned compared to other forms. This cleanup makes text boxes, color pickers, checkboxes, and paired fields display neatly. (#152)

## Users

- **[Task]** **Compare the old and new Users areas** — A documentation review listing what the Users screen can do today versus the old system, to guide which features still need to be added. (#80)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of the product loaded with production-like data for testing and verification, with writing disabled so nothing can be accidentally changed. (#270)
- **[Feature]** **Automatically turn conversations into tracked tasks** — A helper that reads designated chat channels and files new work items automatically, cutting out manual copy-and-paste when capturing action items. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
