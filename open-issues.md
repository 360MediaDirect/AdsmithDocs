# Open Issues — Plain-Language Overview

_Last updated 2026-07-07 20:35:30 UTC · 23 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Task]** **Bringing missing Users features over from the old system** — We're comparing the old Users area to the new one so nothing important gets left behind. Over time you'll get back things like selecting several users at once, seeing two-factor sign-in status, and viewing when someone last logged in. (#80)
- **[Bug]** **Clearer message when a link test fails** — Right now, testing a bad link quietly sends you to the Dashboard. Once fixed, you'll get a clear error telling you the link didn't work, so you're not left guessing. (#239)
- **[Feature]** **Protection against two people editing the same record** — When someone else already has a record open, you'll see who's editing it and won't be able to accidentally overwrite their changes. If you both do edit at once, you'll be warned to refresh instead of losing work. (#267)
- **[Feature]** **A searchable activity history** — Administrators will be able to see who changed what and when across the app — from pausing an offer to editing a placement — making it easy to answer "who changed this?" (#276)
- **[Feature]** **Removing buttons and settings that don't actually do anything** — Some controls (like certain Advertiser web-presence fields and a few user/data-client options) look like they work but have no effect. We'll hide or remove them so the screens only show settings that really matter. (#296)
- **[Task]** **Deciding the future of the old file-share page** — We're checking whether anyone still uses the legacy file-share page so we can either rebuild it in the new app or retire it cleanly. (#328)

## Surveys

- **[Feature]** **Making every design option in a survey take effect** — We're going through all the survey design choices to make sure each one you set actually shows up for visitors, with no "dead" settings that appear to work but don't. (#288)
- **[Bug]** **Turning on survey styling that's currently ignored** — Many Design-tab settings (colors, buttons, headers, legal text, and more) are saved but don't reach the live survey. This connects them so what you configure is what visitors see. (#290)
- **[Bug]** **Voucher code and info links now showing on the survey** — For affected data clients, the voucher code line and the privacy/terms/details links aren't appearing on the live survey the way they did before. This restores them, which matters for both leads and compliance. (#291)
- **[Feature]** **Finishing the last few survey design settings** — A handful of Design-tab options (like survey height and question display format) still don't reach visitors. We'll wire up the ones that should work and remove any that aren't needed. (#293)

## Offers

- **[Bug]** **Offer settings that weren't reaching the live page** — Several saved offer options (including Modal-tab fields and "force more info visible") never made it to what visitors actually see. We'll make sure each saved option either takes effect or is clearly removed. (#295)
- **[Feature]** **Automatic performance estimates for new offers** — Instead of relying on a manual gut-check, new offers could be scored against past offers and history to project how they're likely to perform, giving a helpful estimate at intake time. (#322)
- **[Task]** **Fixing auto-register offers that skip visitor targeting** — Auto-register offers currently fire for everyone, even visitors who should be excluded by age, gender, state, zip, or device. We'll confirm the intended behavior and make sure targeting is respected. (#333)
- **[Feature]** **Previewing your unsaved changes** — On placement and offer edit screens, the Preview button will show your current edits instead of the last-saved version, so you can check changes before saving. (#292)

## Legacy Feature Parity

- **[Feature]** **Bringing the Campaigns module into the new platform** — Campaign management (creating and editing campaigns, offer groups, offers, and related settings) isn't in the new app yet. This adds it back so you can manage campaigns as you did before. High priority. (#200)
- **[Feature]** **Banner placements — confirmed retired** — After review, banner placements haven't run since 2017 and won't be rebuilt in the new platform. This is documented as an intentional decision so it stops being flagged as missing. (#326)
- **[Feature]** **Restoring post-conversion delivery steps for certain clients** — Some clients had special actions that ran after a successful conversion. We're checking which are still needed and rebuilding them in the new platform (or documenting them as retired). (#327)
- **[Feature]** **Restoring an older pre-ping method** — A legacy per-client pre-ping option isn't available in the new platform yet. We'll port it (or confirm the new pre-ping fully covers it) so any offers relying on it keep working. High priority. (#330)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Parts of the Flow form appear unstyled or awkwardly laid out (plain text boxes, misaligned paired fields). This gives the form a clean, consistent appearance that matches the other screens. (#152)

## Modals

- **[Feature]** **Making the Modal Design tab actually work — or removing it** — None of the six Modal Design settings currently affect the visitor modal. We'll either connect them so they take effect or remove the tab if it isn't needed. (#294)

## Reports

- **[Task]** **Investigating why report numbers don't match the old system** — During testing, some Dashboard report figures differed from the legacy app. We're comparing the same date ranges to find and explain any differences and confirm the numbers can be trusted. (#271)

## Behind the Scenes

- **[Task]** **Setting up a safe testing environment** — We're standing up a read-only test environment using production-like data, so the team can verify the app against real-world numbers without any risk of changing live data. (#270)
- **[Feature]** **Turning conversations into tracked to-dos automatically** — An internal helper will read team chat and file the action items for us, so requests raised in conversation don't slip through the cracks. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8f35b6bb8c9f04a34bfea6e350a1042391d5802a91bb952fed266f447103150c -->
