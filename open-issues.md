# Open Issues — Plain-Language Overview

_Last updated 2026-07-13 22:18:37 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing on completed offers** — A high-priority fix so that the conversion tracking pixels admins set up on an offer actually fire when someone completes it, restoring lost attribution and revenue tracking. (#297)
- **[Task]** **Auto-register offers currently ignore audience targeting** — A high-priority fix so that "auto-register" offers respect the same age, gender, state, zip, and device targeting rules as regular offers, instead of showing up for visitors they should exclude. (#333)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several offer options you can fill in today (like Display URL and certain Modal and data-client settings) are being dropped before they reach the visitor-facing widget. This will make sure each saved setting either works or is cleanly removed. (#295)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — The Preview button will show the edits you're currently working on, so you no longer have to save first just to see what a change looks like. (#292)
- **[Feature]** **Automatic performance projection for new offers** — When a new offer comes in, you'll get a data-driven estimate of how it's likely to perform based on past offers, replacing today's manual gut-check review. (#322)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When someone opens a record for editing, others will see it's in use and be warned before their work can be accidentally overwritten, preventing silent lost changes across all entity screens. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will get an "Audit Log" that records who changed what and when across offers, placements, advertisers, and more, making it easy to answer "who changed this and when." (#276)
- **[Feature]** **Removing settings that don't actually do anything** — Certain controls that currently save but have no effect (such as an Advertiser's Web Presence fields and a few permission and data-client options) will be hidden or removed so the screens only show settings that genuinely work. (#296)
- **[Task]** **Comparing the old and new Users screens** — A documentation and review effort to catch any features from the old Users area (like bulk role changes, last-login, and two-factor status) that aren't yet in New Adsmith Frontend, so nothing important is missed. (#80)
- **[Task]** **Deciding the future of the old file-share page** — A quick review to determine whether the legacy file-share page is still needed or can be retired, so nothing users rely on is dropped by accident. (#328)

## Surveys

- **[Feature]** **Making sure every design option actually shows up** — A full check that each customization option on the design tabs is carried all the way through to what visitors see, with any options that do nothing either fixed or removed. (#288)
- **[Feature]** **Finishing the Placement design settings** — A handful of placement design options (like survey height, display format, and skip behavior) aren't yet reflected in the live survey widget. This will finish wiring them up or remove the ones that aren't used. (#293)
- **[Feature]** **Fixing the Modal design tab** — The entire Modal design tab currently has no effect on what visitors see. This will either make those header and progress-bar options work or remove them if the modal is meant to be header-free. (#294)

## Data Clients

- **[Feature]** **Bringing over custom pre-check rules from the old system** — A high-priority effort to port the legacy per-client validation rules (used by hundreds of active data clients) so they run on the new platform instead of silently doing nothing. (#338)
- **[Feature]** **Restoring post-conversion delivery steps** — The legacy "after success" delivery and redirect behaviors for certain clients will be brought over to the new platform as a configurable option. (#327)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging version of the product loaded with production-like data for testing and verification, locked to read-only so nothing can be accidentally changed. (#270)
- **[Task]** **Checking that report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy system, to pinpoint the cause and confirm the numbers are consistent. (#271)
- **[Feature]** **A helper bot for capturing action items** — A tool that reads team conversations and automatically turns agreed-upon needs into tracked work items, reducing manual copy-and-paste. (#272)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — A styling pass so that text boxes, color pickers, checkboxes, and paired fields on the Flow form appear polished and consistent with the other forms, instead of looking unstyled or misaligned. (#152)

## Campaigns

- **[Feature]** **Bringing the Campaigns area to the new platform** — A high-priority, larger effort to add campaign management (creating and editing campaigns, offer groups, and related settings) that exists in the old admin but is currently missing here. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
