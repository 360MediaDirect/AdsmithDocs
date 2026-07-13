# Open Issues — Plain-Language Overview

_Last updated 2026-07-13 16:50:24 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview shows your unsaved changes** — When you preview a placement or offer while editing, you'll see exactly what you've changed on screen instead of the last saved version, so you can check your work without saving first. (#292)
- **[Bug]** **Some saved offer settings weren't reaching live pages** — A number of offer options you fill in (including the offer's Modal settings, Force More Info Visible, Display URL, and several data-client options) weren't being carried through to what visitors actually see. This fix makes sure each option either works or is cleaned up. (#295)
- **[Bug]** **Success tracking pixels now fire correctly** — Conversion pixels set up on offers were silently never firing, meaning completed conversions weren't being tracked. This high-priority fix restores that tracking so you don't lose credit for results. (#297)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, new offers will get an estimated performance projection based on your own historical offer data, giving you a helpful read on how an offer is likely to do. (#322)
- **[Bug]** **Auto-register offers will respect visitor targeting** — Auto-register offers were firing for everyone, ignoring age, gender, state, zip, and device targeting rules. This high-priority fix makes them honor the same targeting as regular offers so they only reach the right visitors. (#333)

## General / Across the App

- **[Feature]** **Warning when two people edit the same record** — If a colleague is already editing an offer, placement, advertiser, or other record, you'll see a clear "locked by" notice and be protected from accidentally overwriting each other's changes. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when across the app, including automated updates, so you can easily answer "who changed this and when" for any record. (#276)
- **[Feature]** **Clean up controls that don't do anything** — Several admin settings (like the Advertiser Web Presence fields, some user permission toggles, and a few data-client and pre-ping options) look active but currently have no effect. They'll be hidden or removed so the screens only show controls that actually work. (#296)
- **[Task]** **Decision on the old file-share page** — The legacy file-sharing page has no equivalent in New Adsmith Frontend. We're confirming whether anyone still needs it before either rebuilding it or officially retiring it. (#328)
- **[Task]** **Review of the Users area against the old system** — A detailed comparison of the Users screens in New Adsmith Frontend versus the legacy system, so we know which features still need to be added (like bulk role changes and last-login details). (#80)

## Surveys

- **[Feature]** **Design tab settings will fully affect the live survey** — We're checking that every design customization you set actually shows up in the survey visitors see, and auditing form options across all screens so nothing is a dead end. (#288)
- **[Feature]** **Finish connecting Placement Design settings** — A handful of placement design options (like survey height and display format) aren't yet reflected in the live survey widget. This finishes wiring them up, or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Bring back post-conversion delivery steps** — Certain after-success actions from the old system (used by active clients) weren't carried over. This restores that behavior so post-conversion delivery works as it did before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients rely on custom pre-ping validation that isn't running on the new platform yet. This high-priority work brings that validation back so leads are checked correctly before delivery. (#338)

## Reports & Dashboard

- **[Task]** **Making sure new dashboard numbers match the old system** — Testers noticed some dashboard report figures didn't match the legacy app. We're investigating where the difference comes from and confirming the numbers can be trusted. (#271)
- **[Bug]** **Clear error for a bad test link** — When you test an invalid link, you're currently bounced to the dashboard with no explanation. This fix will show a proper error message so you know the link didn't work. (#239)

## Behind the Scenes

- **[Task]** **A read-only test environment with real-world data** — Setting up a safe, view-only staging copy so the team can verify the product against production-like data without any risk of changing real records. (#270)
- **[Feature]** **Turning conversations into tracked tasks automatically** — A helper that reads team chat and files action items as tracked issues automatically, cutting out manual copy-and-paste when capturing requests. (#272)

## Campaigns

- **[Feature]** **Bringing the Campaigns module to New Adsmith Frontend** — The Campaigns feature from the old admin isn't available yet. This high-priority work adds the ability to view, create, edit, and configure campaigns and their offer groups, matching the legacy workflow. (#200)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — Every field on the Modal Design tab currently saves but has no effect on the modal visitors see. This will either wire those header and progress-bar settings into the live modal or remove the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with paired fields stacking awkwardly instead of sitting side by side. This cleanup brings the form's appearance in line with the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
