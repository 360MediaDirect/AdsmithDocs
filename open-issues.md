# Open Issues — Plain-Language Overview

_Last updated 2026-08-22 06:05:28 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes on Offers and Placements** — When editing an offer or placement, the Preview button will show exactly what you're working on right now, including edits you haven't saved yet, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Manually selected offers now show correctly** — On placements set to deliver a hand-picked list of offers, the new platform was showing an empty selection and displaying the wrong offers. This fix makes the new app show the same chosen offers, in the same order, as before. (#370)
- **[Bug]** **Offer settings that weren't reaching the live experience** — Several saved offer options (including the Modal tab fields, Display URL, and certain delivery flags) weren't actually being used when offers were shown to visitors. Each will be properly connected or cleared out so what you set is what runs. (#295)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your own history of past offers, giving the team a data-backed gut-check at intake instead of relying on a manual review. (#322)

## Surveys

- **[Feature]** **Design tab options that truly take effect** — A full check to make sure every look-and-feel option you set on the Design tab actually shows up in the live survey, across all entity screens, with no settings that quietly do nothing. (#288)
- **[Feature]** **Placement survey design settings fully connected** — A handful of Placement Design-tab settings (such as survey height and display format) weren't being applied to the live survey widget. Each will either be made to work or removed so the form only shows options that matter. (#293)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery steps** — Certain "after-success" behaviors that ran once a lead converted weren't carried over to the new platform. These are being rebuilt so affected clients keep working as they did before. (#327)
- **[Feature]** **Restoring custom pre-check validation at serve time** — A large group of data clients relied on custom checks that quietly stopped running on the new platform. This high-priority work reconnects those checks so leads are validated correctly before delivery. (#338)

## Dashboard

- **[Feature]** **Add and view notes on Placements, Advertisers, and Offers** — Bringing back the ability to jot short, categorized notes right on a Placement, Advertiser, or Offer detail page, with a recent-notes roll-up on the main Dashboard. Notes will appear immediately without needing a page reload. (#382)
- **[Task]** **Making dashboard report numbers match the old system** — An investigation into why some dashboard figures differed from the previous system, so the numbers you rely on can be trusted and verified. (#271)

## General / Across the App

- **[Feature]** **Cleaning up controls that don't do anything** — Some admin settings (like the Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) are saved but currently have no effect. These will be removed, hidden, or properly implemented so nothing misleads you. (#296)
- **[Task]** **Bringing the Users area up to full feature parity** — A detailed review comparing the older Users management screen with the new one, guiding work to add missing capabilities like bulk actions, last-login visibility, and more. (#80)

## Behind the Scenes

- **[Feature]** **A Slack helper that turns conversations into tracked work items** — An internal assistant that reads team conversations and logs action items automatically, reducing manual note-keeping. No direct change to the product you use. (#272)
- **[Task]** **Strengthening automated testing** — Behind-the-scenes improvements to the automated checks that guard the Admin area, making them more reliable so issues are caught before they reach you. (#379)

## Modals

- **[Feature]** **Making the Modal Design tab work as expected** — The Modal Design tab's header and progress-bar settings currently don't appear in the visitor-facing modal. These will either be made to display or removed so the form reflects reality. (#294)

## Advertisers

- **[Feature]** **Web Presence links on the Advertiser page** — The website, social profiles, and a "Search on Google" shortcut you enter for an advertiser will finally appear as clickable icons on the Advertiser detail page, instead of being captured but never shown. (#383)

## Publishers

- **[Bug]** **Pausing a publisher or property now fully takes effect** — Pausing wasn't being enforced consistently on one of the serving paths. This fix ensures a paused publisher or property is reliably stopped everywhere. (#299)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly instead of sitting side by side. This tidies up the form so it matches the polished look of the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
