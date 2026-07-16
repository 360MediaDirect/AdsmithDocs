# Open Issues — Plain-Language Overview

_Last updated 2026-07-16 13:32:40 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Placements & Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers to fire when a lead succeeds have been silently doing nothing, meaning conversions weren't being tracked. This high-priority fix makes those pixels fire reliably so your attribution and revenue reporting stay accurate. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of options you can set on an offer (including several Modal-tab settings, Display URL, and various delivery flags) were being saved but not actually applied where visitors see them. Once fixed, the settings you configure will take effect as expected — or be removed if they're not meant to do anything. (#295)
- **[Bug]** **Auto-register offers ignore visitor targeting rules** — Auto-register offers have been firing for every visitor, even when age, gender, state, ZIP, or device targeting should have excluded them. This high-priority fix makes them honor the same targeting rules as regular offers so leads only fire for the right audiences. (#333)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — Today the Preview button shows the last saved version, so you have to save before you can see edits. Soon Preview will reflect your current, unsaved changes so you can check your work without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature that would estimate how a new offer is likely to perform based on your historical offer data, replacing the informal manual gut-check review. It would give the team a quick, data-grounded read on expected performance at intake. (#322)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When two users open the same record, one could unknowingly save over the other's changes. This adds an editing lock and a warning so you'll see "Locked by [name]" when someone else is editing, and you'll be prompted to reload if a record changed while you had it open — preventing lost work across all entity screens. (#267)
- **[Feature]** **Cleaning up controls that don't actually do anything** — Several admin settings currently save but have no effect (the Advertiser Web Presence tab, some user permission toggles, and a few Data Client and Pre-Ping options). These will be removed or hidden so the screens only show controls that genuinely work, avoiding confusion. (#296)
- **[Task]** **Users screen review against the old system** — A detailed comparison of the Users area in New Adsmith Frontend versus the legacy system, identifying which features still need to be brought over (like bulk actions and additional columns). This guides what's added next so the Users area reaches full capability. (#80)
- **[Bug]** **Testing an invalid link now shows a clear error** — Entering an invalid link in Link Testing currently dumps you back on the Dashboard with no explanation. After this fix you'll see a proper failure message so you know the link didn't pass. (#239)
- **[Task]** **Decision on the old file-share page** — The legacy file-share page has no equivalent yet. This is a quick keep-or-retire decision to confirm whether anyone still needs it before either adding it or officially dropping it. (#328)

## Surveys

- **[Feature]** **Design tab settings will fully carry through to the live survey** — A review to make sure every customization option on the Design tab actually shows up in the survey visitors see, across all entities, with any settings that don't connect either fixed or removed. The result is that what you configure is what visitors get. (#288)
- **[Feature]** **Finishing the Placement Design-tab settings** — A few Placement Design settings (like iFrame height and display format) are saved but not yet applied to the live widget. This completes the wiring so those settings take effect, and cleans up any that won't be used. (#293)

## Data Clients

- **[Feature]** **Bringing back post-conversion delivery behavior** — The old system's after-success scripts (which run after a lead converts) haven't been carried over yet. This restores that behavior in a flexible, configurable way so active data clients keep working as they did before. (#327)
- **[Feature]** **Restoring custom pre-ping checks for data clients** — Hundreds of data clients relied on custom validation that ran before a lead was served in the old system, and that logic isn't running on the new platform yet. This high-priority effort ports those checks so lead qualification behaves as expected for the affected clients. (#338)

## Modals

- **[Feature]** **Making the Modal Design tab work — or removing it** — Every field on the Modal Design tab currently saves but has no effect on the modal visitors see. This will either wire those fields up so they actually change the modal's header and progress bar, or remove the tab if it's not needed. (#294)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with some fields stacking vertically instead of sitting side by side. This is a careful cleanup to make the Flow form look consistent with the Placement and Modal forms. (#152)

## Dashboard

- **[Task]** **Confirming Dashboard report numbers match the old system** — During testing, some Dashboard report figures didn't line up with the legacy system. This investigation compares the two over a fixed date range to find any differences, explain them, and confirm the numbers can be trusted. (#271)

## Behind the Scenes

- **[Task]** **Staging environment for safe testing** — Setting up a read-only test environment using a copy of real data, so the team can validate the product against realistic information without any risk of changing live records. (#270)
- **[Feature]** **Automated issue creation from team conversations** — An internal helper that turns action items from team chats into tracked work items automatically, reducing manual copy-and-paste and helping nothing slip through the cracks. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d541cdec2d7ef7e80b16585fe689f12231c8b31406080f26d5421cd3a156890a -->
