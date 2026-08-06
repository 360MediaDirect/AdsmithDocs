# Open Issues — Plain-Language Overview

_Last updated 2026-08-06 06:52:29 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Manually selected offers now carry over from the old system** — On placements set to deliver a hand-picked list of offers, the new system was showing an empty selection and falling back to the wrong offers. This fix makes the new app show the same chosen offers, in the same order, as the legacy app. (#370)
- **[Bug]** **Set surveys to Display or AR from an offer's Delivery tab** — The controls for choosing Display or AR on each survey row went missing, so you couldn't set a survey's delivery mode without going back to the old app. This restores those selectable controls. (#371)
- **[Bug]** **Several saved offer options weren't reaching live pages** — A number of offer settings (including the Modal-tab fields, "Force More Info Visible," Display URL, and some data-client options) were being saved but never actually shown to visitors. Each will be either wired up so it takes effect or removed if it isn't needed. (#295)
- **[Bug]** **Offer edits will show up in History** — Right now, editing an offer doesn't add an entry to its "History" section even though the change saves. This investigates and fixes the gap so your edits are properly recorded. (#380)
- **[Feature]** **Preview unsaved changes on placements and offers** — Today the Preview button shows the last saved version, so you have to save before you can preview a change. This lets Preview reflect your current, unsaved edits. (#292)
- **[Feature]** **Automatic performance estimate for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, replacing the informal manual gut-check. It would give you a data-driven projection at intake. (#322)

## Data Clients

- **[Feature]** **Bring over custom pre-serve validation checks** — A large set of per-client validation rules from the old system (448 clients) don't currently run on the new platform. This ports them so those checks are enforced again. Marked high priority. (#338)
- **[Feature]** **Restore post-conversion delivery steps** — The old "after success" delivery and redirect steps weren't carried over. This adds them back as a reusable, configurable option so post-conversion handling works as before. Nearly complete. (#327)

## Surveys

- **[Feature]** **Make every survey design option actually take effect** — A full check to confirm each customization on the design tab really shows up in the live survey view, across all entities, with any unused options fixed or removed. (#288)
- **[Feature]** **Finish connecting placement survey design settings** — Settings like survey height and display format are saved but not yet applied. This makes them (and a few others) take effect in the live widget, or removes any that aren't needed. (#293)

## Dashboard & Reports

- **[Feature]** **Add and view Notes on Placement, Advertiser, and Offer dashboards** — Restores the ability to attach short, categorized notes (with topic and priority) to these records, plus a recent-notes roll-up on the main Dashboard — with notes appearing instantly without a page reload. (#382)
- **[Task]** **Investigating why some dashboard report numbers differ from the old system** — During testing, certain report figures didn't line up with the legacy app. This work pins down where the difference comes from and either fixes it or confirms the numbers are correct. (#271)

## Admin & Users

- **[Task]** **Reviewing the Users area against the old system** — A side-by-side review of the old and new Users screens to see which features still need to be brought over (such as bulk role changes, last-login and 2FA status, and the password field). This is a planning/analysis document. (#80)
- **[Feature]** **Removing controls that don't do anything** — Some admin settings (the Advertiser Web Presence fields, a couple of user-permission toggles, and a few data-client and pre-ping options) are saved but have no effect, which can be misleading. These will be hidden or removed, or scheduled to be properly built. (#296)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned compared with other forms (plain text boxes, unstyled color pickers, fields stacked instead of side-by-side). This brings its appearance in line with the rest of the app. Partly done. (#152)

## Publishers

- **[Bug]** **Pausing a publisher or property will be fully enforced** — One of the checks that should block a paused publisher or property wasn't working, so enforcement was inconsistent. This makes pausing take effect reliably. (#299)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — The entire Design tab for modals (header title, subtitle, colors, progress bar) is saved but never shown to visitors. These fields will either be built into the visitor modal or removed from the form. (#294)

## Advertisers

- **[Feature]** **Show Web Presence links on the Advertiser detail page** — The website, social profiles, and a "Search on Google" shortcut are captured in the edit form but never displayed. This adds the icon links to the detail page header, shown only when a value exists, opening safely in a new tab. (#383)

## Behind the Scenes

- **[Feature]** **A Slack helper that turns conversations into tracked work items** — An internal tool to automatically capture action items from Slack and file them, reducing manual copy-and-paste. No direct effect on the product screens. (#272)
- **[Task]** **Improving the automated testing setup** — An internal review of the app's automated tests found gaps (some tests silently skipped, tests not run automatically) that are being addressed to make future releases more reliable. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
