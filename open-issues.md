# Open Issues — Plain-Language Overview

_Last updated 2026-07-30 06:50:13 UTC · 17 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers & Placements

- **[Feature]** **Preview unsaved changes on placements and offers** — When editing a placement or offer, the Preview button will show your current in-progress changes instead of only the last saved version, so you can check your work before saving. (#292)
- **[Bug]** **Some saved offer options never reach the live experience** — Certain offer settings (including modal fields, "Force More Info Visible," Display URL, and several data-client options) are saved but don't actually appear where visitors see them. This fix ensures each option either works end-to-end or is cleanly removed so nothing is misleading. (#295)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, giving Kurt a data-driven gut-check at intake in place of the retired manual review. (#322)
- **[Bug]** **Manually selected offers not carried over from the legacy system** — On Manual-delivery placements, the new app's "Selected Offers" list is coming up empty, so the wrong offers display. This fix migrates your chosen offers and their order correctly so both systems show the same thing. (#370)
- **[Bug]** **Missing Display/AR controls on the Offer Delivery tab** — The DISP and AR columns appear but currently offer no way to actually assign a survey to Display or AR. This restores the selectable controls so you can set a survey's delivery mode without going back to the legacy app. (#371)

## Surveys

- **[Feature]** **Design-tab customizations fully reflected in the survey** — A thorough check across all entities to make sure every design and form option you set actually shows up in the live survey, with any options that do nothing either fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live widget** — Several Placement design options (such as iFrame Height, Display Format, and skip/more-info behavior) aren't yet reflected where visitors see them. This wires them through so your choices take effect, or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — Bringing over the legacy "after success" handling for data clients so post-conversion redirects and delivery scripts work as they did before. Nearly complete. (#327)
- **[Feature]** **Restore custom pre-ping validation for data clients** — A large group of data clients relied on custom pre-serve validation that currently doesn't run on the new platform. This high-priority work reconnects that validation so leads are checked correctly at serve time. (#338)

## Admin Area

- **[Task]** **Review of the Users area against the legacy system** — A detailed comparison identifying which Users features still need to be brought over (like bulk actions, last-login and 2FA visibility) so the new Users screens match what you're used to. (#80)
- **[Feature]** **Remove admin settings that don't do anything** — Several controls across Advertisers (Web Presence), user permissions, Data Clients, and Pre-Ping are saved but have no effect. Hiding or removing them prevents confusion and false expectations about what they control. (#296)

## Behind the Scenes

- **[Feature]** **Slack-to-issue automation** — A helper that turns action items from Slack conversations into tracked work items automatically, reducing manual copy-and-paste when logging follow-ups. (#272)
- **[Task]** **Improvements to automated testing** — Behind-the-scenes fixes to the automated test suite so it runs reliably and catches problems before they reach you. No visible change to the product itself. (#379)

## Modals

- **[Feature]** **Make the Modal design settings actually work** — The Modal Design tab's header and progress-bar options currently don't appear in the visitor-facing modal. This connects them so your settings show up, or removes the tab if it isn't needed. (#294)

## Publishers

- **[Bug]** **Pausing a publisher or property now takes effect consistently** — A pause wasn't being fully enforced on one of the serving paths. This fix ensures a paused publisher or property is reliably blocked everywhere. (#299)

## Flows

- **[Task]** **Fix visual styling issues on the Flow form** — Parts of the Flow form look unstyled or misaligned (plain textareas, unstyled color pickers, fields stacking instead of sitting side-by-side). This tidies up the form so it matches the polished look of the Placement and Modal forms. (#152)

## Dashboard & Reports

- **[Task]** **Confirm report numbers match the legacy system** — Investigating why some dashboard report figures differed from the old app, so you can trust that the numbers you see are accurate and consistent. (#271)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
