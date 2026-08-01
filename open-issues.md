# Open Issues — Plain-Language Overview

_Last updated 2026-08-01 06:48:01 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Manually selected offers not carried over from the old system** — On placements that use manual offer delivery, the new system was showing the wrong offers because the hand-picked offer list wasn't being brought across. Once fixed, these placements will display the same offers, in the same order, as the legacy app. (#370)
- **[Bug]** **Set surveys to Display or AR on the Offer Delivery tab** — The DISP and AR columns currently show as headers with no way to actually choose one. This restores the selectable controls so you can assign a survey's delivery mode and have it save, matching the old app. (#371)
- **[Bug]** **Offer edits now show up in History** — Right now, changing an offer doesn't always add an entry to its History section, so there's no record of the change. This fix ensures every real edit is logged so you can see who changed what. (#380)
- **[Bug]** **Saved offer options that never reached the live experience** — A number of offer settings were being saved but silently dropped before they could affect what visitors see. This work makes each of those settings either actually take effect or be cleanly removed so nothing is misleading. (#295)
- **[Feature]** **Preview unsaved changes on placements and offers** — Today the Preview button only shows the last saved version, so you have to save before you can check an edit. This upgrade lets Preview reflect your current, in-progress changes without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory effort to estimate how a new offer is likely to perform, based on your own historical offer data, replacing a manual human gut-check. It would give a data-driven read on expected performance at intake. (#322)

## Surveys

- **[Feature]** **Make every design option actually change the survey** — A thorough review to confirm that each customization on the Design tab genuinely shows up in the live survey, across all entities. Any option that doesn't do anything will be wired up or removed, so what you set is what you get. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live widget** — Several Placement Design-tab settings (like iFrame height and display format) are saved but not yet reflected in the visitor experience. This completes the connection so those settings take effect, or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Bring over post-conversion delivery steps for clients** — Certain after-success behaviors from the legacy system (what happens right after a conversion) hadn't been carried into the new platform. This adds a flexible, configurable version so those client behaviors work again. (#327)
- **[Feature]** **Restore custom pre-check validation for data clients** — Hundreds of data clients relied on legacy custom checks that run before a lead is passed along, and these currently don't run on the new platform. This high-priority work reconnects those checks so lead validation behaves consistently. (#338)

## General / Across the App

- **[Feature]** **Remove admin controls that don't do anything** — Several settings across the app (an Advertiser Web Presence tab, some user permission toggles, and a few data-client and pre-ping options) are saved but never actually used, which is misleading. They'll be hidden or removed so controls you see reflect real behavior. (#296)
- **[Task]** **Users area: comparing the old and new experience** — A detailed review of the Users screens versus the legacy version to identify what's missing (such as bulk role changes, last-login info, and 2FA status) and prioritize what to add. This guides bringing the new Users area up to full parity. (#80)

## Modals

- **[Feature]** **Make the Modal Design tab work — or retire it** — The entire Modal Design tab (header text, colors, progress bar, and more) is saved but currently has no effect on the visitor modal. This work either makes those settings actually display or removes the tab so it isn't misleading. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or broken — plain textareas, unstyled color pickers, and paired fields stacking vertically instead of side by side. This cleanup brings the form in line with the polished look of the Placement and Modal forms. (#152)

## Publishers

- **[Bug]** **Pausing a publisher or property now reliably takes effect** — A behind-the-scenes check meant that pausing a publisher or property wasn't always enforced on one of the delivery paths. This fix ensures a paused publisher or property is consistently blocked everywhere. (#299)

## Reports

- **[Task]** **Investigate why dashboard report numbers differ from the legacy system** — During testing, some dashboard figures didn't match the old app, making it hard to trust the numbers. This investigation pins down where the difference comes from and confirms the reports are accurate. (#271)

## Behind the Scenes

- **[Feature]** **Turn Slack conversations into tracked work items automatically** — A helper that reads designated Slack channels, spots action items, and files them as tracked issues — cutting out manual copy-and-paste. This speeds up how quickly requests and fixes get captured. (#272)
- **[Task]** **Strengthen automated testing of the admin screens** — A review of the automated test suite found gaps, including tests that silently skipped and tests not running automatically. Addressing these makes the safety net more reliable, catching problems before they reach you. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
