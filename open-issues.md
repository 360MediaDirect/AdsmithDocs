# Open Issues — Plain-Language Overview

_Last updated 2026-07-18 20:15:42 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview shows your unsaved edits** — When you preview a placement or offer while editing, you'll see the changes you just made instead of the last-saved version, so you no longer have to save first just to check how something looks. (#292)
- **[Bug]** **Some offer settings weren't reaching live pages** — Several saved offer options (including Modal-tab settings, a "Display URL," and a few delivery flags) weren't actually being used when offers were shown to visitors. This fix makes sure the choices you set on an offer take effect, or removes the ones that were never meant to do anything. (#295)
- **[Bug]** **Success pixels now fire correctly** — High priority. Conversion tracking pixels set up on offers were silently never firing, which meant lost tracking of successful conversions. Once fixed, the pixels you configure will fire as expected. (#297)
- **[Bug]** **Auto-register offers will respect visitor targeting** — High priority. Certain "auto-register" offers were being counted for every visitor, ignoring the age, gender, state, ZIP, and device targeting you set. This work makes those offers honor your targeting rules so they only count for the right visitors. (#333)
- **[Bug]** **The "Conflicting Referrals" field will do something (or be removed)** — Right now this offer field can be filled in but has no effect on what visitors see. We're confirming its intended purpose and will either make it work or take it off the form so it isn't misleading. (#351)
- **[Feature]** **Automatic performance projections for new offers** — Exploratory. We're looking at estimating how a new offer is likely to perform based on your own historical offer data, to replace today's manual gut-check review. If it pans out, you'd see a projection right when a new offer comes in. (#322)

## Surveys

- **[Feature]** **Design choices will actually show up in surveys** — We're checking every customization option across all entity screens to make sure the settings you pick in the Design tab are truly reflected in what visitors see, with no options that quietly do nothing. (#288)
- **[Feature]** **Finishing the Placement Design-tab settings** — A few placement design options (like survey height and display format) are saved but not yet applied to the live widget. This work connects them so your design choices take effect, and cleans up any settings that aren't used. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bringing back post-conversion delivery behaviors** — Some client-specific actions that ran after a successful conversion in the old system weren't carried over. This restores them in a flexible, reusable way so those clients keep working as before. (#327)
- **[Feature]** **Restoring custom pre-ping checks for data clients** — High priority. Hundreds of data clients rely on custom serve-time validation from the old system that currently doesn't run on the new platform. This work brings that validation back so those checks are applied again. (#338)

## Modals

- **[Feature]** **Making the Modal Design tab work (or removing it)** — The Modal Design tab's header and progress-bar settings are saved but never shown to visitors. We'll either wire them up so they appear or remove the tab to avoid confusion. (#294)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned, with some paired fields stacking instead of sitting side by side. This cleanup brings the Flow form in line with the polished look of the Placement and Modal forms. (#152)

## Properties

- **[Bug]** **Property domain allowlist will be enforced** — Today a property's list of allowed domains is editable but not actually applied, so ads can serve on any website. This fix makes the allowlist work, so ads only serve on the domains you've approved. (#350)

## Dashboard

- **[Task]** **Confirming Dashboard report numbers match the old system** — During testing, some Dashboard report figures didn't line up with the legacy system. We're investigating where the difference comes from so you can trust the numbers match. (#271)

## Admin & Users

- **[Task]** **Reviewing the Users area against the old system** — A detailed comparison of the old and new Users screens is underway to spot any missing options (like bulk role changes or last-login info) so the new Users area covers what you rely on. (#80)

## General / Across the App

- **[Feature]** **Removing admin controls that don't do anything** — Several settings across the app (such as Advertiser "Web Presence" fields and some user permission toggles) are saved but have no real effect. We'll hide or remove these so the admin screens only show controls that actually work. (#296)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a practice copy of the product loaded with realistic data for testing and verification, locked to read-only so nothing can be changed by accident. (#270)
- **[Feature]** **Turning conversations into tracked work items automatically** — A helper that reads team discussions and files the resulting to-dos automatically, reducing manual note-taking so nothing slips through the cracks. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
