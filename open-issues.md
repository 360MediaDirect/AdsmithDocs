# Open Issues — Plain-Language Overview

_Last updated 2026-07-12 13:30:34 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes before saving** — On the Offer and Placement edit screens, the Preview button will show exactly what you've changed on the form, even before you save, so you no longer have to save first just to check how an edit looks. (#292)
- **[Bug]** **Saved offer options not reaching the live experience** — Several offer settings you configure (including modal fields, "Force More Info Visible," Display URL, and certain data-client options) are being dropped before they reach visitors. This fix makes sure the options you set actually take effect, or removes ones that were never used. (#295)
- **[Bug]** **Success pixels aren't firing** — Conversion tracking pixels set up under "Pixels to Fire on Success" have been silently not firing, meaning lost tracking with no warning. This high-priority fix ensures configured success pixels actually fire. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for everyone, skipping the age, gender, state, ZIP, and device targeting rules that normal offers follow. This high-priority fix makes them respect your targeting so they only fire for the right visitors. (#333)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check review, new offers will get an automated estimate of likely performance based on your own historical offer data, helping you gauge a new offer at intake. (#322)

## General / Across the App

- **[Task]** **Bringing the Users area up to parity with the old system** — A review of the Users screen against the legacy version, so features you rely on (like bulk role changes, last-login info, and password setup when adding a user) can be added to the new experience. (#80)
- **[Feature]** **Warning when two people edit the same record** — Editing screens will show a clear "locked by someone else" notice and prevent one person's save from silently wiping out another's changes, protecting your work when teammates edit the same offer, flow, or other record. (#267)
- **[Feature]** **Searchable history of who changed what** — A new Audit Log will record every change to your records (manual or automatic) with who made it and when, so you can finally answer "who changed this and when?" from a searchable page and from each record's history. (#276)
- **[Feature]** **Removing controls that don't actually do anything** — Some settings (like the Advertiser Web Presence tab, certain user permission options, and a few data-client and pre-ping fields) are saved but have no effect. These misleading controls will be hidden or removed so the screens only show options that truly work. (#296)
- **[Bug]** **Invalid link test sends you to the Dashboard** — Testing an invalid link currently dumps you on the Dashboard with no explanation. This nearly-finished fix will show a clear error result instead. (#239)
- **[Task]** **Decision on the old file-share page** — The legacy file-share page has no equivalent yet; this is a check on whether anyone still needs it, so it's either rebuilt or officially retired. (#328)

## Surveys

- **[Feature]** **Design tab settings that actually show up** — A thorough check across all screens to make sure every option on the Design tab (and other form options) genuinely affects what visitors see, fixing or removing any that currently do nothing. (#288)
- **[Feature]** **Finishing the Placement survey design settings** — A handful of Placement Design tab settings (like survey height and display format) are saved but not yet applied to the live survey. This wires them through so your choices take effect, or clears out ones that won't be used. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restoring post-conversion delivery behavior** — Certain after-success delivery and redirect behaviors from the old system weren't carried over. This brings them back for the affected clients so post-conversion handoffs work as before. (#327)
- **[Feature]** **Restoring per-client pre-ping validation** — Hundreds of data clients relied on custom pre-ping checks that currently don't run on the new platform. This high-priority work rebuilds those checks so serve-time validation works as it did before. (#338)

## Modals

- **[Feature]** **Making the Modal Design tab work (or removing it)** — Every field on the Modal Design tab is currently saved but never shown to visitors. This will either make those header and progress-bar settings appear in the visitor modal or remove the tab if it's not needed. (#294)

## Flows

- **[Task]** **Fixing the appearance of the Flow form** — Parts of the Flow form look unstyled and misaligned compared to other screens. This cleanup brings its layout and styling in line with the rest of the app. (#152)

## Campaigns

- **[Feature]** **Bringing back the Campaigns module** — Campaign management from the old admin isn't available yet in New Adsmith Frontend. This high-priority work adds the ability to view, create, edit, and configure campaigns and offer groups, matching the legacy workflow. (#200)

## Behind the Scenes

- **[Task]** **A safe practice environment for testing** — Setting up a read-only version of the app loaded with production-like data, so testing and verification can happen without any risk of changing real records. (#270)
- **[Task]** **Checking that report numbers match the old system** — An investigation into why some Dashboard report figures didn't line up with the legacy system, to pinpoint any differences and confirm the numbers can be trusted. (#271)
- **[Feature]** **Turning conversations into tracked to-dos automatically** — A helper that reads team conversations and files the resulting action items automatically, reducing manual copy-paste when capturing new work. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
