# Open Issues — Plain-Language Overview

_Last updated 2026-07-16 11:32:06 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers are saved in a format the system can't read, so they silently never fire and conversions go untracked. This high-priority fix makes configured success pixels fire reliably so attribution and revenue signals aren't lost. (#297)
- **[Bug]** **Some offer settings never reach the live experience** — A number of saved offer options (including modal fields, Display URL, and several data-client flags) are being dropped before they reach visitors, so they have no effect. This fix ensures each option is either honored on the live offer or cleanly removed from the form. (#295)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers can fire for visitors who should be excluded by age, gender, state, ZIP, or device targeting. This high-priority fix will make these offers respect the same targeting rules as regular offers (or document any intended difference). (#333)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — Today the Preview button shows the last saved version of a placement or offer, so you must save before you can see your edits. Once done, Preview will reflect your current in-progress changes without forcing a save first. (#292)
- **[Feature]** **Predict how a new offer will perform** — A new tool will estimate expected performance for an incoming offer based on your historical offer data, replacing the informal manual gut-check. It's meant as a helpful decision aid at offer intake, not a guarantee. (#322)

## Admin Area

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record for editing, others will see it as locked with a note about who has it open, and the system will warn you if a record changed while you had it open. This protects against accidentally wiping out a colleague's changes. (#267)
- **[Feature]** **Clean up settings that don't do anything** — Several admin controls (Advertiser Web Presence fields, some user permission toggles, and a few Data-Client and Pre-Ping options) currently save but have no effect. These will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Review of the Users area against the old system** — A detailed comparison of the old Users management against New Adsmith Frontend to spot missing features (like bulk role changes and login/2FA details) and prioritize what to add. This documentation guides bringing the Users area up to parity. (#80)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back post-conversion delivery scripts** — The old system's after-success delivery/redirect behavior for certain clients wasn't carried over. This work re-adds that capability in a reusable, configurable way so those clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients relied on custom serve-time validation from the old system that currently doesn't run. This high-priority, larger effort will bring that validation back so leads are correctly checked before delivery. (#338)

## Surveys

- **[Feature]** **Make sure survey design options actually show up** — Customizations set on the Design tab aren't always reflected in the survey visitors see. This work checks every design option end-to-end so what you configure is what visitors get, with any unused options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — A handful of Placement Design-tab settings (like survey height and display format) don't yet affect the live survey widget. Each will be wired through so it works, or removed from the form if it's not needed. (#293)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The Modal Design tab's header and progress-bar settings currently save but never appear in the modal visitors see. These will either be connected so they take effect or removed so the tab isn't misleading. (#294)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of the app connected to production-like data, locked to read-only so testing can't change real records. This gives the team a realistic place to verify changes before they go live. (#270)
- **[Feature]** **Automatically turn Slack discussions into tracked tasks** — A helper that reads designated Slack conversations and files the action items as tracked issues, cutting out manual copying. It de-duplicates against existing items and posts back links to what it created. (#272)

## Flows

- **[Task]** **Tidy up the appearance of the Flow form** — Parts of the Flow form currently look unstyled or misaligned, with fields stacking oddly instead of sitting side by side. This work brings the Flow form's look in line with the Placement and Modal forms. (#152)

## Dashboard & Reports

- **[Task]** **Investigate report numbers that don't match the old system** — During testing, some dashboard report totals didn't line up with the legacy app. This investigation compares the two over a fixed date range to find where the difference comes from and either fix it or confirm the numbers are correct. (#271)

## General / Across the App

- **[Bug]** **Testing an invalid link now shows a clear error** — When you test a bad link, you're currently sent to the dashboard with no explanation. This fix makes Link Testing show a clear failure message instead, so you know the link didn't work. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d541cdec2d7ef7e80b16585fe689f12231c8b31406080f26d5421cd3a156890a -->
