# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 05:52:05 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on Placements and Offers** — When editing a placement or offer, the Preview will show exactly what you've changed on screen, even before you save, so you no longer have to save first just to check how an edit looks. (#292)
- **[Bug]** **Saved offer options that never reach the live experience** — Several offer settings you fill in are being quietly dropped and never applied to what visitors see (including certain modal, "force more info," and display-URL options). This fix ensures the options you set actually take effect. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers to fire on success currently never fire, meaning completed leads aren't being tracked. Fixing this restores accurate conversion and revenue reporting. (#297)
- **[Feature]** **Automatic performance projection for new offers** — Instead of relying on an informal manual gut-check, new offers will get an automated, data-driven estimate of how they're likely to perform based on your own historical offer data. (#322)
- **[Task]** **Auto-register offers should respect visitor targeting** — Auto-register offers are currently firing for everyone, ignoring age, gender, state, zip, and device targeting. This work makes sure they only fire for the visitors they're meant to reach. (#333)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two users open the same record, the app will warn them and protect against one person's changes silently wiping out the other's, across offers, flows, placements, advertisers, and more. High priority. (#267)
- **[Feature]** **Remove admin controls that don't actually do anything** — Some settings (like Advertiser web-presence fields, certain user permission toggles, and a few data-client and pre-ping options) currently save but have no effect. They'll be hidden or removed so the screens only show controls that genuinely work. (#296)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent yet in New Adsmith Frontend. This is a review to confirm whether anyone still needs it or it can be retired. (#328)
- **[Bug]** **Clear error when testing an invalid link** — Testing an invalid link currently dumps you back on the Dashboard with no explanation; it will instead show a clear failure message so you know the test didn't pass. Nearly complete. (#239)
- **[Task]** **Users screen feature comparison with the old system** — A review comparing the Users area against the legacy version to spot missing options (like bulk actions, last-login, and two-factor status) so nothing important is left behind. Documentation and planning work. (#80)

## Surveys

- **[Feature]** **Make sure every Design-tab option affects the survey** — A full check to confirm each customization on the Design tab actually shows up in the live survey, so no setting is left doing nothing. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey** — Several placement Design-tab settings (like survey height and display format) don't yet reach the live survey. This work wires the remaining ones through or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery steps for data clients** — Certain after-success delivery and redirect behaviors from the old system weren't carried over yet. This brings them back so data clients keep working as they did before. Nearly complete. (#327)
- **[Feature]** **Bring back custom pre-ping checks for data clients** — Hundreds of data clients rely on custom validation that runs before a lead is served, and it isn't running yet on the new platform. This restores those checks so leads are validated correctly. High priority. (#338)

## Behind the Scenes

- **[Task]** **Set up a read-only test environment** — A safe, view-only copy of the app running against production-like data, so the team can verify behavior without any risk of changing real records. (#270)
- **[Feature]** **Turn conversation notes into tracked work items automatically** — A helper that reads team conversations and files the resulting to-dos as tracked issues, cutting down manual copy-and-paste when capturing action items. (#272)

## Dashboard

- **[Task]** **Confirm Dashboard report numbers match the old system** — An investigation into why some Dashboard figures differ from the legacy app, to pin down the cause and make sure the reported numbers can be trusted. (#271)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form currently look unstyled or misaligned, with fields stacking oddly instead of sitting side by side. This tidies up the layout to match the other forms. Partly done. (#152)

## Campaigns

- **[Feature]** **Add the Campaigns area to the new platform** — Campaign management from the old admin isn't available yet, so you can't create, edit, or organize campaigns and offer groups. This adds the full Campaigns area back. Critical, high priority. (#200)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — Every field on the Modal Design tab currently saves but has no effect on the modal visitors see. This work either connects those fields so they display, or removes the tab if it isn't needed. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f12be1691f4d05be7a51684fc6fe5ab6d4c4751d5a9de6a600395df673d554b3 -->
