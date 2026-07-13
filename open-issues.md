# Open Issues — Plain-Language Overview

_Last updated 2026-07-13 09:04:45 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Conversion tracking pixels aren't firing** — A high-priority fix so that the "fire on success" pixels you set up on an offer will actually fire when a conversion happens, restoring accurate tracking and attribution that's currently being lost silently. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several options you fill in on the Offer form (including modal settings, display URL, and certain data-client flags) are being dropped before they take effect. This work makes sure the settings you save are either honored or removed so nothing looks active when it isn't. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — A high-priority fix so that auto-registering offers honor the same age, gender, state, ZIP, and device targeting as regular offers, preventing them from firing for visitors who should be excluded. (#333)
- **[Feature]** **Preview your unsaved offer and placement edits** — The Preview button will show your current in-progress changes instead of only the last-saved version, so you can check your work before committing it. (#292)
- **[Feature]** **Performance projection for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, helping guide decisions at intake without relying on a manual gut-check. (#322)

## Admin Area

- **[Feature]** **Protection against two people overwriting each other** — When you open a record to edit, others will see it's locked and won't be able to accidentally save over your changes; if a record was changed while you had it open, you'll be prompted to reload instead of losing work. (#267)
- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every change to your records (and automated system changes too), with who made it and when, so you can easily track down "who changed this and when." (#276)
- **[Feature]** **Removing controls that don't do anything** — Several settings that currently save but have no effect (Advertiser Web Presence fields, some user permission and data-client options, and a pre-ping option) will be hidden or removed so the admin screens only show controls that actually work. (#296)
- **[Task]** **Review of the Users area against the old system** — A behind-the-scenes documentation effort comparing the new Users management screens to the legacy version to confirm nothing important is missing. (#80)
- **[Task]** **Decision on the old file-share page** — Confirming whether the legacy file-share page is still needed and either bringing it into the new admin or retiring it for good. (#328)

## Surveys

- **[Feature]** **Design tab choices will show up in the survey** — Ensuring every customization option on the Design tab actually appears in the live survey, plus a review across all screens to catch any settings that currently lead nowhere. (#288)
- **[Feature]** **Finishing the Placement Design tab settings** — A handful of Placement Design options (like survey height and display format) will be fully connected to the live survey widget, and any options that can't be used will be cleaned up. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restoring custom pre-ping checks for data clients** — A high-priority effort to bring back the legacy per-client validation that runs when offers are served, so the checks configured for hundreds of active data clients work again on the new platform. (#338)
- **[Feature]** **Bringing back after-success delivery for data clients** — The post-conversion delivery and redirect behavior from the legacy system will be restored for the affected clients so lead delivery continues to work as before. (#327)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging version of New Adsmith Frontend using production-like data that can't be accidentally changed, so the team can verify behavior against real-world data. (#270)
- **[Feature]** **Automatic issue creation from team chats** — A helper that turns action items from team conversations into tracked tasks automatically, cutting out manual copy-and-paste. (#272)

## Campaigns

- **[Feature]** **Bringing the Campaigns module to the new platform** — A critical, high-priority effort to add campaign management (creating and editing campaigns, offer groups, and related settings) that exists in the old system but is currently missing here. (#200)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Fixing styling issues on the Flow form so fields, color pickers, and paired settings display neatly and consistently, matching the other forms in the app. (#152)

## Modals

- **[Feature]** **Making the Modal Design tab actually work** — The Modal Design tab settings (header text, colors, progress bar, and more) currently have no effect on the visitor modal. This work will either connect them so they display, or remove them if the modal is meant to be header-free. (#294)

## Dashboard

- **[Task]** **Confirming dashboard report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy app, so you can trust the numbers you see are accurate. (#271)

## General / Across the App

- **[Bug]** **Clearer result when testing an invalid link** — Instead of quietly sending you to the dashboard, testing an invalid link will show a proper error so you know the test failed. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
