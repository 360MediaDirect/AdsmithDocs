# Open Issues — Plain-Language Overview

_Last updated 2026-07-29 06:51:31 UTC · 17 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Manually selected offers aren't carrying over from the old system** — On placements set to show a hand-picked offer list, the new "Selected Offers" panel is coming up empty, so visitors see the wrong offers. This fix ensures your chosen offers—and their order—match what you set in the legacy app. (#370)
- **[Bug]** **Missing Display/AR controls on the Offer Details Delivery tab** — The Display and AR columns show as headers but have no buttons to actually assign a survey to Display or AR. This restores those controls so you can set a survey's delivery mode without going back to the old app. (#371)
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of options you can set on an offer (including the Modal tab fields, Display URL, and several data delivery flags) are being dropped before they reach visitors. This work makes sure every saved option either takes effect or is cleaned up so it isn't misleading. (#295)
- **[Feature]** **Preview your unsaved offer and placement edits** — The Preview button will show the changes you're currently working on, instead of only the last saved version—so you can check your edits before committing them. (#292)
- **[Feature]** **Performance projections for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your own historical offer data, giving you a data-driven gut-check at intake. (#322)

## Surveys

- **[Feature]** **Make sure every design option actually changes the survey** — A full review to confirm that each customization you set on the Design tab is reflected in what visitors see, with any options that do nothing either fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Settings like survey height, display format, and skip/more-info options will properly take effect in the survey widget, so what you configure is what visitors experience. (#293)

## Data Clients

- **[Feature]** **Bring back after-conversion delivery behaviors** — Post-conversion redirect and delivery steps that existed in the old system are being rebuilt in the new platform, so affected clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-check logic for data clients** — Hundreds of data clients rely on custom validation that runs before a lead is delivered; this high-priority work rebuilds that behavior so those checks run again in the new platform. (#338)

## General / Across the App

- **[Task]** **Review of the Users area against the old system** — A documentation effort comparing the old and new Users screens to spot missing features (like bulk role changes and last-login info) so the team can prioritize what to add. (#80)
- **[Feature]** **Remove settings that don't actually do anything** — Several admin controls (the Advertiser Web Presence tab, certain user permission toggles, and a few data-client and pre-ping options) currently save but have no effect. They'll be hidden or removed to avoid confusion—or scheduled to be properly built. (#296)

## Modals

- **[Feature]** **Make the Modal Design tab work—or remove it** — Every field on the Modal Design tab currently saves but never appears in the visitor modal. This work will either wire those header and progress-bar options through to visitors or remove the tab so it isn't misleading. (#294)

## Publishers

- **[Bug]** **Pausing a publisher or property isn't fully enforced** — Because of a mismatch in how the paused state is checked, one of the paths that serves content wasn't honoring the pause. This fix ensures a paused publisher or property is reliably blocked everywhere. (#299)

## Flows

- **[Task]** **Fix unstyled areas of the Flow form** — Parts of the Flow form show plain, unstyled boxes and stacked fields that should sit side-by-side. This tidies up the layout so it matches the polished look of the Placement and Modal forms. (#152)

## Reports

- **[Task]** **Investigate why dashboard report numbers differ from the old system** — A review to pin down where report totals diverge between the legacy and new platforms, so you can trust that the numbers on the Dashboard match. (#271)

## Behind the Scenes

- **[Feature]** **Automatic issue creation from team conversations** — An internal helper that turns action items from team chats into tracked work items, reducing manual copy-and-paste. No visible change in the product. (#272)
- **[Task]** **Improvements to automated testing** — Behind-the-scenes work to make the app's automated quality checks more reliable and actually run on every update, helping catch problems earlier. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
