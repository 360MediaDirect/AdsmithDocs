# Open Issues — Plain-Language Overview

_Last updated 2026-07-06 22:26:31 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make design settings actually change the survey** — We're connecting the survey Design tab so every styling and behavior option you set is reflected in what visitors see, and checking form options across all screens to make sure none of them are just for show. (#288)
- **[Bug]** **Bring the rest of the Design settings to life** — Right now most survey styling choices (colors, buttons, headers, legal text, progress bar) are saved but ignored by the live survey. This fix wires them through so your customizations take effect. (#290)
- **[Feature]** **Finish connecting the remaining survey styling options** — A few leftover Design-tab settings, like survey height and question display format, will finally be applied to the live widget instead of quietly doing nothing. (#293)
- **[Bug]** **Show voucher code and info links on live surveys** — For affected data clients, the voucher code line and the privacy/terms/details links are missing from the new survey page even though they're set up correctly. This restores them to match the older system. (#291)

## General / Across the App

- **[Feature]** **Warn when two people edit the same record** — If a colleague changes a record while you have it open, you'll be told before you accidentally overwrite their work, protecting against lost updates across offers, flows, placements, advertisers, and more. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when across the platform, including automated changes, so you can easily investigate "who edited this and when." (#276)
- **[Feature]** **Remove buttons and fields that do nothing** — Several admin controls (like Advertiser Web Presence, some user permission toggles, and a few Data Client and Pre-Ping options) are saved but have no effect. These will be hidden or removed so the screens only show controls that actually work. (#296)
- **[Bug]** **Show a clear error for an invalid link test** — Testing an invalid link currently dumps you on the dashboard with no explanation; instead you'll get a clear failure message right where you tested it. (#239)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — You'll be able to download the breakdown-by-day data with a single button, making it easy to work with the numbers outside the dashboard. (#286)
- **[Bug]** **Fix Offer Detail failing on "Last Month"** — Opening an Offer Detail page with the "Last Month" filter currently times out and shows a "Failed to load" error. This fix makes that date range load reliably. (#318)
- **[Task]** **Confirm dashboard numbers match the old system** — We're investigating why some dashboard report figures differed from the legacy system to pin down the cause and ensure the numbers you see are trustworthy. (#271)

## Placements

- **[Feature]** **Better control of the offer list order and filtering** — New placements will default to your manual offer order (so your arrangement is actually used), and you'll be able to filter the available offers by category instead of only searching by text. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show your current in-progress edits instead of the last saved version, so you no longer have to save just to see how a change looks. (#292)

## Behind the Scenes

- **[Task]** **Read-only staging environment for testing** — Setting up a safe, look-but-don't-touch copy of the product against realistic data so changes can be verified before they reach everyone. (#270)
- **[Feature]** **Turn Slack conversations into tracked tasks** — A helper that reads designated Slack discussions and automatically logs the action items, reducing manual note-taking and follow-up. (#272)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — Campaign management from the older admin isn't available yet in New Adsmith Frontend. This high-priority work adds the ability to view, create, edit, and configure campaigns and their offer groups. (#200)

## Offers

- **[Bug]** **Stop offer settings from getting lost before they reach visitors** — Several saved offer options (including Modal-tab fields and other flags) currently never make it to the live experience. This ensures each option is either delivered and used or clearly removed. (#295)

## Modals

- **[Feature]** **Make the Modal Design tab do something** — Every field on the Modal Design tab is currently saved but has no effect on the visitor modal. We'll either connect these settings so they display or remove them to avoid confusion. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or broken, with fields stacking awkwardly and plain-looking text boxes and color pickers. This cleans up the layout to match other forms. (#152)

## Users

- **[Task]** **Compare the old and new Users screens** — A review of what the older Users area could do versus the new one, so we know which features to bring over and can plan improvements. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6c27af732f3641fd9b535e157afcb427a79ad241cf9415444c675c49de3c7588 -->
