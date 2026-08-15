# Open Issues — Plain-Language Overview

_Last updated 2026-08-15 06:05:37 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer options never reach the live ad** — Several settings you can enter on an offer (including its Modal-tab fields, Display URL, and certain data-delivery options) aren't currently carried through to the visitor experience. This work makes sure every option that appears on the form actually takes effect, or is removed if it's not needed. (#295)
- **[Bug]** **Can't set a survey to Display or AR on an offer** — On the Offer Details Delivery tab, the Display and AR choices show as column headers but have no selectable controls, so you can't assign a survey's delivery mode. This restores those selections so you no longer have to fall back to the legacy app. (#371)
- **[Bug]** **Offer edits aren't showing up in History** — When you edit and save an offer, the change isn't recorded in the offer's History section. This fix makes your edits appear in History as expected. (#380)
- **[Bug]** **Manually selected offers coming across empty** — On placements set to Manual delivery, the list of hand-picked offers isn't carrying over, so the wrong offers can display. This fixes the migration so your selected offers (and their order) show and serve correctly. (#370)
- **[Feature]** **Preview your unsaved changes on placements and offers** — The Preview button will show the edits you're currently making, instead of only the last saved version, so you can check your work without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, giving Kurt a data-driven gut-check at intake instead of a manual review. (#322)

## Surveys

- **[Feature]** **Make sure every design option actually works** — A thorough check across all entities to confirm that each customization you set on a Design tab is truly reflected in the live survey, with any settings that do nothing either fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings** — A handful of placement Design-tab settings (like iFrame height and display format) are saved but not yet applied to the live survey. This wires them through so they take effect, and cleans up any that aren't used. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery steps** — Certain after-conversion delivery and redirect behaviors from the legacy system weren't yet available in New Adsmith Frontend. This brings those behaviors back so affected clients keep working as before. (#327)
- **[Feature]** **Bring across custom pre-delivery validation checks** — Hundreds of data clients rely on custom serve-time validation that isn't yet running on the new platform. This high-priority work ports those checks so leads are validated consistently. (#338)

## Dashboard & Reports

- **[Task]** **Investigate mismatched report numbers** — During testing, dashboard report figures didn't match the legacy system. This looks into where the difference comes from and either fixes it or confirms the numbers are correct. (#271)
- **[Feature]** **Add notes to Placements, Advertisers, and Offers** — You'll be able to attach short, categorized notes (with a topic and priority) directly from a Placement, Advertiser, or Offer detail page, and see a recent-notes roll-up on the main Dashboard — matching what the legacy app offered. (#382)

## General / Across the App

- **[Task]** **Bring user management up to par with the legacy app** — A review of the Users area against the older system to identify what's still missing (such as bulk actions and extra columns) so user management feels complete. (#80)
- **[Feature]** **Remove settings that don't do anything** — Several admin controls (like the Advertiser Web Presence tab, some user-permission toggles, and a few data-client and pre-ping options) currently save but have no effect. Hiding or removing them prevents confusion about what's actually in use. (#296)

## Behind the Scenes

- **[Feature]** **Auto-create tasks from Slack conversations** — An internal helper that turns action items from Slack discussions into tracked tasks automatically, reducing manual copy-and-paste. This is an internal workflow tool with no direct effect on the product screens. (#272)
- **[Task]** **Strengthen automated testing** — Behind-the-scenes improvements to the automated test suite so issues are caught more reliably before release. No user-facing change. (#379)

## Advertisers

- **[Feature]** **Show Web Presence links on the Advertiser detail page** — The website, social profile, and "Search on Google" links you enter for an advertiser will appear as a set of quick-access icons in the page header, just like in the legacy app. (#383)

## Flows

- **[Task]** **Fix styling on the Flow form** — Parts of the Flow form currently look unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacking instead of sitting side by side). This tidies up the layout to match the other forms. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The Modal Design tab's fields (header text, colors, progress bar) are saved but don't appear in the visitor modal. This either wires them up so they show or removes the tab if it isn't needed. (#294)

## Publishers

- **[Bug]** **Pausing a publisher or property doesn't always stick** — On one of the serving paths, pausing a publisher or property isn't being enforced. This fix makes sure a paused publisher or property is reliably blocked everywhere. (#299)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
