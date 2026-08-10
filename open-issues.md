# Open Issues — Plain-Language Overview

_Last updated 2026-08-10 06:26:19 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach the live ad** — Several options you set on an offer (including its Modal-tab settings and certain display options) aren't actually being applied when the offer runs. This work makes sure every option you can set either takes effect or is removed so nothing misleads you. (#295)
- **[Bug]** **Hand-picked offer lists weren't carried over** — On placements set to show a manually selected list of offers, the new app was showing the wrong offers or none at all. This fix makes the new app display the same selected offers, in the same order, as before. (#370)
- **[Bug]** **Can't set a survey to Display or AR on the Delivery tab** — The Display and AR controls on an offer's Delivery tab are missing, so you can't choose how a survey is delivered. This restores those selectable controls so you can configure it without going back to the old app. (#371)
- **[Bug]** **Offer edits aren't showing up in History** — When you edit and save an offer, the change isn't being recorded in the offer's History section. This fix ensures your edits appear there so there's a clear record of what changed. (#380)
- **[Feature]** **Automatic performance estimate for new offers** — Instead of relying on a manual gut-check, the system will estimate how a new offer is likely to perform based on your existing offers and their history, giving you a data-backed read at intake. (#322)

## Dashboard & Reports

- **[Feature]** **Notes on Placements, Advertisers, and Offers** — You'll be able to add short, categorized notes (with a topic and priority) directly on a Placement, Advertiser, or Offer, and see a recent-notes roll-up on the main Dashboard. Notes will appear right after you save them, without a page reload. (#382)
- **[Task]** **Checking that report numbers match the old system** — Some dashboard report figures didn't line up with the legacy app during testing. This investigation pins down where the difference comes from so you can trust the numbers. (#271)

## Surveys

- **[Feature]** **Design-tab customizations that actually show up** — Every option on the survey Design tab will be reflected in what visitors see, and a full check across all screens will catch any setting that currently does nothing. (#288)
- **[Feature]** **Finishing the Placement Design-tab settings** — Some Placement survey design options are saved but don't yet change what visitors see. This work either connects each one so it takes effect or removes it so the form only shows options that matter. (#293)

## Data Clients

- **[Feature]** **Restoring after-conversion delivery steps (high priority)** — Certain custom steps that ran right after a conversion in the old system weren't brought over. This work ports them so those data clients keep working as expected. (#327)
- **[Feature]** **Restoring custom pre-send checks (high priority)** — Hundreds of data clients relied on custom checks that ran before a lead was sent; these aren't running on the new platform yet. This work brings that validation back so leads are screened the same way as before. (#338)

## Behind the Scenes

- **[Feature]** **Turning conversations into tracked work items** — A helper that reads designated chat channels and automatically logs action items, so requests raised in conversation don't get lost. No direct effect on the product screens. (#272)
- **[Task]** **Strengthening automated testing** — A review of the automated checks that guard the app turned up gaps to close, so future changes are caught and verified more reliably. Behind-the-scenes quality work. (#379)

## Placements

- **[Feature]** **Preview your unsaved changes** — The Preview button on the Placement (and Offer) edit pages will show your current, in-progress edits instead of only the last saved version, so you can check a change before committing to it. (#292)

## Advertisers

- **[Feature]** **Web Presence links on the Advertiser page** — The advertiser's website, social profiles, and a "Search on Google" shortcut will appear as quick icon links in the page header, using the details you already enter on the Web Presence tab. (#383)

## Modals

- **[Feature]** **Making the Modal Design tab count** — The Modal Design tab's settings (title, subtitle, colors, progress bar) don't currently change what visitors see. This work either connects them so they take effect or removes the tab so it isn't misleading. (#294)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Parts of the Flow form look unstyled or stack awkwardly compared to other forms. This cleanup brings its layout and styling in line with the rest of the app. (#152)

## Admin Area

- **[Task]** **Bringing the Users area up to parity** — A detailed comparison of the old and new Users screens to identify what's missing (like bulk actions, last-login, and two-factor status) and prioritize bringing it over. A planning and documentation step toward a fuller Users experience. (#80)

## Publishers & Properties

- **[Bug]** **Making "paused" reliably stop serving** — Pausing a publisher or property isn't being enforced consistently, so a paused item could still serve in some cases. This fix ensures a pause is respected everywhere. (#299)

## General / Across the App

- **[Feature]** **Removing controls that do nothing** — Several admin settings (like the Advertiser Web Presence fields, certain user-permission toggles, and a few data-client and pre-ping options) are saved but aren't actually used anywhere. Hiding or removing them prevents confusion about settings that have no effect. (#296)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
