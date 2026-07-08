# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 21:25:25 UTC · 23 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Feature]** **Preview shows your unsaved changes** — When editing a placement or offer, the Preview will reflect the edits you've made but not yet saved, so you can check your work before committing it. (#292)
- **[Bug]** **Saved offer options not reaching live pages** — Some options you save on an offer (such as the Display URL and modal-related settings) aren't currently carried through to the live offer. This fix makes sure saved options actually appear where they should. (#295)
- **[Feature]** **Automatic performance projection for new offers** — New offers will get an estimated performance projection based on your historical offer data, replacing the manual gut-check review that's being retired. (#322)
- **[Bug]** **Auto-register offers now respect targeting** — Auto-register offers currently fire for every visitor regardless of age, gender, state, zip, or device targeting. This high-priority fix makes them honor the same targeting rules as regular offers. (#333)

## Admin & Users
- **[Task]** **Review of the Users screen against the old system** — A comparison of the legacy Users management area with the new one to identify and bring across missing capabilities like bulk actions, last-login, and two-factor status. (#80)
- **[Feature]** **Remove settings that don't do anything** — Several admin controls (Advertiser Web Presence fields, certain user permission toggles, and some Data-Client and Pre-Ping options) currently save but have no effect. They'll be hidden or removed so the screen only shows controls that actually work. (#296)
- **[Task]** **Decide the future of the file-share page** — Confirming whether the legacy file-share page is still used and, if so, where it belongs in the new admin — otherwise retiring it. (#328)

## General / Across the App
- **[Bug]** **Invalid link now shows a clear error** — Testing an invalid link currently drops you on the dashboard with no explanation. This fix shows a proper failure message instead. (#239)
- **[Feature]** **Prevent two people overwriting each other's edits** — When two admins open the same record, you'll see a clear "locked by" notice and a warning if it changed while you were working, so no one's changes get silently lost. (#267)
- **[Feature]** **Searchable activity history across the platform** — A new audit log will record who changed what and when — for both manual edits and automated updates — making it easy to trace changes from any entity's detail page. (#276)

## Surveys
- **[Feature]** **Design choices fully applied to the live survey** — A thorough check to make sure every design customization you set actually shows up on the survey visitors see, with nothing left disconnected. (#288)
- **[Feature]** **Finish connecting placement design settings** — A few placement Design-tab settings (like iframe height and display format) don't yet change the live survey. This wires them through so they take effect. (#293)

## Pre-Pings
- **[Feature]** **Live offer check at display time** — Display-trigger pre-pings will actually verify with the advertiser when an offer is shown and hide it if rejected, matching how the legacy system behaved. (#337)
- **[Feature]** **Bring over legacy per-client pre-ping checks** — Custom pre-conversion checks used by hundreds of clients aren't yet running on the new platform. This high-priority work ports them so those validations apply again. (#338)

## Data Clients
- **[Bug]** **Voucher code and info links missing on the survey** — For affected clients, the configured voucher code line and the privacy/terms/details links aren't showing on the live survey even though they're saved. This high-priority fix restores them. (#291)
- **[Feature]** **Restore after-success delivery behavior** — The legacy post-conversion delivery and redirect steps are being brought over so they run correctly on the new platform. (#327)

## Reports
- **[Task]** **Investigate dashboard numbers vs. the legacy system** — Looking into why some dashboard report figures don't match the old system, pinpointing the cause and confirming the numbers can be trusted. (#271)
- **[Feature]** **Fix zero offer impressions in historical placement reports** — Historical placement reports currently show offer impressions as 0. This will populate the real figure so past performance reads correctly. (#339)

## Behind the Scenes
- **[Task]** **Read-only test environment with realistic data** — Setting up a safe, look-but-don't-touch environment that mirrors production data for verification and testing. (#270)
- **[Feature]** **Assistant that turns conversations into tracked tasks** — A helper that reads designated Slack discussions and automatically files them as tracked issues, cutting out manual copy-and-paste. (#272)

## Flows
- **[Task]** **Fix styling on the Flow form** — Parts of the Flow form currently look unstyled or misaligned (text boxes, color pickers, and side-by-side fields). This restores a clean, consistent layout. (#152)

## Campaigns
- **[Feature]** **Add the Campaigns module** — Bringing campaign management to the new platform so you can view, create, and edit campaigns and manage their offer groups, matching the legacy system. This is a high-priority, core feature. (#200)

## Modals
- **[Feature]** **Make the Modal Design tab take effect** — The modal Design-tab settings (header text, colors, progress bar) currently have no effect on what visitors see. They'll either be wired up to work or removed if the modal is meant to have no header. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 46bbd1bcbe54e8b503159e4003f7324c83439148b0efea1c528a5b6e64990cc5 -->
