# Open Issues — Plain-Language Overview

_Last updated 2026-07-13 18:33:02 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Bring the Campaigns area into New Adsmith Frontend** — Campaign management from the old system isn't in the new platform yet. Once added, you'll be able to view, create, and edit campaigns and manage offer groups and their offers, just like before. (#200)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit, others will see it's being worked on, and you'll be warned if someone changed it while you had it open — so no one's changes get silently lost. (#267)
- **[Feature]** **A searchable history of who changed what** — A new activity log will record every change to records (and automatic system changes) with the person, time, and what changed, viewable per record and searchable across the app. Great for answering "who changed this and when?" (#276)
- **[Feature]** **Clean up settings that don't actually do anything** — Several controls (Advertiser Web Presence fields, some user permission toggles, and a few Data Client and Pre-Ping options) currently save but have no effect. These will be removed or hidden so screens only show settings that truly work. (#296)
- **[Task]** **Restore missing options on the Users screen** — A review compared the old Users area with the new one to find features that haven't been carried over yet (like bulk role changes, 2FA status, and last-login info) so they can be prioritized and added back. (#80)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-sharing page has no equivalent yet. This confirms whether anyone still needs it and either finds it a home in the new admin or retires it cleanly. (#328)

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers currently never fire, which means lost tracking. This fix makes configured success pixels fire reliably. (High priority.) (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of offer options you can set (including Modal-tab fields, Display URL, and several data-client flags) are being dropped before they reach visitors. Each will be wired through properly or removed if not needed. (#295)
- **[Task]** **Make auto-register offers respect targeting rules** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting, so they can fire for visitors who should be excluded. This will bring them in line with regular offers (or confirm the difference is intentional). (High priority.) (#333)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — The Preview button will show the edits you're currently making, not just the last saved version, so you can check your work before saving. (#292)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool to estimate a new offer's likely performance based on your historical offer data, replacing an informal manual review with a data-driven projection at intake. (#322)

## Surveys

- **[Feature]** **Make every survey Design setting actually take effect** — A full check to ensure all Design-tab customizations show up in the live survey, with any options that aren't connected either wired up or removed. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey** — Several Placement Design-tab settings (like iFrame Height and Display Format) don't yet affect the live widget. Each will be made to work or removed from the form. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior for clients** — After-success delivery/redirect steps from the old system haven't been carried over. All required behaviors will be reintroduced as a configurable option so affected clients work as before. (#327)
- **[Feature]** **Bring back custom pre-ping checks for data clients** — Hundreds of data clients rely on custom serve-time validation that isn't running on the new platform. This ports that logic so those checks run again and correctly pass or reject. (High priority.) (#338)

## Reports & Dashboard

- **[Task]** **Confirm dashboard numbers match the old system** — Reviewers noticed report figures differing from the legacy app. This investigation compares the two over a fixed period, pinpoints any differences, and confirms the numbers can be trusted. (#271)
- **[Bug]** **Show a clear error for invalid link tests** — Testing an invalid link currently sends you to the dashboard with no explanation. Instead, you'll see a clear failure message. (#239)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — All six Modal Design fields currently save but don't change anything visitors see. They'll either be built into the visitor modal or removed from the form. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacking instead of sitting side by side). This tidies up the layout to match other forms. (#152)

## Behind the Scenes

- **[Task]** **Set up a read-only test environment** — A staging setup using production-like data for safe verification and testing, with saving disabled so nothing can be accidentally changed. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads designated chat channels and files new work items automatically, reducing manual copy-and-paste from meetings. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
