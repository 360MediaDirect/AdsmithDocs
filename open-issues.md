# Open Issues — Plain-Language Overview

_Last updated 2026-07-09 11:01:13 UTC · 24 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Admin & General

- **[Feature]** **Protection against two people editing the same record at once** — When someone opens a record to edit it, others will see it's locked and by whom, and the app will warn you if a record changed since you opened it — so edits can no longer silently overwrite each other. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will let administrators see who changed what and when across offers, placements, advertisers, and more — including automated changes — making it easy to track down "who touched this record." (#276)
- **[Feature]** **Cleaning up controls that don't do anything** — Several admin settings that look active but currently have no effect (Advertiser Web Presence fields, some user permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden so the screens only show controls that truly work. (#296)
- **[Task]** **Users screen: comparing old vs. new** — A review of the older Users management screens against the new ones, so any missing capabilities (like bulk actions or extra columns) can be prioritized and added. A documentation/planning update. (#80)
- **[Task]** **Consistent alert and banner colors everywhere** — Warning, info, success, and error banners will look identical from page to page instead of drifting slightly in shade. A behind-the-scenes tidy-up with a small visible polish. (#341)
- **[Task]** **Decide the future of the old file-share page** — A quick review to confirm whether the legacy file-share page is still needed in the new platform or can be retired. (#328)

## Offers

- **[Feature]** **Bring back the Campaigns module** — Campaign management from the older admin (creating, editing, and organizing campaigns and offer groups) will be rebuilt in New Adsmith Frontend so this core workflow is available again. High priority. (#200)
- **[Feature]** **Preview your unsaved changes** — On placement and offer edit screens, the Preview button will show the changes you've made but not yet saved, so you no longer have to save first just to check how something looks. (#292)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, replacing the informal manual review that's being retired. (#322)
- **[Bug]** **Some saved offer settings weren't reaching the live page** — A number of saved offer options (including several modal fields and display settings) weren't making it through to what visitors see; each will be properly connected or removed if unused. (#295)
- **[Task]** **Auto-register offers now respect visitor targeting** — Fixing a case where auto-registering offers fired for everyone, ignoring age, gender, state, ZIP, and device targeting; once fixed they'll only fire for the visitors they're meant to. High priority. (#333)

## Surveys

- **[Feature]** **Design tab changes fully reflected in the survey** — A full check that every customization option on the design tab actually shows up in the live survey, with any disconnected options fixed so what you set is what visitors see. (#288)
- **[Feature]** **Finishing the placement design settings** — Several placement design options (such as survey height and display format) will be fully connected to the live survey, or removed if not needed, so no setting is left doing nothing. (#293)
- **[Bug]** **Voucher codes and info links missing on live surveys** — On some survey pages the voucher code line and the privacy/terms/details links weren't showing even though they were set up in the admin; this fixes the display so they appear as they did before. High priority. (#291)

## Pre-Pings

- **[Feature]** **Restore serve-time offer validation** — Offers set to check with the advertiser as they're displayed will again make that live check and hide the offer if it's rejected, matching the older system's behavior. High priority. (#337)
- **[Feature]** **Bring back per-client pre-ping checks** — Legacy custom validation used by hundreds of data clients will be ported to the new platform so those serve-time checks run again. High priority. (#338)

## Behind the Scenes

- **[Task]** **A safe staging environment for testing** — Setting up a look-but-don't-touch test environment loaded with production-like data, so changes can be verified without any risk of altering real records. (#270)
- **[Feature]** **Automatic issue-filing from Slack conversations** — A helper that reads designated Slack channels and turns action items into tracked tasks automatically, cutting out manual copy-paste. (#272)

## Data Clients

- **[Feature]** **Restore post-conversion delivery steps** — The older "after-success" behaviors that run once a lead converts (for clients like bPerx and RWDB) will be brought over to the new platform so they run as before. Nearly complete. (#327)

## Placements

- **[Feature]** **Fixing zero offer impressions in historical reports** — Offer impression numbers that were showing as 0 in older placement reports will be populated correctly, giving accurate historical figures. (#339)

## Modals

- **[Feature]** **Make the Modal Design tab actually work** — The modal design settings (header title, colors, progress bar, etc.) currently don't affect the visitor's modal; they'll either be connected so they take effect or removed if the modal is meant to be header-less. (#294)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned (plain text boxes, stacked fields, unstyled color pickers); this cleans up the layout to match the polished look of other forms. (#152)

## Dashboard & Reports

- **[Task]** **Confirming dashboard numbers match the old system** — An investigation into why some dashboard report figures didn't line up with the legacy system, to pinpoint the cause and confirm the numbers can be trusted. (#271)

## Link Testing

- **[Bug]** **Clear error when testing an invalid link** — Testing an invalid link currently dumps you back on the dashboard; instead you'll get a clear failure message so you know the link didn't work. Nearly complete. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: e97c0c87fd1c264309b547c86ecde9d1b7abd3cebd9c6dc642ac728d6283da48 -->
