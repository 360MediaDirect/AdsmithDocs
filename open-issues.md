# Open Issues — Plain-Language Overview

_Last updated 2026-07-10 11:00:58 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Feature]** **Preview edits before saving on placements and offers** — When you preview an offer or placement, you'll see your current, unsaved changes instead of the last-saved version, so you no longer have to save just to check how something looks. (#292)
- **[Bug]** **Saved offer settings not reaching the live page** — Several offer options you fill in (including Modal-tab fields, Display URL, and certain backend flags) currently never make it to the live experience. This fix ensures each saved setting is either used on the live page or removed if it does nothing. (#295)
- **[Bug]** **Success tracking pixels silently not firing** — Conversion pixels set up under "Pixels to Fire on Success" are not actually firing, meaning lost tracking with no warning. Once fixed, configured success pixels will reliably fire and be verified end-to-end. This is a high-priority fix. (#297)
- **[Feature]** **Automatic performance projection for new offers** — Instead of relying on a manual gut-check review, you'll be able to get a data-driven estimate of how a new offer is likely to perform, based on your own historical offer results. An exploratory improvement to help decisions at offer intake. (#322)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for everyone, even visitors who should be excluded by age, gender, state, zip, or device. This high-priority fix will make them respect the same targeting rules as regular offers (or clearly document any intended difference). (#333)
- **[Bug]** **bPerx voucher code missing from offer preview** — The bPerx voucher code line isn't showing on offer previews (and likely the live survey) in the test environment. This fix tracks down why the code lookup fails so the voucher displays correctly again. (#344)

## Admin & Users
- **[Task]** **Users area — comparison with the older system** — A review comparing the Users screens against the legacy system to spot missing pieces (like bulk role changes, select-all, last-login, and two-factor status) so the new Users area can reach full parity. Ongoing documentation and planning work. (#80)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record for editing, others will see it's locked and by whom, and you'll be warned if a record changed while you had it open — so no one accidentally wipes out another person's changes. Applies across all editable screens. (#267)
- **[Feature]** **Remove settings that don't actually do anything** — Several admin controls (Advertiser Web Presence fields, certain user-permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no effect. They'll be removed or hidden so the screens only show controls that truly work. (#296)
- **[Task]** **Decide the fate of the old file-share page** — The legacy file-share page has no equivalent in New Adsmith Frontend. This is a keep-or-retire decision to confirm whether anyone still needs it. (#328)

## Surveys
- **[Feature]** **Design-tab settings that fully take effect** — A thorough check to make sure every customization option on the Design tab (and other entity forms) actually changes what visitors see on the survey, with no "dead" settings that quietly do nothing. (#288)
- **[Bug]** **Voucher code and info links missing on live surveys** — For affected clients, the voucher code line and the privacy/terms/details links are set up in admin but not showing on the live survey page. This high-priority fix restores them to match the legacy display. (#291)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A handful of Placement Design-tab settings (like survey height and display format) are saved but not yet applied to the live widget. Each will be either fully wired up or removed from the form. (#293)

## Pre-Pings
- **[Feature]** **Run display-trigger checks at the right moment** — Certain pre-ping checks that should run (and hide an offer if rejected) when a page loads currently only do a light check. This high-priority fix makes them perform the full check like the legacy system, so unqualified offers are properly hidden. (#337)
- **[Feature]** **Bring legacy per-client pre-ping checks to the new platform** — Hundreds of data clients rely on custom pre-ping validation that isn't yet running in New Adsmith Frontend. This work ports those checks so each client's serve-time validation works as it did before. A high-priority parity effort. (#338)

## General / Across the App
- **[Bug]** **Clear error when testing a bad link** — Testing an invalid link currently dumps you on the dashboard instead of telling you the link failed. After this fix you'll get a clear error message in the Link Testing screen. (#239)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when across the platform — for both people and automated processes — so administrators can look up the full history of any record and troubleshoot changes with confidence. (#276)

## Behind the Scenes
- **[Task]** **Safe, read-only test environment** — Setting up a staging copy of the app against prod-like data for verification and testing, locked to read-only so nothing can be accidentally changed. Behind-the-scenes maintenance. (#270)
- **[Feature]** **Automatic issue creation from Slack conversations** — A helper that reads designated Slack conversations, pulls out action items, and files them as tracked tasks automatically — reducing manual note-taking. Internal tooling. (#272)

## Reports
- **[Task]** **Make sure report numbers match the legacy system** — An investigation into why some dashboard report figures differ from the old system, to pinpoint the cause and either fix it or confirm the numbers are correct. (#271)

## Placements
- **[Feature]** **Historical placement reports show offer impressions** — Offer impressions currently read as zero in historical placement reports. This improvement populates that figure so past reports show accurate offer-impression counts. (#339)

## Modals
- **[Feature]** **Make the Modal Design tab actually work** — All six fields on the Modal Design tab are saved but never shown to visitors. They'll either be wired up to display in the modal or removed from the form so the tab reflects reality. (#294)

## Flows
- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with some paired fields stacking awkwardly instead of sitting side by side. This cleanup brings the form in line with the polished look of the Placement and Modal forms. (#152)

## Campaigns
- **[Feature]** **Bring back the Campaigns area** — The Campaigns module from the legacy admin isn't yet available in New Adsmith Frontend. This high-priority work adds it back so you can view, create, edit, and configure campaigns and offer groups. (#200)

## Data Clients
- **[Feature]** **Restore post-conversion delivery behaviors** — The legacy "after-success" client actions (delivery and redirect steps that run after a conversion) weren't carried over. This work ports them so affected clients behave as they did before. (#327)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 20c05265760e30b087db164aa9ffb7701fea9cb19d23bb2497ef9c503a36041b -->
