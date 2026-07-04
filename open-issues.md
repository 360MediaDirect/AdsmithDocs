# Open Issues — Plain-Language Overview

_Last updated 2026-07-04 00:29:09 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Bring back the Campaigns module** — You'll be able to view, create, edit, and configure campaigns and their offer groups directly in New Adsmith Frontend, matching what the older admin system could do. This is a high-priority piece of core functionality that's currently missing. (#200)
- **[Feature]** **Protection against two people overwriting each other's edits** — When someone else is already editing a record (an offer, flow, placement, advertiser, and so on), you'll see a clear "locked by" notice, and the system will warn you before you can accidentally save over changes someone made while you had the page open. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when across the product — including automated changes — so you can easily answer "who edited this and when." You'll also be able to view a record's history right from its detail page. (#276)
- **[Feature]** **Cleaning up controls that don't do anything** — Some settings currently appear in the admin (like the Advertiser Web Presence fields, certain user permission toggles, and a few Data Client and Pre-Ping options) but have no real effect. These will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link will now show a proper error message instead of quietly sending you to the Dashboard. (#239)

## Surveys

- **[Feature]** **Design settings that truly match the live survey** — Every customization option on the Design tab will be reflected in what visitors actually see, and we're auditing options across all screens so nothing looks adjustable while secretly doing nothing. (#288)
- **[Bug]** **Most survey Design-tab settings now take effect** — Today only a couple of the roughly 30 styling and behavior settings (colors, buttons, header, legal text, and more) actually change the live survey; the rest are saved but ignored. This work connects them so your choices show up for visitors. (#290)
- **[Bug]** **Voucher code and info links appear on the survey again** — For affected Data Clients, the custom voucher-code line and the privacy/terms/details links are configured but not showing on the live survey. This restores them, matching the older app — important for passing leads and staying compliant. (#291)
- **[Feature]** **Finishing the remaining Design-tab settings** — A handful of survey settings that were left partly connected (such as iframe height and display format) will either be made to work or removed so nothing is misleading. (#293)

## Placements & Offers

- **[Feature]** **Better offer ordering and filtering on Placements** — Manually arranged offers will actually serve in that order, and you'll be able to filter the available-offers list by vertical/category instead of only searching by text. (#275)
- **[Feature]** **Preview your unsaved changes** — On placement and offer edit pages, the Preview button will show your current in-progress edits rather than the last saved version, so you can check a change before committing it. (#292)
- **[Bug]** **All saved offer options reach the live experience** — Several saved offer settings (including Modal-tab fields and "Force More Info Visible") currently never make it to what visitors see. Each will be wired through or removed so saved options behave as expected. (#295)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example as a spreadsheet) for your own analysis. (#286)
- **[Task]** **Confirming report numbers match the older system** — We're investigating why some Dashboard report figures didn't line up with the legacy app, pinpointing where any differences come from and correcting them so you can trust the numbers. (#271)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the product against realistic data so changes can be verified without any risk of altering live information. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — An internal helper that reads team conversations and files the resulting to-dos as tracked items, reducing manual copy-and-paste. This is an internal workflow tool with no direct change to the product screens. (#272)

## Users

- **[Task]** **Comparing the new Users area to the older one** — A review documenting which Users features from the legacy system still need to be added (like bulk actions, two-factor status, and last-login info), to guide what gets built next. (#80)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Fixing styling gaps so textareas, color pickers, checkboxes, and paired fields look consistent and lay out correctly, matching the Placement and Modal forms. (#152)

## Modals

- **[Feature]** **Making the Modal Design tab count** — The Modal Design tab's settings (header title, subtitle, colors, progress bar) currently have no effect on what visitors see. These will either be connected to the live modal or removed so the tab isn't misleading. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
