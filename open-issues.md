# Open Issues — Plain-Language Overview

_Last updated 2026-07-16 01:33:24 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on Placements and Offers** — When editing a placement or offer, the Preview button will show your current edits right away, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Some saved offer settings never reach live pages** — Several options you set on an offer (including modal fields, "Force More Info Visible," Display URL, and certain data-client flags) aren't currently carried through to the live experience. This fix ensures each option either works as expected or is cleaned up so it isn't misleading. (#295)
- **[Bug]** **Success pixels aren't firing** — Conversion tracking pixels set under "Pixels to Fire on Success" currently never fire, which means lost tracking with no warning. This high-priority fix makes configured success pixels fire reliably. (#297)
- **[Feature]** **Automatic performance projection for new offers** — Instead of a manual gut-check, new offers could get an automated estimate of likely performance based on your own historical offer data, helping you gauge a new offer at intake. (#322)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for everyone, even visitors who should be excluded by age, gender, state, ZIP, or device targeting. This high-priority fix brings them in line with the targeting rules you set. (#333)

## General / Across the App

- **[Bug]** **Testing an invalid link should show a clear error** — Right now, entering an invalid link during Link Testing quietly sends you to the dashboard. After this fix you'll get a plain error message telling you the link failed. (#239)
- **[Feature]** **Protection against two people editing the same record** — When someone else is already editing a record, you'll see a clear "locked by" notice, and the app will warn you before you can overwrite changes someone made while you had it open. This prevents accidental lost edits across every entity screen. (#267)
- **[Feature]** **Remove admin controls that don't actually do anything** — Several settings currently appear on screens (Advertiser Web Presence fields, some user permission toggles, and a few Data-Client and Pre-Ping options) but have no effect. They'll be removed or hidden so the admin only shows controls that truly work. (#296)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent in New Adsmith Frontend. This is a decision on whether to rebuild it or officially retire it. (#328)

## Surveys

- **[Feature]** **Design-tab settings should show up in the live survey** — Every customization option on the Design tab will be checked end-to-end so what you set actually appears in the survey. This audit covers all entities to catch any option that looks active but isn't. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey** — A handful of Placement Design settings (like survey height and display format) aren't yet reflected in the live survey. This work wires them up—or removes the ones that aren't needed—so no setting is left doing nothing. (#293)

## Data Clients

- **[Feature]** **Bring back post-conversion delivery scripts** — Certain "after success" delivery behaviors from the old platform haven't been carried over. This restores them as a configurable option so affected clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients rely on custom serve-time validation that currently doesn't run on the new platform. This high-priority work reconnects those checks so leads are validated as intended. (#338)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form currently appear unstyled, with plain text boxes, unstyled color pickers, and fields stacking awkwardly instead of sitting side by side. This gives the form a clean, consistent appearance matching the rest of the app. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab actually work** — The entire Modal Design tab (header text, colors, progress bar, and more) currently has no effect on what visitors see. This work will either wire those settings into the visitor modal or remove the tab if it isn't needed. (#294)

## Reports & Dashboard

- **[Task]** **Confirm dashboard numbers match the old system** — Testers noticed dashboard report figures didn't line up with the legacy app. This investigation pins down any differences and confirms the numbers can be trusted. (#271)

## Admin & Users

- **[Task]** **Review the Users area against the old system** — A side-by-side comparison of the old and new Users screens to spot missing pieces (like bulk actions, last-login info, and 2FA status) and prioritize what to add. (#80)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of the app running against prod-like data, locked to read-only so testers can validate against realistic data without any risk of changing it. (#270)
- **[Feature]** **Automatically turn meeting discussions into tracked tasks** — An internal helper that reads team conversations and files them as tracked work items, reducing manual note-taking and follow-up. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d541cdec2d7ef7e80b16585fe689f12231c8b31406080f26d5421cd3a156890a -->
