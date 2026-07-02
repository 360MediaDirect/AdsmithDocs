# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 23:24:49 UTC · 28 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Protect against two people overwriting each other's edits** — When you open a record to edit it, New Adsmith Frontend will let you know if someone else already has it open, and will stop one person's save from silently wiping out another's changes. Applies across all editable screens. (#267)
- **[Feature]** **Searchable history of who changed what** — A new Audit Log will record every change to records — manual or automatic — with a timestamp and the person or process behind it, so you can finally trace "who changed this and when." (#276)
- **[Feature]** **Remove settings that don't actually do anything** — Some admin options (certain Advertiser web-presence fields, a few user-permission toggles, and some Data Client and Pre-Ping settings) currently save but have no effect. They'll be hidden or removed so screens only show controls that truly work. (#296)
- **[Feature]** **Bring back the Campaigns module** — The Campaigns area from the older system isn't in New Adsmith Frontend yet. This high-priority work adds it back so you can create, edit, and manage campaigns and offer groups. (#200)
- **[Bug]** **Invalid link tests will show a clear error** — Right now, testing a bad link quietly sends you to the Dashboard. After this fix you'll get a proper failure message instead. (#239)
- **[Task]** **Review of the Users area against the older system** — A behind-the-scenes comparison of the old and new Users screens to catch any missing capabilities and plan what to add. (#80)

## Compliance & Lead Delivery
- **[Feature]** **TrustedForm compliance program** — The overarching effort to claim and safely store TrustedForm consent certificates for leads, and to harden the lead-delivery pipeline. The items below are part of this work. (#309)
- **[Bug]** **Stop a lead from being sent to an advertiser twice** — Under certain retry conditions a lead could be delivered to an advertiser more than once. This fix ensures each lead is delivered a single time, avoiding double-billing and advertiser-trust issues. (#303)
- **[Bug]** **Stop retrying leads that can never succeed** — Leads that are rightfully rejected (duplicates, do-not-call, failed validation) are currently retried repeatedly before being set aside. This fix lets the system recognize final outcomes and stop wasting retries. (#304)
- **[Feature]** **Add a Data Client control for TrustedForm cert claiming** — There's a per-data-client setting to turn TrustedForm certificate claiming on, but no way to set it in the admin yet. This adds that toggle to the Data Client form. (#305)
- **[Task]** **Review how long consent records are kept** — A behind-the-scenes policy review of the two-year retention on stored TrustedForm certificate records and the personal details they contain. (#306)

## Surveys
- **[Feature]** **Make every survey design option actually take effect** — The Design tab offers many styling choices, but not all of them currently change what visitors see. This work connects each option end to end and audits every form across the product for the same issue. (#288)
- **[Bug]** **Connect the survey Design-tab styling to the live survey** — Most of the roughly 30 survey styling and behavior settings (colors, buttons, header, legal text) are saved but don't yet change the visitor-facing survey. This fix makes them work. (#290)
- **[Bug]** **Show voucher codes and info links on the live survey** — For affected data clients, the voucher-code line and the privacy/terms/details links are set up in the admin but don't appear on the new survey page (they do in the old one). This restores them — important for both lead quality and compliance. (#291)
- **[Feature]** **Finish connecting the last few survey Design settings** — A handful of remaining Design-tab options (such as survey height and display format) will either be wired up to the live survey or removed if unused. (#293)

## Dashboard
- **[Feature]** **Filter dates without editing the web address** — Instead of hand-editing the address bar to pull a specific day or range, you'll have easy date controls right in the Dashboard. Links will still stay shareable. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A high-priority addition of an export button so you can download the breakdown-by-day data (for example, to a spreadsheet). (#286)
- **[Task]** **Add a custom date range picker** — Choosing "Custom" in the Dashboard date filter will open start- and end-date pickers with Apply/Cancel, and the Dashboard will update to your chosen range. (#58)
- **[Task]** **Confirm Dashboard report numbers match the old system** — An investigation into why some Dashboard figures differ from the legacy system, so you can trust the reported numbers. (#271)

## Offers
- **[Bug]** **Make sure saved offer settings reach the live experience** — Several offer options (including modal fields and some data-client flags) are saved but dropped before they reach the live offer. Each will be connected properly or removed if not needed. (#295)
- **[Bug]** **Fix success pixels that never fire** — Conversion tracking pixels set on an offer currently never fire because of a format mismatch, so attribution can be lost silently. This fix makes configured success pixels fire reliably. (#297)

## Placements
- **[Feature]** **Better sorting and filtering when choosing offers** — New placements will be able to default to manual offer ordering (so your arranged order is actually used), and the available-offers list will gain a filter by vertical/category alongside search. (#275)
- **[Feature]** **Preview your unsaved edits** — On placement and offer edit screens, Preview will show your current in-progress changes instead of only the last saved version, so you don't have to save first to see how something looks. (#292)

## Behind the Scenes
- **[Task]** **Set up a safe testing environment with May and June data** — Provides a stable dataset for validating reports and testing without touching live information. (#270)
- **[Feature]** **Automatically turn conversations into tracked work items** — A helper that reads designated chat conversations and files the resulting action items automatically, reducing manual copy-and-paste. (#272)

## Flows
- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned compared with other forms. This clean-up makes text boxes, color pickers, checkboxes, and paired fields look consistent. (#152)

## Modals
- **[Feature]** **Make the Modal Design tab work — or remove it** — Every field on the Modal Design tab currently saves but has no effect on the visitor-facing modal. This work either connects them (headers, progress bar) or removes the tab if it isn't needed. (#294)

## Properties
- **[Bug]** **Make Property domain restrictions actually apply** — Domain base and allow-list settings entered on a Property currently have no effect at runtime. This fix ensures the restrictions you configure are enforced, and updates existing records to match. (#300)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 0fee697ea8c356ff0dd7e2484fe5d7102761b0916f13b0161fbcef18cc7a1087 -->
