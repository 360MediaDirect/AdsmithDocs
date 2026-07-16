# Open Issues — Plain-Language Overview

_Last updated 2026-07-16 07:41:33 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Feature]** **Preview unsaved changes on placements and offers** — When editing a placement or offer, the Preview will show your current in-progress changes instead of only the last saved version, so you can check your work before saving. (#292)
- **[Bug]** **Some saved offer settings never reach the live offer** — Several options you set on an offer (including modal-tab fields and a few delivery flags) are being dropped and never take effect; this fix makes those saved settings actually apply. (#295)
- **[Bug]** **Conversion "success" pixels aren't firing** — Pixels configured to fire when an offer converts are silently not firing, which means lost tracking. A high-priority fix will restore reliable conversion tracking. (#297)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, new offers could get a data-driven estimate of likely performance based on your historical offer results, giving a helpful preview at intake time. (#322)
- **[Task]** **Auto-register offers currently ignore visitor targeting** — Auto-register offers can fire for visitors they should exclude (by age, gender, state, zip, or device). This high-priority fix ensures they respect the same targeting rules as regular offers. (#333)

## General / Across the App
- **[Feature]** **Protection against two people overwriting each other** — If someone else is editing the same record you have open, you'll see a clear "locked by" notice and be warned before anyone's changes get silently overwritten. (#267)
- **[Feature]** **Remove settings that don't actually do anything** — Several controls that quietly have no effect (Advertiser Web Presence fields, certain user permissions, and some data-client and pre-ping options) will be hidden or removed so the admin only shows settings that truly work. (#296)
- **[Task]** **Decide the future of the legacy file-share page** — A review to confirm whether the old file-share page is still needed and either bring it forward or formally retire it. (#328)
- **[Task]** **Users screen feature review** — A documented comparison of the Users area against the older system to identify which user-management features still need to be added. (#80)
- **[Bug]** **Testing an invalid link should show an error, not the Dashboard** — When you test a bad link, you're currently sent to the Dashboard with no explanation. This fix will show a clear failure message right in Link Testing. (#239)

## Surveys
- **[Feature]** **Design choices fully reflected in the live survey** — Every customization on the Design tab will actually show up in the survey visitors see, plus a wider check across all screens to catch any options that aren't yet connected. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey** — Design-tab settings like survey height and display format will properly take effect in the live survey widget instead of being saved but ignored. (#293)

## Data Clients
- **[Feature]** **Restore after-success delivery behaviors** — Post-conversion delivery and redirect steps from the older system are being brought over so affected data clients keep working as before. (#327)
- **[Feature]** **Bring over custom pre-check validation for data clients** — Hundreds of data clients rely on custom checks that don't yet run on the new platform. This high-priority work restores those checks so they run at the right time again. (#338)

## Behind the Scenes
- **[Task]** **Read-only staging environment for safe testing** — A test environment loaded with realistic data (view-only, so nothing can be changed) to make verification and sign-off more reliable. (#270)
- **[Feature]** **Turn Slack conversations into tracked tasks automatically** — An internal helper that reads designated Slack channels and files action items as tracked issues, cutting out manual copy-paste. (#272)

## Flows
- **[Task]** **Fix visual styling on the Flow form** — Parts of the Flow form currently look unstyled (plain textareas, unstyled color pickers, and fields stacked instead of side-by-side). This tidies up the form's appearance. (#152)

## Modals
- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design tab's settings currently have no effect on the modal visitors see. This work will either connect them so they apply or remove the tab if it isn't needed. (#294)

## Dashboard & Reports
- **[Task]** **Investigate mismatched report numbers** — Some Dashboard report figures didn't match the older system during testing. This investigation will pin down the cause and confirm the numbers are accurate. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d541cdec2d7ef7e80b16585fe689f12231c8b31406080f26d5421cd3a156890a -->
