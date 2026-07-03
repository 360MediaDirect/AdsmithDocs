# Open Issues — Plain-Language Overview

_Last updated 2026-07-03 13:33:54 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Survey

- **[Feature]** **Make sure every survey design option really works** — We're checking each customization option across the app so that anything you set on a Design tab actually shows up for visitors, with no "dead" settings that look adjustable but do nothing. (#288)
- **[Bug]** **Survey styling settings that don't take effect** — Right now only a couple of the roughly 30 look-and-feel options (colors, buttons, header text, legal text, progress bar) actually change the live survey. This fix connects the rest so the survey visitors see matches what you set up. (#290)
- **[Bug]** **Voucher code and info links missing on the live survey** — For affected data clients, the voucher code line and the privacy/terms/details links are configured but not appearing on the new survey page. This restores them so they show just like in the legacy app. (#291)
- **[Feature]** **Finish connecting the remaining Placement design settings** — A handful of survey settings (such as height and display format) are saved but still don't reach the live widget. Each will either be made to work or removed from the form so nothing is misleading. (#293)

## General / Across the App

- **[Bug]** **Invalid link test should show a clear error** — When you test a link that isn't valid, you'll get a proper failure message instead of being unexpectedly bounced to the dashboard. (#239)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else is already editing a record, you'll see a clear "locked by" note and be warned before you can accidentally undo their changes. This protects against silent lost edits across all entity screens. (#267)
- **[Feature]** **Searchable history of who changed what** — A new Audit Log will record every change to offers, placements, advertisers and more (including automated ones), with a timestamp and who made it, so you can always trace "who changed this and when." (#276)
- **[Feature]** **Remove controls that don't do anything** — Several settings (like the Advertiser Web Presence fields, some user permission toggles, and a few data-client and pre-ping options) are shown but have no effect. They'll be hidden or removed so the admin only shows controls that actually work. (#296)

## Dashboard

- **[Feature]** **Pick report dates without editing the web address** — You'll get proper date controls in the dashboard toolbar to pull daily or custom-range reports, instead of having to hand-edit the address bar. Shareable links still work. (#268)
- **[Task]** **Investigate why report numbers don't match the legacy system** — We're comparing the new dashboard figures against the old app to find and explain any differences, so you can trust the reported numbers. (#271)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example as a spreadsheet). This is a high-priority addition. (#286)

## Leads & Compliance

- **[Feature]** **TrustedForm compliance for leads** — This is the umbrella effort to properly claim and retain compliance certificates when leads come through, with per-data-client control and a stronger, more reliable lead pipeline. (#309)
- **[Bug]** **Stop a lead from being sent to an advertiser twice** — A retry could occasionally deliver the same lead more than once. This fix ensures each lead is only delivered once, avoiding double-billing and advertiser-trust issues. This is high priority. (#303)
- **[Bug]** **Stop pointless retries of leads that can't succeed** — Leads rejected for good reasons (like duplicates or do-not-call) are currently retried several times before being set aside. This change stops the wasted retries and keeps the error queue meaningful. (#304)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on placements** — New placements will default to your manual offer order (so your drag-to-reorder actually takes effect), and you'll be able to filter the available offers list by category instead of only searching by text. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show your current in-progress edits, so you no longer have to save first just to see how a change looks. (#292)

## Offers

- **[Bug]** **Some saved offer settings never reach the live widget** — Several offer options (including the Modal-tab fields, Display URL, and a few backend flags) are saved but dropped before they take effect. Each will be connected properly or removed so what you configure is what runs. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — Pixels set to fire when an offer converts are saved but silently never run, meaning lost conversion tracking. This high-priority fix makes configured success pixels reliably fire. (#297)

## Behind the Scenes

- **[Task]** **Read-only test environment for verification** — Setting up a safe, look-but-don't-touch copy of the app running against prod-like data so testing can be done without risk to live information. (#270)
- **[Feature]** **Turn Slack conversations into tracked tasks automatically** — A helper that reads designated Slack channels and files action items as tracked issues automatically, replacing manual copy-and-paste. (#272)

## Campaigns

- **[Feature]** **Bring back the Campaigns area** — The Campaigns module from the old admin isn't in the new platform yet. This adds the ability to view, create, edit and configure campaigns and offer groups, matching the legacy workflow. This is a high-priority, core feature. (#200)

## Flows

- **[Task]** **Tidy up the appearance of the Flow form** — Some parts of the Flow form look unstyled or misaligned compared to other screens (plain text boxes, paired fields stacking vertically). This cleans up the layout so it matches the rest of the app. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab actually work — or remove it** — All six settings on the Modal Design tab currently have no effect on what visitors see. Each will either be wired up to the visitor modal or removed so the tab isn't misleading. (#294)

## Properties

- **[Bug]** **Domain restrictions on Properties aren't applied** — Allowed-domain settings you enter on a Property are saved but ignored at runtime, so the restriction does nothing. This fix makes the domain allow-list actually take effect. (#300)

## Users

- **[Task]** **Compare the new Users area to the old one** — A review of the old versus new Users management to catch anything missing (like bulk actions or last-login info) and plan what to add. This is a documentation and analysis effort. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d38d8ca1795a452a0f0d67dcfaeace8d181daef5615cf577e333d88f335aa7ae -->
