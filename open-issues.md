# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 09:37:03 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — Conversion tracking pixels that admins set up on offers are silently not firing, meaning successful conversions aren't being recorded. This high-priority fix will make sure configured success pixels reliably fire so you don't lose attribution. (#297)
- **[Bug]** **Some saved offer settings never reach live pages** — A number of offer options you can set in the form (including the Modal-tab fields, Display URL, and several data-client flags) currently get dropped and never take effect on the visitor-facing pages. This work makes each setting either work as expected or be cleanly removed so the form only shows options that actually do something. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting, so they can fire for people they should exclude. This confirms and corrects that behavior so these offers only fire for the right visitors. (#333)
- **[Feature]** **Preview unsaved changes on placements and offers** — Today the Preview button shows the last saved version, so you have to save before you can see edits. Soon Preview will reflect your current, unsaved changes, letting you check your work before committing it. (#292)
- **[Feature]** **Performance projection for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, giving the team a quick, data-driven read at intake instead of relying on a manual gut-check. (#322)

## General / Across the App

- **[Feature]** **Warn when two people edit the same record** — When two users open the same record, one person's changes can quietly overwrite the other's. This adds a friendly "someone else is editing this" notice and a safeguard on save, so edits across offers, flows, placements, advertisers, and more won't clobber each other. (#267)
- **[Feature]** **Clean up admin controls that don't do anything** — Several settings (like the Advertiser Web Presence fields, certain user-permission toggles, and a few Data-Client and Pre-Ping options) are shown but currently have no effect. These will be hidden or removed so the screens only show controls that actually work. (#296)
- **[Task]** **Bringing the Users area up to full parity** — An ongoing review comparing the older Users screens to the new ones to spot missing capabilities (like bulk actions and additional columns). This guides what still needs to be built so the new Users management matches what you're used to. (#80)
- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link currently dumps you on the dashboard with no explanation. This fix shows a proper error message so you immediately know the link didn't pass. (#239)
- **[Task]** **Decision on the legacy file-share page** — The old file-share page has no equivalent in New Adsmith Frontend yet. This confirms whether anyone still needs it, and either brings it over or documents that it's been retired. (#328)

## Surveys

- **[Feature]** **Design tab settings will match what visitors see** — A thorough check to make sure every customization option on the design tabs is actually reflected in the survey, with any options that go nowhere fixed or removed across all screens. (#288)
- **[Feature]** **Finishing the Placement Design settings** — A handful of Placement design options (like iFrame height and display format) are saved but not yet shown to visitors. This wires them through so your design choices take effect, and tidies up any that shouldn't be there. (#293)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery behavior** — Some after-success delivery and redirect behaviors from the older system weren't carried over yet. This brings them back as a reusable setting so affected clients keep working as before. (#327)
- **[Feature]** **Restoring per-client pre-ping checks at serve time** — Hundreds of data clients rely on custom serve-time validation from the old system that isn't running on the new platform yet. This high-priority work maps each client's checks over and runs them at the right moment, so leads are validated correctly. (#338)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the product against realistic data for testing and verification, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Automatic issue-filing from team chats** — A helper that reads team conversations and turns action items into tracked tasks automatically, reducing manual copy-paste and keeping follow-ups from slipping through the cracks. (#272)

## Reports

- **[Task]** **Confirming report numbers match the previous system** — Testing surfaced dashboard report figures that didn't line up with the older system. This investigation pins down where any differences come from and confirms the numbers can be trusted. (#271)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Parts of the Flow form currently look unstyled or misaligned compared to other forms, with fields stacking oddly instead of sitting side by side. This cleanup brings the Flow form's look in line with the rest of the app. (#152)

## Modals

- **[Feature]** **Making the Modal Design tab do something** — The Modal Design tab's fields (header text, colors, progress bar, and more) are saved but don't currently appear to visitors. This either wires them up so they show, or removes the tab if the modal is meant to be header-less. (#294)

## Campaigns

- **[Feature]** **Bringing Campaigns into New Adsmith Frontend** — Campaign management from the older admin isn't available in the new platform yet. This high-priority work adds a Campaigns area so you can view, create, edit, and configure campaigns and their offer groups, just like before. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f12be1691f4d05be7a51684fc6fe5ab6d4c4751d5a9de6a600395df673d554b3 -->
