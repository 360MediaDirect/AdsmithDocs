# Open Issues — Plain-Language Overview

_Last updated 2026-07-11 15:21:43 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Bring back Campaigns management** — You'll be able to create, edit, and manage campaigns and their offer groups directly in New Adsmith Frontend, matching what the old admin panel did. This is a high-priority gap since campaign management can't be done in the new platform today. (#200)
- **[Feature]** **Preview your unsaved edits on Placements and Offers** — When editing a placement or offer, the Preview button will show the changes you're currently making, so you no longer have to save first just to see how an edit looks. (#292)
- **[Bug]** **Some saved offer settings don't reach the live experience** — A fix so that offer options you configure (including modal settings, display URL, and several delivery flags) actually take effect on the live page instead of being quietly dropped. (#295)
- **[Bug]** **Success tracking pixels not firing** — A high-priority fix so the conversion pixels you set to fire on a successful offer actually fire, restoring accurate attribution and revenue tracking. (#297)
- **[Feature]** **Automatic performance estimate for new offers** — Explore giving you a data-driven projection of how a new offer is likely to perform, based on your historical offers, replacing today's informal manual review. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — A fix so auto-registering offers honor age, gender, state, zip, and device targeting rules like regular offers do, instead of firing for visitors they should exclude. (#333)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record you're already editing, they'll see a clear "locked by" notice, and you'll be warned if a record changed while you had it open, so one person's changes can't silently wipe out another's. (#267)
- **[Feature]** **Searchable history of who changed what** — A new Audit Log will record every change made across the app (by people and by automated jobs) with a timestamp, and let administrators search by record, person, action, and date to answer "who changed this and when." (#276)
- **[Feature]** **Clean up controls that don't do anything** — Several settings that currently appear editable but have no effect (Advertiser Web Presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping options) will be removed or hidden, so what you see reflects what actually works. (#296)
- **[Bug]** **Testing an invalid link now shows a clear error** — Instead of quietly sending you to the Dashboard, entering an invalid link in Link Testing will show a proper failure message. (#239)
- **[Task]** **Review of the Users area against the old system** — A behind-the-scenes comparison of user management in New Adsmith Frontend versus the legacy system to catch any missing features (such as bulk actions and login details) before they slip through. (#80)
- **[Task]** **Decide the future of the old File Share page** — A keep-or-retire decision on the legacy file-share page, which has no equivalent in the new platform, so nothing important is lost. (#328)

## Surveys

- **[Feature]** **Make sure every design option actually changes the survey** — A review across all screens to confirm each customization option you set on a Design tab is reflected in what visitors see, with any dead options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Remaining Placement design options (like survey height and display format) will actually take effect in the survey widget, or be removed if they aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — The "after success" delivery and redirect steps from the old system will be brought over to New Adsmith Frontend so active data clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — A high-priority effort to bring over the legacy per-client validation that runs before an offer is served, so the checks hundreds of data clients rely on aren't silently skipped. (#338)

## Modals

- **[Feature]** **Make the Modal Design tab actually work** — The Modal Design settings (header text, colors, progress bar) will either be connected so they show in the visitor modal, or removed if the modal is meant to have no header. (#294)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Continued styling fixes so the Flow form's text boxes, color pickers, checkboxes, and paired fields look consistent with the rest of the app instead of appearing broken or unstyled. (#152)

## Reports

- **[Task]** **Confirm Dashboard report numbers match the old system** — An investigation into why some Dashboard report figures differed from the legacy app, to pin down the cause and confirm the numbers can be trusted. (#271)

## Behind the Scenes

- **[Task]** **Staging environment for safe testing** — Setting up a read-only test environment using a copy of real data, so the team can verify the product against production-like information without any risk of changing live data. (#270)
- **[Feature]** **Automatic issue tracking from team conversations** — An internal helper that turns action items from team chats into tracked work items automatically, reducing manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
