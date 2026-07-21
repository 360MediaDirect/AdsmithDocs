# Open Issues — Plain-Language Overview

_Last updated 2026-07-21 17:31:31 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview offers and placements with your unsaved changes** — When editing an offer or placement, the Preview button will show exactly what you've changed on screen, even before you save, so you no longer have to save just to check how an edit looks. (#292)
- **[Bug]** **Some saved offer options never reach the live ad** — A number of offer settings you fill in (including the Modal-tab options, "Force More Info Visible," Display URL, and several data-client flags) are currently being dropped and never take effect. This fix makes sure the options you configure actually apply. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — Conversion/success pixels set up on offers silently never fire, which means conversions aren't being recorded. This high-priority fix ensures a configured success pixel actually fires when a conversion happens, protecting your attribution and revenue tracking. (#297)
- **[Feature]** **Automatic performance projection for new offers** — Instead of relying on a manual gut-check, new offers could be scored automatically against your historical offer data to estimate how they're likely to perform. This is an exploratory decision aid to help judge new offers at intake. (#322)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for every visitor even when age, gender, state, zip, or device targeting should exclude them. This high-priority fix makes these offers respect the same targeting rules as regular offers. (#333)
- **[Bug]** **"Conflicting Referrals" field has no effect** — The Conflicting Referrals box on the offer Delivery tab is saved but currently does nothing at serve time. This work confirms the intended behavior and wires it up so the setting is either enforced or removed to avoid confusion. (#351)

## Surveys

- **[Feature]** **Design tab options fully connected to what visitors see** — Every customization on the survey Design tab will actually be reflected in the live survey view, and all form options across the product will be audited so nothing is left disconnected. You'll be able to trust that the options you set genuinely change the output. (#288)
- **[Feature]** **Placement design settings now shown in the survey widget** — Several placement Design-tab settings (like iFrame height and display format) are saved but not yet applied to the live widget. This finishes connecting them so your placement styling and behavior choices take effect. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Post-conversion delivery behavior restored for clients** — Certain after-success actions from the legacy system (post-conversion delivery and redirect steps for specific clients) weren't carried over. This work brings that behavior back so those clients keep working as before. (#327)
- **[Feature]** **Bring over legacy pre-ping validation for data clients** — Custom serve-time validation used by hundreds of data clients in the old system doesn't currently run on the new platform. This high-priority work restores that checking so those clients' pass/reject rules apply again before serving. (#338)

## Behind the Scenes

- **[Task]** **A safe, read-only testing environment** — Setting up a staging version of New Adsmith Frontend using a copy of real data, locked to read-only, so the team can verify behavior against realistic data without any risk of changing live records. (#270)
- **[Feature]** **A Slack helper that turns conversations into tracked work items** — A behind-the-scenes assistant that reads designated Slack discussions and automatically logs action items as tracked tasks, reducing manual note-taking and follow-up. (#272)

## Reports & Dashboard

- **[Task]** **Confirming dashboard report numbers match the old system** — During testing, some Dashboard report figures didn't line up with the legacy system. This investigation compares the two over a fixed date range, pinpoints any differences, and confirms the numbers can be trusted. (#271)

## Advertisers & General / Across the App

- **[Feature]** **Remove admin controls that don't actually do anything** — Several settings (the Advertiser Web Presence fields, certain user-permission toggles, and a few data-client and pre-ping options) are saved but have no real effect. Removing or hiding them prevents confusion and false expectations about what they control. (#296)

## Properties

- **[Bug]** **Domain allowlist will finally be enforced** — The allowed-domains list on a Property is editable today but isn't actually applied, so ads serve on any site. This fix makes the allowlist work: only approved hostnames will serve the ad, while properties that leave the list empty are unaffected. (#350)

## Flows

- **[Task]** **Clean up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned compared to other forms (plain text boxes, unstyled color pickers, and fields that stack instead of sitting side by side). This work tidies the layout so the Flow form looks consistent with the rest of the app. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The Modal Design tab's header and progress-bar settings are saved but never appear on the visitor modal. This work either wires them up so they display, or removes the tab if the modal is meant to be header-less. (#294)

## Admin & Users

- **[Task]** **Comparing the new Users area against the old one** — A documentation review that maps what the legacy Users management offered versus the new Users screen, so any missing capabilities (like bulk role changes, last-login info, and 2FA status) are identified and prioritized. (#80)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
