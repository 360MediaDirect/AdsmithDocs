# Open Issues — Plain-Language Overview

_Last updated 2026-07-13 20:26:37 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on an offer's "success" step currently don't fire at all, which means completed conversions may not be reported to partners. This fix makes those pixels fire reliably so attribution isn't lost. (#297)
- **[Task]** **Auto-register offers will respect visitor targeting** — Some auto-register offers currently fire for every visitor, ignoring age, gender, state, ZIP, and device targeting. This work makes them follow the same targeting rules as regular offers so they only show to the right people. (#333)
- **[Bug]** **Offer settings that never reach the live experience** — Several saved offer options aren't actually being carried through to what visitors see. This cleans that up so every setting either works as expected or is clearly removed if it's no longer needed. (#295)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — Right now the Preview button shows the last saved version, so you have to save before you can check an edit. This lets Preview reflect your current, unsaved changes on both Placement and Offer edit screens. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check review, this explores estimating how a new offer is likely to perform based on your own historical offer data. It's aimed at giving you a helpful projection right at intake. (#322)

## General / Across the App

- **[Feature]** **Warning when two people edit the same record** — If a colleague opens the same offer, flow, placement, or other record while you have it open, you'll see a clear notice instead of one person silently overwriting the other's changes. This protects your edits across every entity screen. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when, across offers, placements, and other entities, including automated changes. You'll be able to search this history and see a record's changes right from its detail page. (#276)
- **[Feature]** **Removing controls that don't do anything** — Some settings (like the Advertiser Web Presence fields, certain user permission toggles, and a few Data Client and Pre-Ping options) are saved but have no effect. These will be hidden or removed so the screens only show controls that actually work. (#296)
- **[Task]** **Reviewing what the Users area still needs** — A detailed comparison of the old Users management against the new one, so we know which features (like bulk actions or last-login info) still need to be brought over. This is a planning/documentation step. (#80)
- **[Bug]** **Clearer error when testing an invalid link** — Testing an invalid link currently dumps you back on the Dashboard with no explanation. This fix will show a clear failure message so you know the link didn't pass. (#239)
- **[Task]** **Decision on the legacy file-share page** — The old file-share page has no equivalent yet. This is a quick review to decide whether it's still needed or can be retired. (#328)

## Surveys

- **[Feature]** **Design settings that actually show up in the survey** — Every option on the Design tab should be reflected in what visitors see. This work checks each customization across all entities and makes sure none of them are dead ends. (#288)
- **[Feature]** **Finishing the Placement Design tab settings** — A handful of Placement design options (like iFrame height and display format) are saved but not yet applied to the live survey widget. This wires the remaining ones through, or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Bringing over after-success delivery behavior** — Certain post-conversion delivery and redirect behaviors from the old system weren't carried over yet. This adds them back as a flexible, configurable option so those clients keep working as before. (#327)
- **[Feature]** **Restoring file-based pre-ping checks** — Hundreds of data clients rely on custom pre-ping validation that isn't running on the new platform yet. This work brings that serve-time validation over so those checks behave the way they did in the legacy system. (#338)

## Behind the Scenes

- **[Task]** **A read-only staging environment for testing** — Setting up a test environment loaded with production-like data that can be used for verification without any risk of changing real records. (#270)
- **[Feature]** **A Slack helper that turns discussions into tracked tasks** — An assistant that reads designated Slack conversations, pulls out action items, and files them as tracked issues automatically, cutting out manual copy-paste. (#272)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly and plain-looking text boxes and color pickers. This tidies up the appearance so it matches the polished look of the Placement and Modal forms. (#152)

## Modals

- **[Feature]** **Making the Modal Design tab do something** — The entire Modal Design tab (headers, colors, progress bar) is saved but never actually shown to visitors. This will either wire those settings into the visitor-facing modal or remove the tab if it isn't needed. (#294)

## Campaigns

- **[Feature]** **Bringing the Campaigns module to the new platform** — Campaign management, including offer groups and offer selection, doesn't exist in the new platform yet. This high-priority work adds the ability to view, create, edit, and configure campaigns just like the legacy system. (#200)

## Reports

- **[Task]** **Confirming report numbers match the legacy system** — During testing, some Dashboard report figures didn't line up with the old system. This investigation compares the two over a fixed period, pinpoints where any differences come from, and confirms the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
