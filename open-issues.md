# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 11:30:22 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview shows your unsaved edits** — When you edit an offer or placement, the Preview button will reflect the changes you're currently making instead of only the last saved version, so you can check your work before committing it. (#292)
- **[Bug]** **Some offer settings weren't reaching the live experience** — A number of saved offer options (including several modal fields, Display URL, and certain delivery flags) were being dropped before they reached visitors. This fix ensures configured options actually take effect, or removes options that were never used. (#295)
- **[Bug]** **Success pixels now fire as configured** — A formatting mismatch meant conversion/success pixels set up by admins were silently never firing, losing tracking data. This high-priority fix makes configured success pixels fire reliably. (#297)
- **[Feature]** **Automated performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform, based on your own historical offer data, replacing the informal manual gut-check with a data-driven decision aid. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently ignore age, gender, state, zip, and device targeting, so they can fire for people they should exclude. This work makes them honor the same targeting rules as regular offers (a high-priority fix). (#333)

## General / Across the App

- **[Bug]** **Clear error when testing an invalid link** — Testing an invalid link currently dumps you back on the dashboard with no explanation. Soon you'll see a clear failure message right in the Link Testing screen. (#239)
- **[Feature]** **Protection against two people editing the same record** — A new editing lock will warn you when someone else already has a record open, and prevent one person's save from quietly overwriting another's changes across all entity screens. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when — across offers, placements, advertisers, and more — including automated changes, so you can always answer "who changed this?" (#276)
- **[Feature]** **Cleaning up controls that don't do anything** — Several admin settings (like the Advertiser Web Presence fields, some user permission toggles, and a few data-client and pre-ping options) currently save but have no effect. These will be removed or hidden so the screens only show controls that actually work. (#296)

## Surveys

- **[Feature]** **Design settings that actually change the survey** — A full review to make sure every option on the Design tab is reflected in the live survey view, with no settings that appear to do something but don't. (#288)
- **[Feature]** **Finishing the Placement design settings** — Several Placement design options (like survey height and display format) are saved but not yet applied to the live survey widget. This work wires them through or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restoring after-success delivery behavior** — Post-conversion delivery and redirect steps from the previous system are being brought over to New Adsmith Frontend so affected clients keep working as before. (#327)
- **[Feature]** **Restoring custom pre-ping checks for data clients** — Hundreds of data clients relied on custom serve-time validation from the old system that isn't running yet. This high-priority work brings those checks over so leads are validated as intended. (#338)

## Admin & Users

- **[Task]** **Users screen review against the old system** — A documentation review comparing the new Users area to the previous version to spot missing features (like bulk role changes and last-login info) and prioritize what to add. (#80)
- **[Task]** **Decide the future of the file-share page** — The old file-share page has no equivalent yet. This is a keep-or-retire decision to confirm whether anyone still needs it. (#328)

## Behind the Scenes

- **[Task]** **A safe, read-only testing environment** — Setting up a practice environment loaded with production-like data where changes can't accidentally be saved, so the team can verify the product against realistic data. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — A helper that reads team chat and files the resulting to-dos as tracked items automatically, reducing manual copy-and-paste. (#272)

## Modals

- **[Feature]** **Making the Modal Design tab do something** — The Modal Design tab's settings (header text, colors, progress bar) currently save but never appear to visitors. This work either brings them to life in the visitor modal or removes them. (#294)

## Campaigns

- **[Feature]** **Bringing back the Campaigns module** — The Campaigns feature from the previous admin system isn't available yet in New Adsmith Frontend. This high-priority work restores the ability to view, create, edit, and configure campaigns and their offer groups. (#200)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned compared to other forms. This work polishes the layout — such as side-by-side paired fields and properly styled text boxes and color pickers — with care not to disturb the rest of the form. (#152)

## Dashboard

- **[Task]** **Confirming dashboard numbers match the old system** — During testing, some dashboard report figures didn't line up with the previous system. This investigation pins down where any differences come from and confirms the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
