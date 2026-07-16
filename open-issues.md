# Open Issues — Plain-Language Overview

_Last updated 2026-07-16 15:31:53 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on placements and offers** — When editing a placement or offer, the Preview button will show your in-progress changes exactly as they'll appear, so you no longer have to save first just to see how an edit looks. (#292)
- **[Bug]** **Conversion tracking on offers not firing** — High priority. Success pixels set up on offers currently don't fire, meaning some conversions go unrecorded. This fix ensures configured success pixels reliably fire, protecting your attribution and revenue tracking. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several offer options you can set (including modal-tab fields, display URL, and certain delivery flags) are saved but never actually applied to what visitors see. This work makes sure each option either takes effect or is cleaned up so nothing misleads you. (#295)
- **[Task]** **Auto-register offers should respect visitor targeting** — High priority. Auto-register offers currently ignore age, gender, state, zip, and device targeting, so they can fire for visitors who should be excluded. This fixes them to honor the same targeting rules as regular offers. (#333)
- **[Feature]** **Automatic performance projection for new offers** — Explores a tool that estimates how a new offer is likely to perform based on your historical offer data, giving a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Admin & Users

- **[Feature]** **Remove admin controls that don't do anything** — Some settings across Advertisers (Web Presence), user permissions, Data Clients, and Pre-Ping currently save but have no effect. Hiding or removing them prevents confusion and false expectations about what's actually being applied. (#296)
- **[Task]** **Review of the Users area against the old system** — A behind-the-scenes comparison of the new Users management screens versus the legacy version, so we know which capabilities (like bulk actions and login/2FA details) still need to be brought over. (#80)

## Surveys

- **[Feature]** **Make sure every design option actually shows up** — A thorough check across all entities to confirm that every customization option in the Design tab is fully connected to what visitors see, with any dead options fixed or removed. (#288)
- **[Feature]** **Connect remaining placement design settings to the live survey** — A handful of placement Design-tab settings (like survey height and display format) aren't yet reflected in the survey widget. This finishes wiring them up or removes ones that aren't needed. (#293)

## Data Clients

- **[Feature]** **Port after-success delivery behavior from the old system** — High priority. Post-conversion delivery and redirect steps that certain clients relied on in the legacy system are being brought over to the new platform so those clients keep working as expected. (#327)
- **[Feature]** **Bring over legacy pre-ping validation for data clients** — High priority. Custom serve-time validation rules used by hundreds of data clients in the old system don't yet run here. This restores that per-client validation so leads are checked as they were before. (#338)

## Reports & Dashboard

- **[Task]** **Investigate mismatched dashboard report numbers** — Reviewers noticed Dashboard report figures didn't match the legacy system. This work compares the two over a fixed date range to find the cause and confirm the numbers can be trusted. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — Every field on the Modal Design tab currently saves but has no effect on what visitors see. This either connects those header and progress-bar options to the live modal or removes the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form look unstyled or misaligned, with fields stacking oddly and inputs using plain browser defaults. This cleans up the layout to match the polished look of other forms. (#152)

## Behind the Scenes

- **[Task]** **Set up a read-only staging environment** — Internal maintenance to run the app against a copy of live data for safe testing, with no ability to change real records. No visible change for users. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — An internal tool that captures action items from team chats and files them automatically, streamlining how requests get logged. No direct effect on the product screens. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->
