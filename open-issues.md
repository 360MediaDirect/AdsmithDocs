# Open Issues — Plain-Language Overview

_Last updated 2026-08-02 06:51:28 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Saved offer settings not reaching live ads** — Some options you set on an offer (like its Modal settings, Display URL, and certain delivery flags) currently never show up on the live ad. This fix makes sure the choices you save actually take effect where visitors see them. (#295)
- **[Bug]** **Restore Display/AR selection on the Offer Delivery tab** — The DISP and AR columns appear but have no buttons to click, so you can't set a survey to Display or AR. This brings back the selectable controls so you can configure a survey's delivery mode again. (#371)
- **[Bug]** **Offer edits will show up in History** — Right now, changing an offer saves correctly but leaves the History section empty. Once fixed, every edit you make will appear as a recorded change so you can see who changed what and when. (#380)
- **[Bug]** **Manually selected offers now carried over from the legacy app** — On Manual-delivery placements, the new app's "Selected Offers" list is coming up empty, so visitors see the wrong offers. This fix migrates your hand-picked offers and their order so the new app matches the old one. (#370)
- **[Feature]** **Preview shows your unsaved changes** — Today the Preview button on placement and offer edit pages only shows the last-saved version, so you have to save before you can check a change. This upgrade lets Preview reflect the edits you've made right now, without saving first. (#292)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your existing offers and their history, giving you a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Surveys

- **[Feature]** **Design choices that actually change the survey** — We're making sure every option on the Design tab is reflected in the live survey, and reviewing form options across all screens so nothing you set is quietly ignored. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live survey** — Settings like survey height, display format, skip options, and "more info" visibility are being wired through (or removed if unused) so the choices you make on a placement show up for real visitors. (#293)

## Data Clients

- **[Feature]** **High priority: restore custom serve-time checks** — Legacy accounts relied on custom validation that runs when an ad is served, and it doesn't currently run on the new platform. This work brings those checks back so delivery behaves the way each client expects. (#338)
- **[Feature]** **Bring back after-success delivery behavior** — The post-conversion delivery and redirect steps used by some clients weren't carried over. This restores them as a reusable setting so conversions hand off correctly again. (#327)

## Modals

- **[Feature]** **Make the Modal Design tab work (or retire it)** — The Modal Design tab's header title, colors, and progress-bar options currently don't affect what visitors see. We'll either wire them up so they take effect or remove them so the tab isn't misleading. (#294)

## Reports

- **[Task]** **Getting Dashboard report numbers to match the legacy system** — Reviewers noticed dashboard figures didn't line up with the old app. We're comparing the two over a fixed date range to find and fix the cause, so you can trust the numbers match. (#271)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unfinished — plain text boxes, unstyled color pickers, and paired fields stacking instead of sitting side by side. This cleanup brings the Flow form in line with the polished look of the Placement and Modal forms. (#152)

## Publishers

- **[Bug]** **Pausing a publisher or property fully takes effect** — A gap means pausing a publisher or property isn't always enforced everywhere. This fix makes sure a paused publisher or property is consistently stopped from serving. (#299)

## Users

- **[Task]** **Review of missing Users features from the old app** — A side-by-side comparison of the old and new Users screens to catalog what's missing (like bulk actions, last-login and two-factor status, and password entry) so we can prioritize closing those gaps. (#80)

## General / Across the App

- **[Feature]** **Remove settings that don't actually do anything** — Some controls save your input but have no effect, including the Advertiser "Web Presence" tab, a couple of user-permission toggles, and some Data-Client and Pre-Ping options. We're hiding or removing these so the app only shows settings that genuinely work. (#296)

## Behind the Scenes

- **[Feature]** **A helper that turns chat discussions into tracked to-dos** — An internal assistant that reads team conversations and automatically logs action items, reducing manual note-taking. No change to the product you use day to day. (#272)
- **[Task]** **Strengthening our automated testing** — A review of the automated checks that guard the app turned up gaps we're addressing, so future updates are caught before they reach you. Behind-the-scenes quality work. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
