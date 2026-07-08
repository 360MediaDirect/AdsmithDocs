# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 18:29:39 UTC · 23 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Task]** **Review of the Users area against the old system** — A side-by-side check of the Users screens to spot anything the previous system offered that's missing here, such as selecting several users at once to change their role, and seeing last-login and two-factor status. The result guides what gets added back. (#80)
- **[Feature]** **Safer editing when two people open the same record** — If a colleague is already editing an offer, placement, advertiser, or other record, you'll see a clear "being edited by…" note and be protected from accidentally saving over each other's changes. (#267)
- **[Feature]** **Removing settings that don't actually do anything** — Some controls (like certain Advertiser web-presence fields, a few user-permission toggles, and some Data Client and Pre-Ping options) are shown but currently have no effect. These will be hidden or removed so the screens only show settings that truly work. (#296)
- **[Task]** **Decision on the old file-sharing page** — Confirming whether the legacy file-share page is still needed and, if so, where it belongs in the new admin — otherwise it'll be retired cleanly. (#328)
- **[Feature]** **A searchable history of changes** — A new activity log will record who changed what and when across the product (including automated changes), so you can look up the history of any offer, placement, or other record. (#276)

## Offers
- **[Bug]** **Saved offer options that never reached the live experience** — Several offer settings were being saved but dropped before visitors saw them. This fix ensures each saved option either takes effect or is removed if it isn't needed. (#295)
- **[Feature]** **Performance projections for new offers** — An automated estimate of how a new offer is likely to perform, based on your historical offer data, to replace the current manual gut-check review. (#322)
- **[Task]** **Auto-register offers ignoring audience targeting** — Auto-register offers are currently shown to everyone, even visitors they should exclude by age, gender, state, zip, or device. This work makes them respect the same targeting rules as regular offers. (#333)
- **[Feature]** **Preview your unsaved changes** — On offer and placement edit screens, Preview will show your current in-progress edits instead of the last saved version, so you no longer have to save just to see how a change looks. (#292)

## Surveys & Modals
- **[Feature]** **Design settings that match what visitors see** — A full check to make sure every option on the Design tab is actually applied in the live survey, with no settings that quietly do nothing. (#288)
- **[Bug]** **Making survey Design settings actually work** — Many survey styling and behavior settings (colors, buttons, header, legal text, progress bar) are saved but don't currently change the live survey. This connects them so your choices take effect. (#290)
- **[Feature]** **Finishing the remaining survey Design settings** — A handful of survey options left over from the previous fix will be wired up (like widget height and question format) or removed if they aren't needed. (#293)
- **[Feature]** **Fixing the Modal Design tab** — The Modal Design tab's settings currently have no effect on the visitor modal. Each will either be made to work or removed so the tab is honest about what it does. (#294)

## Data Clients & Pre-Pings
- **[Feature]** **Restoring after-conversion delivery steps** — Post-conversion delivery and redirect behavior from the old system will be brought over as a configurable option, so affected clients keep working as before. (#327)
- **[Feature]** **Pre-ping checks running at the right moment** — For offers set to check at display time, the real advertiser check will run and hide the offer if it's rejected, matching how the old system worked. (#337)
- **[Feature]** **Bringing over the older per-client pre-ping checks** — Custom pre-ping validation used by hundreds of data clients in the old system isn't running yet on the new platform. This work maps and re-enables those checks so leads are validated as expected. (#338)

## Dashboard & Reports
- **[Task]** **Confirming report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy system, to find the cause and confirm the numbers are trustworthy. (#271)
- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link currently drops you back on the dashboard with no explanation. It will instead show a clear error so you know the test failed. (#239)
- **[Feature]** **Offer impressions showing in placement reports** — Historical placement reports currently show zero offer impressions. This adds that figure so past reports display real numbers. (#339)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging version of the product using production-like data for testing and verification, locked to read-only so no live data can be changed. (#270)
- **[Feature]** **Turning conversations into tracked tasks automatically** — A helper that reads designated Slack conversations and files or updates work items automatically, so action items from meetings don't get lost. (#272)

## Campaigns
- **[Feature]** **Bringing the Campaigns module to the new platform** — Campaign management from the old admin isn't available yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups, matching the old workflow. (#200)

## Flows
- **[Task]** **Cleaning up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking instead of sitting side by side. This tidies the layout so it matches the polished look of the other forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 767867793bb373f1048c3d378d806ae5492206e4d988e86f295446991f13d4bc -->
