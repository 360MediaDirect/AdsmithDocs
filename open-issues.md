# Open Issues — Plain-Language Overview

_Last updated 2026-07-19 20:17:01 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Feature]** **Preview your unsaved changes** — When editing a placement or offer, the Preview button will show your current edits instead of only the last saved version, so you can check a change before committing to it. (#292)
- **[Bug]** **Some saved offer options weren't reaching live ads** — A number of options you set on an offer were being dropped and never appeared to visitors. This fix makes sure the settings you configure actually take effect (or removes options that were never meant to do anything). (#295)
- **[Bug]** **Success tracking pixels weren't firing** — A high-priority fix so the "pixels to fire on success" you configure on an offer actually fire on a conversion. Today they silently do nothing, which means lost conversion tracking. (#297)
- **[Feature]** **Automatic performance estimate for new offers** — An exploratory tool that projects how a new offer is likely to perform based on your historical offer data, replacing today's manual gut-check review. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — A high-priority fix so auto-register offers honor age, gender, state, ZIP, and device targeting like regular offers do, instead of firing for visitors they should exclude. (#333)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This field is saved but has no effect on which offers are shown. The team is confirming the intended rule so it can either be made to work or removed to avoid confusion. (#351)

## Surveys
- **[Feature]** **Every design setting will actually show up in the survey** — A thorough pass to make sure the customizations you set on the Design tab are reflected in what visitors see, with a review across all entities to catch any options that aren't wired through. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live widget** — A few Placement Design-tab settings (like survey height and display format) are saved but not yet applied to what visitors see. This finishes wiring them up or removes the ones that aren't needed. (#293)

## Data Clients
- **[Feature]** **Post-conversion delivery behaviors carried over from the old system** — Custom "after success" delivery and redirect steps that ran in the legacy system will work again on New Adsmith Frontend, so no client behavior is lost in the move. (#327)
- **[Feature]** **Bring legacy pre-ping validation over to the new platform** — A high-priority effort to restore custom serve-time validation for hundreds of data clients that relied on it, so those checks run correctly on New Adsmith Frontend. (#338)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the product loaded with realistic data, locked to read-only, so the team can verify behavior without any risk to live data. (#270)
- **[Feature]** **Automatic issue capture from team chat** — An internal helper that turns action items from team conversations into tracked work items automatically, reducing manual copy-and-paste. (#272)

## Modals
- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The Modal Design tab settings currently don't affect the visitor-facing modal. This work will either connect them so they display, or remove the tab so it isn't misleading. (#294)

## Flows
- **[Task]** **Tidy up the look of the Flow form** — Fixes to spacing and styling on the Flow form so text areas, color pickers, checkboxes, and paired fields look consistent with the rest of the app instead of appearing unstyled. (#152)

## Properties
- **[Bug]** **Domain allowlist will actually be enforced** — When a property lists allowed domains, requests from other websites will be blocked as expected. Today the list is saved but ignored, so any site can serve the ads. (#350)

## Users
- **[Task]** **Closing the gap with the old Users area** — A detailed review comparing the legacy user management screens with the new ones to identify missing capabilities (like bulk actions and last-login info) and prioritize bringing them over. (#80)

## Dashboard
- **[Task]** **Getting dashboard report numbers to match the old system** — An investigation into why some dashboard figures differ from the legacy app, so reported numbers can be trusted and validated. (#271)

## General / Across the App
- **[Feature]** **Removing settings that don't do anything** — Several admin controls (such as the Advertiser Web Presence fields and certain permission toggles) are shown but currently have no effect. They'll be hidden or removed so screens only show options that actually work. (#296)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
