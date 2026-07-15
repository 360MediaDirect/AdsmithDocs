# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 13:32:19 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Live preview of unsaved changes on Placements and Offers** — When editing a placement or an offer, the Preview button will show your current edits right away, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Some saved offer options never reach the live experience** — A number of settings you fill in on the offer form (including modal-tab fields and display options) are being lost before they show to visitors. This fix makes sure the options you save actually take effect. (#295)
- **[Bug]** **Success pixels not firing on offers** — Conversion tracking pixels set up on an offer are silently never firing, which means lost tracking of results. This high-priority fix ensures configured success pixels fire as expected. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers are firing for everyone, even for people who should be excluded by age, gender, state, zip, or device rules. This work makes those offers respect the same targeting rules as regular offers. (#333)
- **[Feature]** **Automatic performance projection for new offers** — Instead of relying on a manual gut-check, new offers could be scored against past offers and historical results to estimate how they're likely to perform. An early, exploratory idea to give a data-driven read at intake. (#322)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is already editing a record, you'll see a clear "locked by" notice, and if a record changes while you have it open you'll be prompted to reload instead of accidentally wiping out their work. This protection will apply across all the main entity screens. (#267)
- **[Feature]** **Remove buttons and options that don't actually do anything** — Several admin controls (Advertiser Web Presence fields, some user permission toggles, and a few Data-Client and Pre-Ping options) currently save but have no effect. They'll be hidden or removed so the screens only show controls that truly work. (#296)
- **[Bug]** **Invalid links in Link Testing send you to the dashboard** — Testing a bad link currently drops you on the dashboard with no explanation. Once fixed, you'll get a clear error result telling you the link failed. (#239)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent in New Adsmith Frontend. This is a quick check on whether anyone still needs it before deciding to rebuild or retire it. (#328)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior for data clients** — Certain "after success" delivery and redirect behaviors from the old system weren't carried over. This work brings them back in a flexible, configurable way so affected clients keep working. (#327)
- **[Feature]** **Bring back file-based pre-ping checks for data clients** — Hundreds of data clients rely on custom validation checks that currently don't run in New Adsmith Frontend. This high-priority effort re-creates that validation so those clients' checks work again. (#338)

## Surveys

- **[Feature]** **Make sure every design option actually changes the survey** — Design-tab customizations will be reviewed across all screens to confirm each one truly affects what visitors see, with any options that do nothing either fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — A handful of Placement design options (like survey height and display format) are saved but not yet shown to visitors. This wires them through so they take effect. (#293)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of the product will be stood up against realistic data for verification, locked to read-only so testing can't change anything. Behind-the-scenes maintenance. (#270)
- **[Feature]** **Slack-to-issue helper for turning conversations into tasks** — An internal tool to automatically capture action items from Slack and file them as tracked issues, reducing manual copy-and-paste. Internal tooling with no direct effect on the product screens. (#272)

## Reports

- **[Task]** **Confirm dashboard report numbers match the old system** — During testing, some dashboard figures didn't line up with the legacy app. This investigation pins down why and confirms the numbers can be trusted. (#271)

## Flows

- **[Task]** **Fix visual styling issues on the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other forms. This tidy-up brings its appearance in line with the rest of the app. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — All six fields on the Modal Design tab currently save but never show to visitors. They'll either be wired up to actually appear in the modal or removed to avoid confusion. (#294)

## Users

- **[Task]** **Close the gaps between the old and new Users screens** — A detailed review of the Users area to identify what the old system had that the new one is still missing (like bulk actions and extra columns), so nothing important is left behind. (#80)

## Campaigns

- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — Campaign management, a core feature from the old admin, isn't available yet. This high-priority work adds the ability to create, edit, and configure campaigns and their offer groups. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f12be1691f4d05be7a51684fc6fe5ab6d4c4751d5a9de6a600395df673d554b3 -->
