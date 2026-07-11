# Open Issues — Plain-Language Overview

_Last updated 2026-07-11 07:33:30 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — High priority. When an offer converts, the pixels set up to record that success currently never fire, so conversions can go uncredited with no visible warning. This fix makes configured success pixels fire reliably. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — High priority. Certain automatic offers are firing for visitors they should exclude (by age, gender, state, zip, or device). Once resolved, these offers will respect the same targeting rules as regular offers. (#333)
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of offer options you can set (including the Modal-tab fields and several delivery flags) are saved but never actually used where visitors see them. This work makes each option either take effect or be cleaned up so nothing misleads you. (#295)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — Today, Preview shows the last saved version. Soon it will reflect the edits you're currently making, so you can check your changes before saving. (#292)
- **[Feature]** **Automatic performance projection for new offers** — Instead of relying on a manual gut-check, new offers could be scored against your historical offer data to estimate how they're likely to perform. This is exploratory work to give the team a helpful, data-driven estimate at intake. (#322)

## General / Across the App

- **[Bug]** **Invalid links should show an error, not bounce to the Dashboard** — When testing a bad link, you're currently dropped on the Dashboard with no explanation. This fix will show a clear failure message so you know the link didn't work. (#239)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit, it will be locked so a colleague can't silently overwrite your changes (and you can't overwrite theirs). If someone else is editing, you'll see who and since when, with an admin option to take over. (#267)
- **[Feature]** **Searchable history of who changed what** — A new admin Audit Log will record every change to your records — manual or automated — with a timestamp and who made it, so you can easily answer "who changed this, and when?" (#276)
- **[Feature]** **Clean up controls that don't do anything** — Several settings (like the Advertiser Web Presence fields, some user permission toggles, and a few Data-Client and Pre-Ping options) currently save but have no effect. They'll be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Decide the future of the legacy file-share page** — The old file-sharing page has no equivalent yet. This is a decision on whether anyone still needs it, so it's either rebuilt or intentionally retired. (#328)

## Surveys

- **[Feature]** **Make Survey design options actually show up in the survey** — Every customization on the Design tab will be checked to confirm it carries through to what visitors see, with any unused options fixed or removed across all screens. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey widget** — A handful of Placement Design-tab settings (like survey height and display format) are saved but not yet reflected in the live widget. This work wires them through, or removes the ones that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behaviors** — Some legacy "after success" delivery steps for specific clients weren't carried over. This brings them back as a configurable option so those clients keep working as before. (#327)
- **[Feature]** **Bring over legacy pre-ping validation for data clients** — High priority. Hundreds of data clients rely on custom serve-time validation checks that aren't running on the new platform yet. This work restores those checks so the right leads are accepted or rejected as they were before. (#338)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only testing environment** — A staging copy of the product will be connected to production-like data in a view-only mode, so the team can verify behavior against realistic data without any risk of changing it. (#270)
- **[Feature]** **Turn Slack conversations into tracked to-dos automatically** — A helper that reads designated Slack messages and files them as tracked issues, so action items from meetings don't get lost or copied over by hand. (#272)

## Reports

- **[Task]** **Confirm report numbers match the legacy system** — Testing found Dashboard report figures didn't line up with the old system. This investigation pins down where any differences come from and confirms the numbers can be trusted. (#271)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — High priority. Campaign management from the legacy system isn't available yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups, matching the old workflow. (#200)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — Every field on the Modal Design tab currently saves but has no effect on what visitors see. This work either wires those header and progress-bar settings into the visitor modal or removes the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or misaligned (plain text boxes, unstyled color pickers, and fields stacking instead of sitting side by side). This tidy-up makes the Flow form match the polished look of the Placement and Modal forms. (#152)

## Users

- **[Task]** **Close the gaps between the old and new Users screens** — A review comparing the legacy Users area to the new one, so features people relied on (like bulk role changes, last-login and two-factor status, and password setup when adding a user) can be prioritized and brought over. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
