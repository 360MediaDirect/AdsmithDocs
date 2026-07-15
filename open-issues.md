# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 00:21:22 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes on Placements and Offers** — When editing a placement or offer, the Preview button will show your current in-progress changes instead of only the last saved version, so you can check your work before committing it. (#292)
- **[Bug]** **Some saved offer settings never reach live pages** — A number of offer options you fill in (including modal fields, Display URL, and several data-client settings) currently get dropped before they appear to visitors. This fix makes sure the settings you save actually take effect. (#295)
- **[Bug]** **Success pixels not firing** — A high-priority fix so the "Pixels to Fire on Success" you configure on an offer actually fire on a conversion, restoring accurate tracking that's silently been missing. (#297)
- **[Bug]** **Auto-register offers ignore audience targeting** — A high-priority fix so auto-register offers respect the same age, gender, state, ZIP, and device targeting rules as regular offers, preventing them from showing to visitors who should be excluded. (#333)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical offer data, replacing today's informal manual gut-check with a data-driven projection. (#322)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record to edit it, others will see it's locked and by whom, and you'll be warned if a record changed while you had it open — so no one's changes get silently lost. (#267)
- **[Feature]** **Clean up settings that don't actually do anything** — Several admin controls that look active but have no effect (Advertiser Web Presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping options) will be removed or hidden so the screens only show controls that work. (#296)
- **[Task]** **Decide the future of the old File Share page** — Reviewing whether the legacy file-share page is still used and either bringing it into the new platform or officially retiring it. (#328)

## Surveys

- **[Feature]** **Make sure every design option actually shows in the survey** — A full review to confirm each Design tab customization across all screens is connected end-to-end, so what you set is what visitors see, with no dead options. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live survey** — Settings like iFrame height and display format will properly take effect in the survey widget, and a few partially-connected options will be either fully wired up or removed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery for data clients** — The legacy "after-success" delivery and redirect behavior that some clients rely on is being brought into the new platform so those clients keep working as before. (#327)
- **[Feature]** **Bring over file-based pre-ping checks for data clients** — Custom validation checks that hundreds of data clients depend on currently don't run on the new platform; this work restores those serve-time checks so leads are validated correctly. (#338)

## Dashboard & Reports

- **[Task]** **Confirm report numbers match the old system** — An investigation into why some dashboard report totals differed from the legacy system, so you can trust that the new reports are accurate. (#271)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will show a proper error message instead of quietly sending you to the dashboard, so you get a clear result. (#239)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The Modal Design tab's header and progress-bar settings currently have no effect on what visitors see. They'll either be fully connected so they display, or removed to avoid confusion. (#294)

## Campaigns

- **[Feature]** **Bring the Campaigns module into the new platform** — A high-priority, core feature: the ability to view, create, edit, and configure campaigns and offer groups — matching the legacy admin — is being built into New Adsmith Frontend. (#200)

## Users

- **[Task]** **Reviewing what's missing in the new Users area** — A detailed comparison between the old and new Users screens to catch missing capabilities (like bulk actions, last-login and two-factor status, and password fields) and prioritize what to add. (#80)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Fixing styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields display cleanly and consistently with the other forms. (#152)

## Behind the Scenes

- **[Task]** **Set up a safe testing environment with real-world data** — Standing up a read-only staging environment that mirrors live data, so features can be verified against realistic information without any risk of changing it. (#270)
- **[Feature]** **Turn Slack conversations into tracked to-dos automatically** — A helper that reads designated Slack channels and files action items as work items automatically, cutting out manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f12be1691f4d05be7a51684fc6fe5ab6d4c4751d5a9de6a600395df673d554b3 -->
