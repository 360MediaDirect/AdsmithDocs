# Open Issues — Plain-Language Overview

_Last updated 2026-08-19 06:07:24 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some offer settings never reach live ads** — Several options you can set on an offer (including its Modal-tab fields, "Force More Info Visible," Display URL, and a handful of data-handling flags) currently get saved but don't actually take effect where visitors see them. This work makes sure each of those settings either works as expected or is cleared out so it isn't misleading. (#295)
- **[Bug]** **Display vs. AR choice missing on Offer Details** — On the Delivery tab, the DISP and AR columns show as headings but you can't actually pick one for a survey. This restores the ability to set a survey to Display or AR and have it stick, matching the previous app. (#371)
- **[Bug]** **Offer edits aren't showing up in History** — When you change and save an offer, the change isn't being recorded in the offer's History section. This fix makes your edits appear there so you have a reliable record of what changed and when. (#380)
- **[Bug]** **Manually chosen offers not carried over** — On placements set to Manual delivery, the list of hand-picked offers didn't come across to New Adsmith Frontend, so the wrong (or no) offers displayed. This restores your selected offers and their order so live ads match what you configured. (#370)
- **[Feature]** **Preview your unsaved offer and placement changes** — The Preview button will show the edits you're currently making, instead of only the last saved version. You'll be able to check how a change looks before committing to it. (#292)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your own historical offer data, replacing today's manual gut-check review. It would give you a data-driven read on a new offer at intake. (#322)

## Surveys

- **[Feature]** **Design choices consistently applied to surveys** — A full review to make sure every customization option on the Design tab actually shows up in the live survey, across all entity types, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting Placement Design settings** — Several Placement Design-tab options (such as survey height and display format) are saved but not yet reflected in the live survey widget. This finishes wiring them up or removes any that aren't needed, so the settings you see actually do something. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery steps** — Certain after-success behaviors from the previous system (used by specific clients) hadn't been carried over. This brings them back in a flexible, reusable way so those clients keep working as before. This work is nearly complete. (#327)
- **[Feature]** **Restore custom pre-send checks for data clients** — Hundreds of data clients relied on custom validation checks that ran before a lead was sent, and these weren't yet active in the new platform. This high-priority work re-establishes those checks so leads are validated consistently. (#338)

## Dashboard & Reports

- **[Task]** **Confirm dashboard report numbers match the old system** — During testing, some dashboard report figures didn't line up with the previous app. This investigation pins down where any differences come from and confirms the numbers can be trusted. (#271)
- **[Feature]** **Add notes to Placements, Advertisers, and Offers** — Bringing back the ability to attach short, categorized notes (with topic and priority) directly on a record's detail page, plus a recent-notes roll-up on the main Dashboard. You'll be able to jot down updates and see them without reloading the page. (#382)

## Admin & Users

- **[Task]** **Review of the Users area vs. the old app** — A detailed comparison of the Users screens to identify which features from the previous app are still missing (like bulk actions and password entry) so they can be prioritized. This is documentation to guide upcoming work. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings across the app (like the Advertiser Web Presence tab, some user permission toggles, and certain data-client and pre-ping options) are saved but currently have no effect. These will be hidden or removed so the admin screens only show controls that actually work. (#296)

## Behind the Scenes

- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels and automatically logs action items as tracked issues, cutting out manual copy-and-paste when capturing needs from meetings. (#272)
- **[Task]** **Improve the automated testing setup** — Behind-the-scenes maintenance to strengthen the app's automated tests, so problems are caught more reliably before they reach you. (#379)

## Advertisers

- **[Feature]** **Show advertiser website and social links on the detail page** — The Advertiser Details page will display a cluster of quick links (website, social profiles, and a "Search on Google" shortcut) from the Web Presence details already captured in the edit form. You'll be able to jump to an advertiser's online presence in one click. (#383)

## Modals

- **[Feature]** **Make the Modal Design tab actually work** — Every field on the Modal Design tab (header title, subtitle, colors, progress bar, and more) is currently saved but never shown to visitors. This work will either make those settings appear in the visitor modal or remove them so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or awkwardly laid out compared to other forms, with paired fields stacking instead of sitting side by side. This tidies up the form's appearance for a cleaner, more consistent experience. Some of this is already done. (#152)

## Publishers

- **[Bug]** **Pausing a publisher or property now takes full effect** — A pause wasn't being enforced consistently on one of the ad-serving paths, so paused publishers or properties could still serve. This fix makes pausing reliably stop serving everywhere. (#299)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
