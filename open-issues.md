# Open Issues — Plain-Language Overview

_Last updated 2026-07-07 15:00:44 UTC · 23 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Bug]** **Invalid links now show a clear error** — When you test a link that isn't valid, you'll get a proper error message instead of being unexpectedly dropped onto the Dashboard. This fix is nearly finished. (#239)
- **[Feature]** **Protection against two people overwriting each other's edits** — When you open a record to edit, others will see it's being worked on, and you'll be warned if someone changed it since you opened it — so nobody's work gets silently lost. (#267)
- **[Feature]** **A searchable history of who changed what** — A new audit log will record every change across the app, including who made it and when, so admins can easily trace how a record got to its current state. (#276)
- **[Feature]** **Cleaning up settings that don't actually do anything** — Several admin controls (Advertiser Web Presence fields, some user permission options, and a few Data Client and Pre-Ping settings) currently look active but have no effect. They'll be removed or hidden so the screens only show controls that truly work. (#296)
- **[Task]** **Deciding the future of the old File Share page** — A review to confirm whether the legacy file-share page is still needed in the new platform or can be retired. (#328)
- **[Task]** **Comparing the old and new Users screens** — A review of which features from the legacy Users area still need to be brought over, such as bulk role changes and login/2FA details. (#80)

## Surveys

- **[Feature]** **Making every survey design option actually work** — A thorough check to ensure each customization you set on the design tab is reflected in the live survey, with no dead options that quietly do nothing. (#288)
- **[Bug]** **Connecting survey styling settings to the live survey** — Right now only a couple of the many Design tab settings (colors, buttons, headers, legal text) change what visitors see. This wires up the rest so your styling choices take effect. (#290)
- **[Bug]** **Showing the voucher code and info links on the survey** — Items configured for a data client, like the voucher code line and the privacy/terms/details links, will appear on the live survey as they did in the older system. (#291)
- **[Feature]** **Finishing the remaining survey design settings** — Completes the last few styling and behavior options (such as widget height and display format) so they either take effect or are removed if they aren't needed. (#293)

## Offers

- **[Feature]** **Previewing offers and placements with your unsaved changes** — The Preview button will show the edits you've made right now, instead of only the last saved version, so you no longer have to save just to see how something looks. (#292)
- **[Bug]** **Making sure saved offer settings reach the live page** — Fixing cases where certain offer options were saved but never actually applied to what visitors see. (#295)
- **[Feature]** **Automatic performance projection for new offers** — An exploration into estimating how a new offer is likely to perform based on historical data, as a replacement for the current manual gut-check review. (#322)
- **[Task]** **Applying visitor targeting to auto-register offers** — Ensuring auto-register offers respect age, gender, state, zip, and device targeting instead of firing for everyone, including visitors they should exclude. This is a high-priority fix. (#333)

## Behind the Scenes

- **[Task]** **A safe, read-only testing environment** — Setting up a staging area that uses production-like data so features can be verified without any risk of changing real data. (#270)
- **[Feature]** **A Slack helper that turns conversations into tracked tasks** — Behind-the-scenes tooling to capture action items from Slack discussions and file them automatically, cutting out manual copy-and-paste. (#272)

## Campaigns

- **[Feature]** **Adding the Campaigns module** — Bringing campaign and offer-group management into the new platform so you can create, edit, and configure campaigns just like the legacy admin. This is a high-priority gap. (#200)

## Placements

- **[Feature]** **Bringing back the banner placement type** — Confirming whether banner placements are still in use and, if so, adding support for them in the new platform. (#326)

## Modals

- **[Feature]** **Making the Modal Design tab work — or removing it** — The six design fields on the Modal tab currently have no effect on what visitors see. They'll either be wired up to the visitor modal or removed to avoid confusion. (#294)

## Data Clients

- **[Feature]** **Restoring after-conversion delivery steps** — Porting the legacy post-conversion redirect and delivery behaviors for specific clients so they continue to work in the new platform. (#327)

## Pre-Pings

- **[Feature]** **Restoring the legacy per-client pre-ping** — Bringing over the older file-based pre-ping so any offer that still relies on it keeps working. This is a high-priority gap. (#330)

## Flows

- **[Task]** **Fixing the styling on the Flow form** — Correcting unstyled areas and misaligned fields so the Flow form looks clean and consistent with other forms in the app. (#152)

## Dashboard & Reports

- **[Task]** **Investigating mismatched report numbers** — Looking into why some dashboard report figures don't match the legacy system, so the data can be confirmed accurate or corrected. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 0f0dc75345ae083c3f2607503afd91bf3b9663925bf97592fab1f9e589c4ec62 -->
