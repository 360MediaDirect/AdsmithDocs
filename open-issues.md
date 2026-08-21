# Open Issues — Plain-Language Overview

_Last updated 2026-08-21 06:08:10 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview offers and placements with your unsaved changes** — When editing a placement or an offer, the Preview button will show exactly what you're working on right now, including edits you haven't saved yet, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Missing offer settings will reach the live experience** — Several options you set on an offer (including its Modal-tab settings, "Force More Info Visible," and Display URL) currently never make it to what visitors actually see. This fix ensures the choices you save are honored or clearly removed if unused. (#295)
- **[Bug]** **Manually selected offers now carry over correctly** — On placements set to manual offer delivery, the exact offers you've chosen (and their order) will show as expected instead of appearing empty or defaulting to the wrong offer. This closes a gap where the new and old systems displayed different offers. (#370)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory feature to estimate how a new offer is likely to perform, based on your own history with similar offers, giving Kurt a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Surveys

- **[Feature]** **Design choices will actually show up in the survey** — A thorough check across all entities to make sure every design and customization option you set is reflected in the live survey, with any options that do nothing either fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live widget** — Placement Design-tab settings like iframe height and display format will take effect on the visitor-facing survey, and a few settings that currently have no effect will be wired up or cleaned out. (#293)

## Dashboard

- **[Task]** **Confirm dashboard report numbers match the old system** — An investigation into why some dashboard report figures didn't line up with the legacy app during testing, so you can trust that the numbers you see are accurate. (#271)
- **[Feature]** **Notes on Placements, Advertisers, and Offers** — Bringing back the ability to attach short, categorized notes (with topic and priority) to a Placement, Advertiser, or Offer from its detail page, plus a recent-notes roll-up on the main Dashboard. New notes will appear right away without needing to reload the page. (#382)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behaviors** — The after-success delivery and redirect steps used by certain clients (bperx, rwdb) are being carried over to New Adsmith Frontend so those clients keep working as they did before. Nearly complete. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — High-priority work to bring over the custom serve-time validation used by hundreds of data clients, which currently isn't running on the new platform. Once done, paused or filtered leads will be handled correctly for these clients. (#338)

## Behind the Scenes

- **[Feature]** **Automatically turn Slack discussions into tracked work items** — A helper that reads designated Slack conversations, pulls out action items, and logs them as tracked issues, cutting out manual note-taking after meetings. (#272)
- **[Task]** **Strengthen automated testing of the Admin area** — Follow-up work from a review of the app's automated tests to close coverage gaps and make test runs more reliable, so problems are caught before they reach you. (#379)

## General / Across the App

- **[Feature]** **Remove controls that don't do anything** — Several admin settings that quietly have no effect (Advertiser Web Presence fields, certain user-permission toggles, and some Data-Client and Pre-Ping options) will be hidden or removed, so you're not misled by switches that do nothing. (#296)
- **[Task]** **Users management gap review vs. the old app** — A documentation effort comparing the old Users screens with the new ones to identify missing capabilities (like bulk actions and role changes) and plan how to close the gaps. (#80)

## Advertisers

- **[Feature]** **Show Web Presence links on the Advertiser page** — The advertiser's website, social profiles, and a "Search on Google" shortcut will appear as icon links at the top of the Advertiser detail page, using the details you already enter on the Web Presence tab. (#383)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — Every field on the Modal Design tab currently has no visible effect. This work will either bring those header and progress-bar settings to life for visitors or remove the tab so it isn't misleading. (#294)

## Publishers

- **[Bug]** **Pausing a publisher or property will reliably stop delivery** — A fix so that pausing a publisher or property is enforced consistently across the system, closing a gap where one path ignored the paused status. (#299)

## Flows

- **[Task]** **Tidy up the appearance of the Flow form** — Fixes to styling on the Flow form so text boxes, color pickers, checkboxes, and paired fields look consistent and properly laid out, matching the Placement and Modal forms. Partially done. (#152)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
