# Open Issues — Plain-Language Overview

_Last updated 2026-07-12 09:33:52 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record at once, New Adsmith Frontend will show who's already editing it and prevent one person's save from silently wiping out the other's changes. This works across offers, flows, placements, advertisers, and other entity screens. (#267)
- **[Feature]** **Searchable activity history (Audit Log)** — A new admin Audit Log will record every change — who made it, what changed, and when — including automated system changes, so you can finally answer "who changed this and when?" and view a record's history right from its detail page. (#276)
- **[Task]** **Users management catch-up review** — A side-by-side review of the older Users area versus the new one, to plan the still-missing pieces (like bulk role changes, last-login and two-factor status columns, and a password field when adding a user). (#80)
- **[Feature]** **Removing settings that don't actually do anything** — Several controls currently save but have no effect (for example the Advertiser "Web Presence" fields, some user-permission toggles, and a few Data Client and Pre-Ping options). These will be removed or properly wired up so screens don't imply features that aren't there. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Testing an invalid link will now show a proper error message in the Link Testing area instead of quietly bouncing you back to the Dashboard. (#239)
- **[Task]** **Decision on the old File Share page** — Confirming whether the legacy File Share page is still used before either rebuilding it in the new admin or retiring it for good. (#328)

## Offers

- **[Bug]** **Conversion tracking pixels now fire on success (high priority)** — Success pixels configured on offers currently never fire, meaning conversions go untracked with no visible sign of a problem. This fix makes configured success pixels fire reliably again. (#297)
- **[Bug]** **Saved offer options will reach the live experience** — Some options you set on an offer (including several Modal-tab fields and Display URL) aren't currently making it through to what visitors see. Each will be either delivered properly or cleaned up if it's not needed. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting and can fire for visitors who should be excluded. This aligns them with how regular offers are targeted. (#333)
- **[Feature]** **Preview your unsaved changes** — The Preview button on Placement and Offer edit screens will show your current in-progress edits, so you no longer have to save first just to see what a change looks like. (#292)
- **[Feature]** **Automated performance estimates for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, replacing the informal manual gut-check review. (#322)

## Surveys

- **[Feature]** **Design-tab settings that actually show in the survey** — Ensuring every customization option on the design tab is reflected in the live survey view, plus a full check across all entities so no setting is left disconnected. (#288)
- **[Feature]** **Finishing Placement design-tab settings** — Wiring up the remaining Placement design settings (like iFrame height and display format) so they take effect in the survey widget, and cleaning up any that won't be used. (#293)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery behavior** — The older "after success" delivery/redirect handling used by active data clients will be rebuilt in New Adsmith Frontend so those clients keep working as before. (#327)
- **[Feature]** **Restoring custom pre-ping checks (high priority)** — Hundreds of data clients rely on custom serve-time validation that currently doesn't run on the new platform. This work brings those checks back so those clients' visitor validation behaves correctly again. (#338)

## Modals

- **[Feature]** **Making the Modal Design tab do something** — The Modal Design tab (header title, colors, progress bar, and more) currently saves but has no effect on the visitor modal. These fields will either be built into the modal or removed so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Cleaning up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned (plain text boxes, unpolished color pickers, fields stacking instead of sitting side by side). This is a careful visual pass to match the polish of the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bringing the Campaigns module to the new platform** — A core Campaigns area is still missing in New Adsmith Frontend. This adds the ability to view, create, edit, and configure campaigns and their offer groups, matching what's available today. (#200)

## Reports

- **[Task]** **Confirming Dashboard report numbers match the older system** — Investigating why some Dashboard report figures didn't line up with the previous system, pinpointing the cause, and either correcting it or confirming the numbers are consistent. (#271)

## Behind the Scenes

- **[Task]** **A read-only test environment against realistic data** — Standing up a safe, look-but-don't-touch environment using production-like data for verification and testing. (#270)
- **[Feature]** **Faster turning of conversations into tracked work** — An internal helper that reads team conversations and files or updates work items automatically, reducing manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
