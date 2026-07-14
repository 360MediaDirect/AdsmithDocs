# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 15:30:12 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against two people overwriting the same record** — When you open any record to edit it (offers, flows, placements, advertisers, and more), the system will warn you if someone else is already editing it or has changed it since you opened it, so no one's work gets silently wiped out. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will get an Audit Log that records who changed what and when, across both manual edits and automated updates, making it easy to answer "who changed this and why." (#276)
- **[Feature]** **Cleaning up controls that don't actually do anything** — Several settings that currently save but have no effect (such as the Advertiser Web Presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping options) will be removed or hidden so the screens only show controls that work. (#296)
- **[Task]** **Users screen catch-up review** — A review comparing the older Users area to the new one, so any missing options (like bulk role changes, last-login info, and password/notification fields) can be prioritized and added. (#80)
- **[Task]** **Decision on the old File Share page** — The legacy file-sharing page has no equivalent yet; this reviews whether anyone still needs it so it's either rebuilt or officially retired. (#328)
- **[Bug]** **Invalid links should show a clear error** — When testing a link that isn't valid, you'll get a clear failure message instead of being unexpectedly sent to the dashboard. (#239)

## Offers

- **[Bug]** **Success tracking pixels weren't firing** — Conversion pixels set up on offers were silently never firing, meaning credit for successful leads was being lost. This fix makes configured success pixels fire reliably. (#297) — high priority
- **[Bug]** **Auto-register offers ignore visitor targeting** — Offers that fire automatically on page load are currently skipping age, gender, state, zip, and device targeting, so they can trigger for people they should exclude. This will bring them in line with your targeting rules. (#333) — high priority
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of offer options you can set (including modal fields, display URL, and several data-client flags) are being dropped before they reach visitors. Each will be either properly wired up or removed so what you set is what visitors get. (#295)
- **[Feature]** **Preview shows your unsaved changes** — On placement and offer edit screens, the Preview button will reflect the edits you've made but haven't saved yet, so you can check your work without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, replacing today's informal manual gut-check. (#322)

## Surveys

- **[Feature]** **Design tab options that actually take effect** — A thorough check to make sure every customization option on the design tab is reflected in the live survey, with a sweep across all entities to catch any settings that currently do nothing. (#288)
- **[Feature]** **Finishing the Placement design settings** — Several placement design options (such as survey height and display format) will be fully connected so they show up in the survey widget, and any leftover unused options will be either wired up or removed. (#293)

## Data Clients

- **[Feature]** **Restoring after-success delivery behavior** — Post-conversion delivery and redirect steps from the older system that weren't carried over will be rebuilt as a reusable option, so active clients keep working as before. (#327)
- **[Feature]** **Restoring custom pre-lead validation checks** — Custom serve-time validation used by hundreds of data clients wasn't carried over to the new platform. This work brings those checks back so leads are validated as they were before. (#338) — high priority

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging version of New Adsmith Frontend using a copy of real data, locked to read-only so testers can verify behavior against realistic data without changing anything. (#270)
- **[Feature]** **Slack helper for logging work items** — A Slack assistant that reads conversations and automatically turns action items into tracked issues, reducing manual copy-and-paste when capturing to-dos. (#272)

## Reports

- **[Task]** **Confirming report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy system, to pinpoint the cause and confirm the new numbers can be trusted. (#271)

## Modals

- **[Feature]** **Making the Modal Design tab work (or removing it)** — The Modal design settings currently save but don't change anything visitors see. Each field will be either connected to the visitor modal or removed so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned compared to other forms. This tidies up the layout so text boxes, color pickers, checkboxes, and paired fields display cleanly. (#152)

## Campaigns

- **[Feature]** **Bringing back the Campaigns area** — The Campaigns module from the older admin isn't in the new platform yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups, matching what you had before. (#200) — high priority

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
