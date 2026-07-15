# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 17:28:56 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Feature]** **Preview button shows your unsaved changes** — When editing a placement or offer, the Preview will reflect the edits you've made on screen, so you can check your work without having to save first. (#292)
- **[Bug]** **Saved offer options now reach the live experience** — Several offer settings you configure (including modal options, display URL, and certain data-client flags) currently don't actually appear where visitors see them; this fixes them so what you set is what runs. (#295)
- **[Bug]** **Success pixels will actually fire** — Conversion tracking pixels set up on an offer aren't currently firing, meaning lost tracking with no warning. Once fixed, configured success pixels will fire reliably. (#297)
- **[Bug]** **Auto-register offers will respect targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting and can fire for visitors who should be excluded. This makes them honor the same targeting rules as regular offers. (#333)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool to estimate a new offer's likely performance based on your historical offer data, replacing an informal manual gut-check with a data-driven projection. (#322)

## General / Across the App
- **[Feature]** **Protection against two people overwriting the same record** — When someone is already editing a record, you'll see who has it open, and you'll be warned before you can accidentally save over changes made by a colleague. This works across offers, flows, placements, advertisers, and other entity screens. (#267)
- **[Feature]** **Tidying up controls that don't do anything** — Some admin settings (like the Advertiser Web Presence fields and a few permission and data-client options) currently save but have no effect. These will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Decision on the legacy file-share page** — Reviewing whether the old file-share page is still needed in New Adsmith Frontend, so it's either rebuilt or cleanly retired. (#328)
- **[Task]** **Users screen review against the old system** — A comparison of the Users area with the legacy version to confirm which features are carried over and which still need building, so nothing important is missed. (#80)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently drops you back on the Dashboard with no explanation; instead you'll get a clear failure message so you know the link didn't work. (#239)

## Surveys
- **[Feature]** **Design settings will match what visitors actually see** — A review to make sure every design and customization option on the Survey and other entity screens is actually reflected in the live survey, with any options that do nothing being fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A handful of Placement design settings (such as height and display format) aren't yet reflected in the live widget; this connects them so your choices take effect. (#293)

## Data Clients
- **[Feature]** **Restoring after-conversion delivery behavior** — Post-conversion delivery steps from the legacy system weren't carried over yet; this brings them back so client delivery works as it did before. (#327)
- **[Feature]** **Restoring custom pre-ping checks for data clients** — Custom validation checks that ran for hundreds of data clients in the old system aren't running on the new platform yet. This ports them over so those checks happen again at the right moment. (#338)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a testing environment using a copy of live data where nothing can be accidentally changed, so the team can verify the product against realistic data. (#270)
- **[Feature]** **Automatic issue-logging from Slack conversations** — An internal helper that turns discussion notes into tracked work items automatically, reducing manual copying and speeding up how quickly requests get logged. (#272)

## Flows
- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow editing form appear unstyled or don't line up neatly. This cleans up the layout so fields and controls display properly, matching the rest of the app. (#152)

## Campaigns
- **[Feature]** **Bringing the Campaigns area to New Adsmith Frontend** — Campaign management (creating and editing campaigns, offer groups, and related settings) exists in the old admin but isn't in the new one yet. This is high priority and will let you manage campaigns again. (#200)

## Modals
- **[Feature]** **Making the Modal Design tab work (or removing it)** — The Modal Design settings currently have no effect on what visitors see. This will either connect them so they display, or remove the tab if it isn't needed. (#294)

## Reports
- **[Task]** **Confirming report numbers match the old system** — Investigating why some Dashboard report figures didn't line up with the legacy system, to pinpoint any differences and confirm the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f12be1691f4d05be7a51684fc6fe5ab6d4c4751d5a9de6a600395df673d554b3 -->
