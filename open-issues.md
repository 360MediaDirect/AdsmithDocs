# Open Issues — Plain-Language Overview

_Last updated 2026-07-09 15:02:07 UTC · 24 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record to edit it, others will see a clear "locked by {name}" notice, and the system will warn you if a record changed while you had it open — so nobody's work gets silently wiped out. (#267)
- **[Feature]** **New searchable Audit Log** — Administrators will get a history of every change made across the product (who changed what, when, and whether it was a person or an automated job), searchable by record, user, action, and date, with a history view right on each record. (#276)
- **[Feature]** **Remove admin controls that don't actually do anything** — Several settings that look active but have no effect (some Advertiser Web Presence fields, certain user-permission toggles, and a few Data Client and Pre-Ping options) will be hidden or removed so the screens only show controls that truly work. (#296)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent yet; we're confirming whether anyone still uses it before either rebuilding it or officially retiring it. (#328)
- **[Bug]** **Invalid links in Link Testing should show an error, not the Dashboard** — When you test a bad link, you'll get a clear failure message instead of being unexpectedly sent back to the Dashboard. (#239)

## Offers

- **[Bug]** **Saved offer settings that never reach the live page** — Several saved offer options (including Modal-tab settings, Display URL, and "Force More Info Visible") currently get dropped before they reach visitors. We'll make sure each saved setting either shows up live or is clearly documented, so what you save is what appears. A bug fix. (#295)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for everyone, even visitors they should exclude by age, gender, state, zip, or device. This high-priority fix will make them respect the same targeting rules as regular offers. (#333)
- **[Feature]** **Preview offers and placements with your unsaved changes** — The Preview button will show the edits you've made but haven't saved yet, so you can check your work without having to save first. (#292)
- **[Feature]** **Automatic performance projection for new offers** — Instead of a manual gut-check, new offers could be scored against your historical offer data to estimate how they're likely to perform. This is exploratory work with no set deadline. (#322)

## Surveys

- **[Feature]** **Make sure every design option actually changes the survey** — We're reviewing all customization options across every screen to confirm each one truly affects what visitors see, fixing or removing any that don't do anything. (#288)
- **[Bug]** **Voucher code and info links missing from live surveys** — For affected clients, the voucher code line and the privacy/terms/details links are set up in the admin but aren't showing on the live survey page. This high-priority fix restores them, matching the old app. (#291)
- **[Feature]** **Finish connecting Placement Design settings to the live survey** — A handful of Placement design options (like iFrame height and display format) are saved but not yet reflected on the survey. Each will either be wired up so it works or removed if unused. (#293)

## Behind the Scenes

- **[Task]** **Read-only staging environment for safe testing** — A separate testing environment mirroring real data will let the team verify the product against production-like data without any risk of changing live records. (#270)
- **[Feature]** **Turn Slack conversations into tracked to-do items automatically** — A helper that reads designated Slack channels and files action items for the team automatically, cutting out manual copy-and-paste. (#272)
- **[Task]** **Consistent look for alert and banner colors** — Warning, info, success, and error banners will use one shared set of color definitions so they look identical on every screen instead of drifting slightly page to page. (#341)

## Pre-Pings

- **[Feature]** **Run display-trigger pre-ping checks at the right moment** — Offers set to check with the advertiser before being shown will now perform that live check and hide the offer if it's rejected, matching how the old system worked. High priority. (#337)
- **[Feature]** **Bring back per-client custom pre-ping checks** — Hundreds of data clients relied on custom validation checks in the old app that aren't running on the new platform yet. This work restores those checks so leads are validated correctly before delivery. High priority. (#338)

## Data Clients

- **[Feature]** **Restore after-success delivery behavior** — The post-conversion delivery and redirect steps from the old app (used by bperx and rwdb clients) will be rebuilt as a reusable setting so those clients keep working after a lead succeeds. (#327)

## Reports

- **[Task]** **Confirm report numbers match the old system** — We're investigating why some dashboard report figures differed from the legacy app and pinning down the cause, so you can trust the numbers match. (#271)

## Placements

- **[Feature]** **Fix zeros in historical placement reports** — Offer impressions weren't being recorded in past placement reports, showing 0. This adds that figure so historical reports show real numbers. (#339)

## Flows

- **[Task]** **Fix the appearance of the Flow form** — Parts of the Flow form currently look unstyled or broken (plain text boxes, misaligned color pickers, fields stacking instead of sitting side by side). This cleans up the layout to match the rest of the app. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — The Modal Design tab's header and progress-bar settings currently have no effect on the visitor modal. Each will either be connected so it works or removed if the modal is meant to be header-less. (#294)

## Users

- **[Task]** **Review what the new Users area still needs** — A side-by-side comparison of the old and new Users screens to catch missing capabilities (like bulk actions, login/2FA info, and password setup) and prioritize what to add. A documentation and planning effort. (#80)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — Campaign management from the old admin isn't in the new platform yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups. A critical, high-priority feature. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: e97c0c87fd1c264309b547c86ecde9d1b7abd3cebd9c6dc642ac728d6283da48 -->
