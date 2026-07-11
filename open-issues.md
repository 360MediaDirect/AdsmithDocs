# Open Issues — Plain-Language Overview

_Last updated 2026-07-11 19:25:22 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers & Placements
- **[Feature]** **Preview shows your unsaved changes** — When editing a placement or offer, the Preview button will reflect the edits you've made on screen, so you can check your work without having to save first. (#292)
- **[Bug]** **Some saved offer options never reach the live experience** — Several offer settings (including modal options, "Force More Info Visible," Display URL, and certain data-client flags) are saved but currently don't carry through to what visitors actually see. This fix ensures each setting either works or is cleanly removed. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels configured on offers are silently not firing, which means lost tracking. This fix makes sure a pixel you set up actually fires when a conversion happens. (#297)
- **[Task]** **Auto-register offers now respect visitor targeting** — Certain automatic offers currently show to everyone, ignoring age, gender, state, ZIP, and device targeting. This work makes them honor the same targeting rules as other offers so they only reach the intended audience. (#333)
- **[Feature]** **Automatic performance projections for new offers** — Instead of an informal manual gut-check, you'll be able to see a data-driven estimate of how a new offer is likely to perform, based on your own historical offer results. (#322)

## General / Across the App
- **[Feature]** **Protection against two people overwriting each other's edits** — When someone else is already editing a record, you'll see a clear "locked by" notice, and the system will warn you if a record changed while you had it open, so no one's work gets silently lost. (#267)
- **[Feature]** **A searchable activity history for everything** — A new Audit Log will record who changed what and when across the platform (both people and automated jobs), so you can easily answer "who changed this record and when." (#276)
- **[Feature]** **Cleaning up controls that don't do anything** — Some admin settings (such as certain Advertiser web-presence fields, user permission toggles, and a few Data-Client and Pre-Ping options) are saved but currently have no effect. These will be removed, hidden, or properly wired up so what you see is what you get. (#296)
- **[Task]** **Decision on the old file-share page** — The legacy file-share page has no equivalent yet. This is a quick review to decide whether it's still needed or can be retired. (#328)
- **[Bug]** **Invalid links should show a clear error** — When you test a link that isn't valid in Link Testing, you'll get a clear failure message instead of being unexpectedly sent to the dashboard. (#239)

## Surveys
- **[Feature]** **Design tab customizations fully reflected in the survey** — Every option on the survey Design tab will actually change what visitors see. This includes an app-wide check to make sure no customization option is left disconnected. (#288)
- **[Feature]** **Finishing the Placement Design tab settings** — A handful of Placement design options (such as survey height and display format) will be fully connected so they show up in the live survey widget, with any leftover unused options cleaned up. (#293)

## Data Clients & Pre-Pings
- **[Feature]** **Bringing back after-success delivery steps** — The post-conversion delivery and redirect behavior from the old system will be rebuilt on the new platform, so data clients that rely on it keep working. (#327)
- **[Feature]** **Restoring custom pre-ping checks for data clients** — Custom validation checks that ran for hundreds of data clients in the old system aren't yet active on the new platform. This work restores those checks so leads are validated as intended. (#338)

## Modals
- **[Feature]** **Making the Modal Design tab actually work** — The Modal Design tab settings (header title, subtitle, colors, progress bar) currently have no effect on the visitor-facing modal. These will either be connected so they display properly, or removed if the modal is intentionally header-less. (#294)

## Flows
- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly instead of sitting side by side. This cleanup brings the Flow form's appearance in line with the Placement and Modal forms. (#152)

## Campaigns
- **[Feature]** **Bringing the Campaigns module to the new platform** — Campaign management doesn't exist yet in New Adsmith Frontend. This high-priority work adds the ability to view, create, edit, and configure campaigns and offer groups, matching what the old admin could do. (#200)

## Reports & Dashboard
- **[Task]** **Making sure report numbers match the old system** — Some dashboard report figures didn't line up with the legacy system during testing. This investigation finds where the difference comes from and confirms the numbers can be trusted. (#271)

## Admin & Users
- **[Task]** **Reviewing what's missing from the Users area** — A detailed comparison of the old Users management against the new one, so we know which features (like bulk actions, last-login, and password options) still need to be added. (#80)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging version of the product using production-like data for testing and verification, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Automating issue tracking from team chats** — A helper tool that turns action items from team conversations into tracked work items automatically, reducing manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
