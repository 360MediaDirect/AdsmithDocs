# Open Issues — Plain-Language Overview

_Last updated 2026-08-11 06:16:51 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes before saving** — On placement and offer edit pages, the Preview button will show exactly what you've just typed in, instead of only showing the last saved version. That means you can check a change before committing to it. (#292)
- **[Bug]** **Some saved offer options aren't reaching live ads** — A number of offer settings you fill in (including several Modal-tab fields and the Display URL) are being saved but never actually used on live surfaces. This fix makes sure the options you set take effect—or are cleanly removed if they aren't needed. (#295)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory feature to estimate how a new offer is likely to perform, based on your own historical offer data, as a decision aid at intake time. This would replace the current informal manual gut-check review. (#322)
- **[Bug]** **Manually selected offers weren't carried over from the old system** — On Manual-delivery placements, the "Selected Offers" list was coming up empty in New Adsmith Frontend, causing the wrong ads to display. This fix restores your chosen offers and their order so they match the legacy app. (#370)
- **[Bug]** **Restore Display/AR controls on offer delivery** — On the Offer Details Delivery tab, the buttons to set a survey to Display or AR went missing. This fix brings them back so you can configure survey delivery mode without switching to the old app. (#371)
- **[Bug]** **Offer edits should show up in History** — Right now, editing an offer doesn't add an entry to its History section. This fix ensures your changes are recorded so there's a clear trail of who changed what and when. (#380)

## General / Across the App

- **[Task]** **Closing the gap with the legacy Users area** — A review comparing the old Users management with the new one, so missing pieces (like bulk actions, last-login info, and other details) can be prioritized and brought over. (#80)
- **[Feature]** **Removing buttons and settings that don't do anything** — Some admin controls (certain Advertiser web-presence fields, a couple of user permission toggles, and a few data-client/pre-ping options) are shown but have no effect. These will be hidden or removed so the screens only offer choices that actually work. (#296)

## Surveys

- **[Feature]** **Make sure every survey design option actually works** — A full check across all entities to confirm that each customization option you set on a Design tab really shows up in the live survey, with any dead options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Several Placement Design-tab settings (like survey height and display format) are saved but not yet reflected in what visitors see. This work wires them through so they take effect. (#293)

## Dashboard

- **[Task]** **Confirming dashboard report numbers match the old system** — An investigation into why some dashboard report figures didn't line up with the legacy app, so we can pinpoint the cause and confirm the numbers you see are accurate. (#271)
- **[Feature]** **Add and view Notes on Placements, Advertisers, and Offers** — Bringing back the ability to attach short, categorized notes to an object from its detail dashboard, plus a recent-notes roll-up on the main Dashboard—matching the legacy app, with the note appearing right away without a page reload. (#382)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behaviors** — Some after-success delivery/redirect steps from the old platform weren't carried over. This work brings them back for the affected clients so post-conversion handling works as before. (#327)
- **[Feature]** **Restore custom pre-delivery checks for data clients** — A large set of data clients relied on custom serve-time validation from the old system that isn't yet running here. This high-priority work reconnects those checks so delivery behaves consistently with the legacy app. (#338)

## Modals

- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — All six Modal Design-tab fields are currently saved but never shown to visitors. This work will either display them in the visitor modal or remove the tab so it isn't misleading. (#294)

## Advertisers

- **[Feature]** **Show Web Presence links on the Advertiser detail page** — The advertiser's website, social profiles, and a "Search on Google" shortcut are captured in the edit form but not displayed. This adds that cluster of icon links to the detail page header, matching the legacy app. (#383)

## Flows

- **[Task]** **Tidy up the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other forms (plain text boxes, unstyled color pickers, fields stacking oddly). This work brings its look in line with the Placement and Modal forms. (#152)

## Publishers

- **[Bug]** **Pausing a publisher or property should reliably stop serving** — A faulty pause check meant pausing didn't always take effect on one of the serving paths. This fix ensures a paused publisher or property is consistently blocked. (#299)

## Behind the Scenes

- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels and automatically files action items as tracked issues, cutting out manual copy-paste. No direct effect on the product screens. (#272)
- **[Task]** **Strengthening our automated testing** — Findings from a review of the app's automated test coverage, aimed at making tests more reliable and actually catching problems. This is internal quality work with no visible change to the screens. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
