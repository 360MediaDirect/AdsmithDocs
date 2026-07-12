# Open Issues — Plain-Language Overview

_Last updated 2026-07-12 23:18:06 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — High priority. Conversion pixels set up on offers are silently failing to fire, meaning successful conversions aren't being recorded. This fix restores accurate conversion tracking. (#297)
- **[Task]** **Auto-register offers will respect visitor targeting** — High priority. Auto-register offers currently fire for every visitor, ignoring age, gender, state, ZIP, and device targeting. This ensures they only show to the audience they're meant for. (#333)
- **[Bug]** **Saved offer settings will reach the live experience** — Several offer options you save (such as modal settings, display URL, and certain data-client flags) aren't currently carried through to what visitors see. Each will either take effect or be removed if unused. (#295)
- **[Feature]** **Preview will show your unsaved edits** — When previewing a placement or offer you're editing, you'll see your current, unsaved changes instead of the last saved version — no need to save first just to check your work. (#292)
- **[Feature]** **Automatic performance projections for new offers** — New offers will get a data-driven estimate of likely performance based on your historical offers, replacing the manual review step. (#322)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other** — When someone else already has a record open, you'll see a clear notice and be warned before your save could wipe out their changes. Works across all editable screens. (#267)
- **[Feature]** **A searchable activity history** — A new admin page will record who changed what and when across the platform, so you can trace any change back to the person or automated process that made it. (#276)
- **[Feature]** **Removing settings that don't actually do anything** — Some controls (Advertiser Web Presence fields, a couple of user permissions, and certain data-client and pre-ping options) currently have no effect. They'll be removed or hidden so screens only show settings that work. (#296)
- **[Task]** **Users screen compared against the old system** — A documentation review confirming the new Users area matches the legacy one, flagging gaps like bulk actions, last-login, and 2FA status so they can be planned. (#80)
- **[Task]** **Decision on the old file-share page** — Confirming whether the legacy file-share page is still used and either bringing it into the new admin or formally retiring it. (#328)

## Surveys

- **[Feature]** **Design options will truly change what visitors see** — A review across the product to make sure every customization option in a design tab is actually reflected in the live survey, with any dead options fixed or removed. (#288)
- **[Feature]** **Finishing the Placement design settings** — Settings like survey height and display format will properly take effect in the live survey once fully connected. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restoring custom pre-delivery checks** — High priority. Custom serve-time validation used by 448 clients in the old system isn't running on the new platform yet; this brings that logic back so those checks apply again. (#338)
- **[Feature]** **Restoring after-success delivery** — The post-conversion delivery and redirect behavior from the legacy system will be brought into the new platform for the clients that still rely on it. (#327)

## Dashboard

- **[Bug]** **Invalid link tests will show a clear error** — Testing an invalid link currently drops you on the dashboard with no explanation. It will instead return a clear failure message so you know the link didn't pass. (#239)
- **[Task]** **Investigating report numbers vs. the old system** — Some dashboard report figures didn't match the legacy app during testing. This investigation pins down why and confirms the numbers are accurate. (#271)

## Behind the Scenes

- **[Task]** **A safe testing environment against real-world data** — Setting up a read-only staging copy so the team can verify the product against production-like data without any risk of changing it. (#270)
- **[Feature]** **A helper that turns conversations into tracked tasks** — An internal tool to capture action items from team chats and file them automatically, reducing manual note-keeping. (#272)

## Campaigns

- **[Feature]** **Bringing the Campaigns module to the new platform** — High priority. Campaign management isn't available in the new platform yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups, matching the old system. (#200)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Some elements on the Flow form currently look unstyled or stack awkwardly instead of sitting side by side. This cleanup brings its look in line with the other forms. (#152)

## Modals

- **[Feature]** **Making the Modal Design tab work (or removing it)** — The modal's header and progress-bar design settings don't currently affect what visitors see. They'll either be connected so they take effect or removed to avoid confusion. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
