# Open Issues — Plain-Language Overview

_Last updated 2026-07-17 17:25:11 UTC · 17 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — When an advertiser sets up pixels to fire when a lead converts successfully, those pixels are currently never triggered, which means conversions go unrecorded with no warning. This high-priority fix ensures configured success pixels actually fire so you don't lose credit for conversions. (#297)
- **[Bug]** **Some saved offer settings never reach live ads** — Several options you fill in on an offer (including the Modal-tab fields, Display URL, and certain data-delivery flags) are saved but quietly dropped before they reach the live experience. This work makes sure each saved option is either honored or clearly removed so what you configure is what visitors get. (#295)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for every visitor, even ones who fall outside the age, gender, state, ZIP, or device targeting you set. This high-priority fix makes those offers respect your targeting rules so they only fire for the right audience. (#333)
- **[Feature]** **Preview shows your unsaved changes** — On placement and offer edit screens, the Preview button will reflect the edits you're currently making instead of only the last saved version, so you can check your changes before committing them. (#292)
- **[Feature]** **Smart performance projections for new offers** — An exploratory feature that would estimate how a new offer is likely to perform based on your historical offer data, giving you a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Surveys

- **[Feature]** **Design-tab options fully connected across the app** — A thorough pass to make sure every customization option you set on a Design tab actually shows up in the live survey, with a review of all entity forms to catch and fix any settings that currently do nothing. (#288)
- **[Feature]** **Placement Design settings that finally take effect** — Several Placement Design-tab options (like iFrame height, display format, and skip behavior) are saved but don't yet change the live widget. This work wires them through so they work as expected, or removes any that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back file-based pre-ping validation** — Hundreds of data clients rely on custom, serve-time checks that decide whether an ad should be shown, and these haven't been carried over to New Adsmith Frontend yet. This high-priority work restores that validation so those clients behave as they did before. (#338)
- **[Feature]** **Restore post-conversion delivery steps** — The legacy "after-success" behaviors (delivery and redirect steps that run after a lead converts) are being ported over as a reusable, configurable option so affected clients keep working as before. (#327)

## Behind the Scenes

- **[Task]** **A safe practice environment for testing** — Setting up a test version of the app that uses realistic, look-alike data but can't change anything, so the team can verify behavior against production-like data without any risk. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads team chat and files the action items as tracked issues automatically, reducing manual note-taking and making sure requests don't slip through the cracks. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab do something** — The entire Modal Design tab (header text, colors, and progress bar) is currently saved but never shown to visitors. This work either makes those settings appear in the visitor modal or removes the tab so nothing is misleading. (#294)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form currently look unstyled or misaligned, with fields stacking oddly and text boxes and color pickers using plain browser defaults. This cleanup brings the form in line with the polished look of the Placement and Modal forms. (#152)

## Properties

- **[Bug]** **Domain allowlist will actually block unlisted sites** — Today, the allowed-domains list on a Property is saved but never enforced, so ads serve on any website regardless of the list. This fix makes the allowlist work, so ads only serve on the domains a publisher has approved. (#350)

## Dashboard & Reports

- **[Task]** **Confirming report numbers match the old system** — An investigation into why some Dashboard report figures didn't line up with the legacy system, so any differences can be pinned down and corrected, giving you confidence the numbers are accurate. (#271)

## Users

- **[Task]** **Closing the gap with the old Users screen** — A detailed review comparing the current Users area to the legacy version to identify missing capabilities (like bulk actions, last-login and two-factor details, and password setup) so they can be prioritized and added back. (#80)

## General / Across the App

- **[Feature]** **Remove controls that don't do anything** — Several admin settings across Advertisers, Users, Data Clients, and Pre-Pings are saved but have no actual effect, which can be confusing and misleading. These will be hidden or removed (or properly implemented), so every control you see actually does what it says. (#296)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: ab95f9a9ff7298cfa22ea173f916bfe22c57dff5afb263ccbb1f4a49819b6e4b -->
