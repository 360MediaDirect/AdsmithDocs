# Open Issues — Plain-Language Overview

_Last updated 2026-08-17 06:08:53 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some offer settings never reach live surfaces** — Several options you save on an offer (including its Modal-tab fields, "Force More Info Visible," Display URL, and some data-delivery flags) aren't currently carried through to what visitors actually see. This fix makes sure the settings you enter are either used everywhere they should be or clearly removed if they do nothing. (#295)
- **[Bug]** **Display/AR controls missing on the Offer Details Delivery tab** — Right now you can't set a survey to Display or AR from the new app because the selectable buttons are missing. Once fixed, you'll be able to assign each survey's delivery mode directly, matching the old app. (#371)
- **[Bug]** **Offer edits aren't showing up in History** — After changing and saving an offer, its "History" section stays empty. This fix ensures every real edit is recorded so you can see who changed what and when. (#380)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, new offers would get an estimated performance outlook based on your own historical offer data. This is an exploratory idea to give a helpful, data-grounded preview at intake. (#322)

## Surveys & Modals

- **[Feature]** **Design choices reliably reflected in the survey** — A full check to make sure every customization option on the Design tab actually shows up in the live survey, with no settings that quietly do nothing. You'll be able to trust that what you configure is what visitors see. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey widget** — A handful of placement design options (like survey height, display format, and skip behavior) are saved but not yet applied. Once done, these settings will take effect, or be removed if they aren't needed. (#293)
- **[Feature]** **Make the Modal Design tab actually work** — Every field on the Modal Design tab (header title, subtext, colors, progress bar) currently has no effect on the visitor's modal. This work will either wire those fields up so they display, or remove the tab if the modal is meant to be header-less. (#294)

## Placements

- **[Feature]** **Preview shows your unsaved changes** — On the placement and offer edit pages, Preview currently shows the last-saved version, so you have to save before you can see edits. This upgrade lets Preview reflect your in-progress changes without saving first. (#292)
- **[Bug]** **Manually selected offers not carried over on some placements** — On Manual-delivery placements, the list of hand-picked offers isn't coming across to the new app, so it shows different (or empty) offers than the old app. This fix ensures your selected offers—and their order—display correctly. (#370)

## Data Clients & Pre-Pings

- **[Feature]** **Restore post-conversion delivery behavior** — Certain after-conversion delivery/redirect steps from the old system weren't carried over. This work brings that behavior back in a flexible, configurable way so affected clients keep working as before. (#327)
- **[Feature]** **Bring over legacy serve-time pre-ping checks (high priority)** — Custom validation checks that hundreds of data clients relied on aren't running on the new platform yet. This restores those checks so client-level validation happens as expected before delivery. (#338)

## Dashboard

- **[Task]** **Confirm report numbers match the old system** — Reviewers noticed dashboard report figures didn't line up with the legacy app. This investigation pins down where the difference comes from and confirms the numbers can be trusted. (#271)
- **[Feature]** **Notes on Placements, Advertisers, and Offers** — Bringing back the ability to add short, categorized notes to a placement, advertiser, or offer from its detail page, plus a recent-notes roll-up on the main Dashboard. Notes will appear right away without a page reload, and existing legacy notes will still be readable. (#382)

## Advertisers

- **[Feature]** **Show an advertiser's web and social links on their detail page** — The website, social profiles, and a "Search on Google" shortcut are captured in the edit form but never displayed. This adds a tidy cluster of icon links to the Advertiser detail header, opening safely in a new tab. (#383)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unfinished—plain textareas, unstyled color pickers and checkboxes, and paired fields stacking instead of sitting side by side. This tidies up the form so it matches the polished look of the other forms. (#152)

## Publishers

- **[Bug]** **Pausing a publisher or property isn't fully enforced** — A paused publisher or property can still slip through on one of the delivery paths because of a faulty check. This fix makes pausing take effect consistently everywhere. (#299)

## General / Across the App

- **[Task]** **Fill the gaps between the old and new Users area** — A detailed comparison of the old Users management against the new one, identifying missing pieces (like bulk actions, password setup, and last-login/2FA details) so the new Users area reaches full parity. (#80)
- **[Feature]** **Remove controls that don't do anything** — Several admin settings (an advertiser's Web Presence fields, some user permission toggles, and a few data-client and pre-ping options) are saved but currently have no effect. These will be hidden or removed so the interface only shows controls that actually work—no more misleading options. (#296)

## Behind the Scenes

- **[Feature]** **Turn Slack conversations into tracked work items automatically** — An internal helper that reads designated Slack channels and files action items as tracked issues, cutting out manual copy-paste. This is a productivity tool for the team and won't change the product screens you use. (#272)
- **[Task]** **Shore up the automated testing setup** — Behind-the-scenes maintenance to make the app's automated checks more reliable and actually run consistently, so problems get caught earlier before they reach you. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
