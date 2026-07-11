# Open Issues — Plain-Language Overview

_Last updated 2026-07-11 23:17:55 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Bring back the Campaigns module** — Campaign management from the older admin system isn't in New Adsmith Frontend yet. This adds the ability to view, create, edit, and configure campaigns, including offer groups, offer handling, and marketing partners, so this core workflow is available again. (#200)
- **[Feature]** **Preview unsaved changes on placements and offers** — Today the Preview button only shows the last-saved version. Once done, Preview will reflect the edits you're currently making, so you can check your work before saving. (#292)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several offer options (including modal settings, Display URL, and certain data-client flags) are saved but never actually used by the visitor-facing widget. This fixes or cleanly removes those so what you configure is what visitors get. (#295)
- **[Bug]** **Success pixels aren't firing** — Conversion tracking pixels set on an offer's "Fire on Success" list currently never fire, quietly losing tracking data. This restores them so configured pixels reliably fire on a successful conversion. (#297)
- **[Feature]** **Automatic performance projection for new offers** — Explores an assistant that estimates how a new offer is likely to perform based on your historical offer data, replacing the current informal manual gut-check. It would give you a data-grounded projection at offer intake. (#322)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for every visitor, even ones they should exclude by age, gender, state, ZIP, or device. This makes them respect the same targeting rules as regular offers (or documents the difference if that's intended). (#333)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — Adds a shared editing lock and a save-time check across all entity screens, so if someone else is editing the same record you'll see who has it and be warned before your changes could clobber theirs. (#267)
- **[Feature]** **Searchable activity/audit log** — Records every manual and automated change to your records (who changed what and when) and gives administrators a searchable log, plus a history view on each record — making "who changed this?" easy to answer. (#276)
- **[Feature]** **Clean up controls that don't do anything** — Some admin options (Advertiser Web Presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping settings) are saved but have no effect. These will be removed, hidden, or properly wired up so nothing misleads you. (#296)
- **[Task]** **Users screen gap review vs. the older system** — A review comparing the Users area to the legacy system to identify missing capabilities (like bulk actions, last-login, and two-factor status) and prioritize what to add next. (#80)
- **[Task]** **Decide the future of the file-share page** — The old file-share page has no equivalent yet. This confirms whether anyone still needs it and either gives it a home in the new admin or retires it intentionally. (#328)
- **[Bug]** **Invalid links should show a clear error** — When testing a link that isn't valid, you currently get bounced to the dashboard with no explanation. This will show a clear failure message in the Link Testing screen instead. (#239)

## Surveys

- **[Feature]** **Make every Design tab option actually work** — A full audit to ensure each design/customization option across all screens truly changes what visitors see, with any dead options fixed or removed — so what you set is what you get. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live survey** — A handful of Placement Design tab settings (like survey height and display format) are saved but don't yet affect the widget. This wires them through or removes the ones that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore post-conversion delivery behavior** — The older platform's after-success delivery/redirect steps for certain clients weren't carried over. This ports them so those clients' post-conversion handling works as before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients rely on custom serve-time validation from the old system that currently doesn't run. This brings that validation back so leads are checked as intended before delivery. (#338)

## Behind the Scenes

- **[Task]** **A safe testing environment using production-like data** — Sets up a read-only staging environment so the team can verify behavior against realistic data without any risk of changing live records. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack chats and automatically files or updates work items, reducing manual note-taking after meetings. (#272)

## Reports

- **[Task]** **Confirm dashboard report numbers match the old system** — Testing found dashboard report figures that didn't line up with the legacy app. This investigates where any differences come from and confirms the numbers can be trusted. (#271)

## Flows

- **[Task]** **Fix the visual styling of the Flow form** — Parts of the Flow form currently look unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacking oddly). This cleans up the layout to match the polish of other forms. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — All six Modal Design fields are saved but don't currently affect the visitor-facing modal. This either connects them so they take effect or removes the tab if the modal is meant to be header-less. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
