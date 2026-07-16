# Open Issues — Plain-Language Overview

_Last updated 2026-07-16 09:40:38 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — When an offer is set up to fire a conversion pixel on success, that pixel currently never runs, so conversions can go unrecorded. This high-priority fix makes configured success pixels fire reliably again. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several options you fill in on an offer (including its Modal-tab fields, Display URL, and certain delivery flags) are saved but don't actually take effect for visitors. This fix makes those settings either work as expected or be removed so the form only shows what really does something. (#295)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Offers that register automatically currently fire for every visitor, even ones outside their age, gender, state, ZIP, or device targeting. This high-priority fix will make those offers respect the same targeting rules as normal offers. (#333)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — The Preview button will show the edits you've made right now, instead of only the last saved version, so you can check a change before committing to it. (#292)
- **[Feature]** **Automatic performance projection for new offers** — A data-driven estimate of how a new offer is likely to perform, based on your historical offers, replacing the old manual gut-check review. (#322)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When someone else is already editing a record, you'll see a clear "locked by" notice, and you'll be warned if a record changed while you had it open — so one person's save can no longer quietly wipe out another's work. (#267)
- **[Feature]** **Clean up controls that don't do anything** — Several settings that currently save but have no effect (Advertiser Web Presence links, certain user permission toggles, and a few Data-Client and Pre-Ping options) will be removed or hidden so the admin screens only show controls that actually work. (#296)
- **[Task]** **Decide the future of the file-share page** — A review of the old file-share page to confirm whether anyone still needs it and, if so, where it should live in New Adsmith Frontend. (#328)
- **[Task]** **Users screen catch-up review** — A comparison of the Users area against the older system to identify which familiar features (like bulk role changes, last-login and two-factor status, and password setup on new users) still need to be added. (#80)

## Surveys

- **[Feature]** **Design tab settings that actually show up in the survey** — A full check to make sure every option on the design tabs is reflected in what visitors see, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings** — Remaining Placement design-tab options (like survey height and display format) will properly carry through to the live survey, and any leftover unused options will be wired up or removed. (#293)
- **[Feature]** **Make the Modal design tab work** — The Modal design tab currently saves header and progress-bar settings that never appear to visitors; this work will either make them display or remove the tab if it isn't needed. (#294)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back post-conversion delivery steps** — Certain "after success" delivery and redirect behaviors from the older system aren't yet available in New Adsmith Frontend. This adds a general, configurable way to run them again for the clients that rely on them. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Many data clients rely on custom validation checks that currently don't run on the new platform. This high-priority, larger effort will bring those serve-time checks back so leads are validated as before. (#338)

## Dashboard

- **[Task]** **Investigate why report numbers don't match the old system** — A close look at Dashboard report figures compared to the legacy system to find where any differences come from and confirm the numbers can be trusted. (#271)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you back on the Dashboard with no explanation; this fix shows a clear failure message instead. (#239)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned compared to other forms. This work continues cleaning up the layout so paired fields and inputs display neatly. (#152)

## Behind the Scenes

- **[Task]** **Safe testing environment using real-world data** — Setting up a read-only environment that mirrors production data so the team can verify behavior without any risk of changing live records. (#270)
- **[Feature]** **Turn Slack discussions into tracked work items automatically** — An internal helper that reads team conversations and files the resulting to-dos automatically, reducing manual copy-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d541cdec2d7ef7e80b16585fe689f12231c8b31406080f26d5421cd3a156890a -->
