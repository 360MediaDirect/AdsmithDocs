# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 21:20:52 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers currently never fire because of a format mismatch, which means successful leads aren't being counted. This fix makes configured success pixels fire reliably so you don't lose attribution or revenue signals. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several offer options you fill in (including offer-level modal fields, Display URL, and certain data-client flags) are being dropped before they reach visitors. This work makes each of those fields either take effect or be clearly retired, so what you save is what visitors get. (#295)
- **[Task]** **Auto-register offers now respect visitor targeting** — Auto-register offers have been firing for everyone, ignoring age, gender, state, ZIP, and device targeting. This ensures they only fire for the visitors they're meant for (or documents the difference on purpose). (#333)
- **[Feature]** **Preview unsaved changes on offers and placements** — Today the Preview button shows the last saved version, so you have to save before you can check an edit. Soon Preview will reflect your current, unsaved changes right away. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, new offers could be scored against your historical offer data to estimate likely performance. This is an exploratory tool to help judge new offers at intake. (#322)

## General / Across the App

- **[Feature]** **Protection against two people overwriting the same record** — When two admins edit the same offer, flow, placement, advertiser, or other record at once, one person's changes can silently wipe out the other's. This adds an editing lock and a warning so you'll see when someone else is already editing and won't lose work. (#267)
- **[Feature]** **A searchable history of who changed what** — There's currently no easy way to see who paused an offer, changed a cap, or edited a placement, and when. This adds an audit log across the app, plus a per-record history, so you can trace every manual and automated change. (#276)
- **[Feature]** **Cleaning up controls that don't actually do anything** — Some admin settings (an Advertiser "Web Presence" tab, a couple of user permission toggles, and a few Data-Client and Pre-Ping options) look active but currently have no effect. These will be removed or hidden so the screens only show controls that truly work. (#296)
- **[Task]** **Users screen catch-up with the old system** — A review of the older Users management against the new one to spot missing capabilities (like bulk role changes, last-login and two-factor status, and password/notification options on the add-user form). This guides bringing the new Users area up to par. (#80)
- **[Task]** **Decision on the old file-share page** — The previous system had a file-share page with no equivalent here yet. This confirms whether anyone still needs it or whether it can be retired. (#328)

## Surveys

- **[Feature]** **Design-tab options that actually show up in the survey** — An across-the-board check to make sure every look-and-feel option on the design tab genuinely changes what visitors see, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finishing the Placement design settings for the survey widget** — A handful of placement design settings (like iframe height and display format) are saved but not yet applied to the live survey. This wires them up so they take effect, or removes any that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restoring post-conversion delivery for data clients** — Certain after-success delivery and redirect behaviors from the old system weren't carried over yet. This brings them back in a flexible, settings-driven way so active data clients keep working as before. (#327)
- **[Feature]** **Restoring custom pre-ping checks for data clients** — Hundreds of data clients relied on custom serve-time validation checks that don't run on the new platform yet. This ports those checks so the right offers are shown or blocked as intended. (#338)

## Dashboard & Reports

- **[Task]** **Making the new reports match the old numbers** — During testing, dashboard report figures didn't line up with the previous system, which made verification hard. This investigation pins down why and confirms the numbers are accurate. (#271)
- **[Bug]** **Clear error for a bad test link** — Testing an invalid link currently dumps you back on the dashboard with no explanation. This fix shows a clear failure message so you know the link didn't work and why. (#239)

## Modals

- **[Feature]** **Making the Modal design settings count** — The entire Modal design tab is saved but never shown to visitors. This either wires those header and progress-bar settings into the visitor modal or removes the tab if the modal is meant to be header-less. (#294)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned, with fields stacking oddly and plain-looking text boxes and color pickers. This is a careful cleanup so the Flow form looks consistent with the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bringing the Campaigns area to the new platform** — Campaign management (creating and editing campaigns, offer groups, CTA text, offer handling, and more) isn't available in the new platform yet. This adds a Campaigns area matching what the old system offered. (#200)

## Behind the Scenes

- **[Task]** **A safe, read-only testing environment** — Setting up a testing copy of the app loaded with production-like data that can't be changed, so the team can verify behavior without any risk to live data. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — A helper that reads designated chat channels and files action items as tracked issues, cutting out manual copy-paste and reducing the chance things slip through. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
