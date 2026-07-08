# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 07:47:59 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Survey

- **[Bug]** **Most survey styling settings don't change the live survey** — Right now nearly all of the Design-tab options (colors, buttons, header, legal text) are saved but have no effect on what visitors actually see. This fix makes those settings take hold so the survey looks the way you set it up. (#290)
- **[Feature]** **Make sure every Design-tab option reaches the live survey** — A full check that each customization you set on a survey is carried all the way through to what visitors see, with no dead settings left behind. (#288)
- **[Bug]** **Voucher code and info links missing on the live survey** — For affected clients, the voucher code line and the privacy/terms/details links appear in the old app but not the new one. This restores them so visitors see the same content and required legal links. (#291)
- **[Feature]** **Finish connecting the last few survey Design settings** — A handful of placement design settings (such as survey height and display format) still don't take effect. This wires up the remaining ones or removes any that aren't used. (#293)

## Offers

- **[Feature]** **Preview offers and placements with your unsaved changes** — Today the Preview button only shows the last saved version. Soon it will reflect the edits you're making right now, so you can check your work before saving. (#292)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several offer options are saved but quietly dropped before they take effect (including modal fields and a few delivery flags). This ensures each saved option either works or is cleaned up so it isn't misleading. (#295)
- **[Task]** **Auto-register offers currently ignore visitor targeting** — Auto-register offers can fire for visitors they should exclude by age, gender, state, ZIP, or device. This confirms the correct behavior and makes those offers respect targeting rules. (#333)
- **[Feature]** **Automatic performance projection for new offers** — Instead of a manual gut-check, new offers could get a data-driven estimate of likely performance based on your historical offer data. An exploratory decision aid at intake time. (#322)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — If someone else is editing the same record, you'll see a clear notice and be protected from accidentally wiping out their changes. Works across all the main entity screens. (#267)
- **[Feature]** **Remove controls that don't actually do anything** — Some admin options look functional but have no real effect (for example, the Advertiser Web Presence fields and certain user-permission toggles). These will be hidden or removed so the interface only shows settings that work. (#296)
- **[Bug]** **Testing an invalid link should show an error, not the dashboard** — In Link Testing, entering a bad link currently bounces you to the dashboard. This will instead show a clear failure message so you know the link didn't pass. (#239)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent yet. This confirms whether anyone still needs it and either brings it forward or retires it for good. (#328)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a test copy of the product against production-like data so changes can be verified without any risk to live information. (#270)
- **[Feature]** **Turn team conversations into tracked work automatically** — A helper that reads designated Slack discussions and files the action items as tracked tasks, cutting out manual copy-and-paste. (#272)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — A high-priority effort to add Campaigns to New Adsmith Frontend so you can view, create, edit, and configure campaigns and offer groups just like in the legacy system. (#200)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — All six fields on the Modal Design tab are currently saved but have no effect on what visitors see. This either wires them up so they work or removes them to avoid confusion. (#294)

## Pre-Pings

- **[Feature]** **Restore the legacy pre-ping behavior** — A high-priority gap: the older per-client pre-ping check isn't available in the new platform. This ports it over (or confirms the new pre-ping fully covers it) so any offer relying on it keeps working. (#330)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behaviors** — Certain after-conversion delivery and redirect steps from the legacy system haven't been carried over yet. This maps each one to the new platform or documents it as retired. (#327)

## Dashboard

- **[Task]** **Investigate why report numbers don't match the legacy system** — Testers noticed dashboard report figures differing from the old app. This compares the two over a fixed date range, pinpoints the cause, and either fixes it or confirms the numbers are correct. (#271)

## Flows

- **[Task]** **Fix the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned compared with other forms (plain textareas, unstyled color pickers, fields stacking oddly). This cleans up the layout so it matches the rest of the app. (#152)

## Users

- **[Task]** **Compare the old and new Users screens to close gaps** — A review of what the legacy Users area offered versus the new one, highlighting missing pieces like bulk actions, extra filters, and login/security details so they can be prioritized. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: db2e2e32afdf249c2931b9305c5b4e9f6e133e4b3e0fdf0fc98b37cd3f75c917 -->
