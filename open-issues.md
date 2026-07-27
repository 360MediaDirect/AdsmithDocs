# Open Issues — Plain-Language Overview

_Last updated 2026-07-27 07:03:42 UTC · 14 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Feature]** **Preview shows your unsaved changes** — When you use Preview on a placement or offer while editing, you'll see exactly how your in-progress edits look, without having to save first. (#292)
- **[Bug]** **Some offer settings not reaching live pages** — Several saved offer options (including modal fields, display URL, and certain delivery flags) currently don't carry through to what visitors actually see. This fix makes sure each saved option either works end-to-end or is cleaned up so nothing is misleading. (#295)
- **[Feature]** **Automatic performance estimate for new offers** — Instead of relying on a manual gut-check, new offers will get a data-driven projection of how they're likely to perform, based on your own historical offer results. A helpful decision aid at intake time. (#322)

## Surveys
- **[Feature]** **Design choices show up in the live survey** — Every customization you set on the Design tab will actually appear in the survey visitors see. Part of a wider review to make sure no form option is left doing nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings** — Placement Design-tab options like display format and height, plus a few others, will be fully applied to the live survey (or removed if not needed), so what you configure is what visitors get. (#293)

## Data Clients
- **[Feature]** **Restore post-conversion delivery steps** — The follow-up actions that run after a successful conversion (delivery and redirect behavior) are being brought over to New Adsmith Frontend so those clients keep working as before. Nearly complete. (#327)
- **[Feature]** **Restore custom pre-check validation** — A high-priority effort to bring over the custom serve-time checks used by hundreds of data clients, so leads are validated the same way they were in the old system. (#338)

## General / Across the App
- **[Feature]** **Remove buttons and options that do nothing** — Certain admin controls (Advertiser web-presence fields, some user permission toggles, and a few data-client and pre-ping options) currently save but have no effect. These will be removed or hidden so the screens only show settings that truly work. (#296)
- **[Task]** **Users area feature review** — A documentation review comparing the old Users management screens to the new ones, so any missing capabilities (like bulk actions or extra columns) are identified and prioritized. (#80)

## Behind the Scenes
- **[Task]** **Safe practice environment for testing** — A separate, look-but-don't-touch copy of the app running against realistic data, so the team can verify things against production-like numbers without any risk of changing live data. (#270)
- **[Feature]** **Automatic issue capture from team chats** — A helper that reads designated chat conversations and turns action items into tracked tasks automatically, reducing manual copy-and-paste and duplicate entries. (#272)

## Modals
- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design tab's header and progress-bar settings currently have no effect on the modal visitors see. This work will either make those settings apply or remove the tab so it isn't misleading. (#294)

## Flows
- **[Task]** **Tidy up the Flow form's appearance** — Some parts of the Flow form look unstyled or stack awkwardly instead of sitting side-by-side. This cleanup brings its look in line with the Placement and Modal forms. Partly done, with the rest being handled carefully to avoid disrupting other tabs. (#152)

## Dashboard
- **[Task]** **Confirm dashboard numbers match the old system** — An investigation into why some Dashboard report figures didn't line up with the legacy system, to pin down the cause and confirm the new numbers are accurate. (#271)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
