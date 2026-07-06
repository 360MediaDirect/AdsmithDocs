# Open Issues — Plain-Language Overview

_Last updated 2026-07-06 05:26:04 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Survey
- **[Feature]** **Make survey design settings actually change the survey** — Today many customization options in the design tab are saved but don't affect what visitors see. This work confirms every design option flows through end-to-end, so the choices you make in the admin actually show up in the live survey. (#288)
- **[Bug]** **Survey styling controls now take effect** — Around 30 look-and-feel settings (colors, buttons, header, question text, legal text) are configurable but currently ignored by the live survey. This fixes them so your styling choices are reflected for visitors. (#290)
- **[Feature]** **Finish connecting the remaining survey design settings** — A few leftover settings (like survey height and question display format) still don't reach the live survey. This wires them up or removes any option that isn't meant to do anything, so nothing in the form is misleading. (#293)
- **[Bug]** **Voucher codes and info links show on the live survey again** — For affected clients, the voucher code line and the privacy/terms/details links are set up in the admin but aren't appearing on the survey page like they did in the old system. This restores them, which matters for lead processing and compliance. (#291)

## Placements & Offers
- **[Bug]** **Saved offer settings reach the live experience** — Several offer options you set and save (including modal-tab fields and "Force More Info Visible") never make it to what visitors see. This ensures each saved option either works on the live surface or is cleaned up so it isn't misleading. (#295)
- **[Feature]** **Sort offers in your chosen order by default, plus filter by category** — New placements will default to your manual offer order (so your drag-and-drop arrangement is respected), and you'll be able to filter the available offers list by category/vertical to find offers faster. (#275)
- **[Feature]** **Preview your unsaved edits before saving** — On placement and offer edit pages, the Preview button will show the changes you're currently making instead of only the last saved version, so you can check your work without saving first. (#292)

## Dashboard
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example, to a spreadsheet) for your own reporting and analysis. (#286)
- **[Task]** **Confirm dashboard numbers match the old system** — We're investigating why some dashboard report figures differed from the legacy app during testing, so we can pinpoint the cause and give you confidence the numbers are accurate. (#271)

## Admin / Across the App
- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record, the app will warn you if someone else is already editing it and stop your save from silently wiping out their changes, protecting your work across all entity screens. (#267)
- **[Feature]** **Tidy up controls that don't do anything** — Some admin fields (such as Advertiser "Web Presence" links, certain user permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no real effect. These will be removed or hidden so the admin only shows controls that actually work. (#296)

## Reports & Auditing
- **[Feature]** **See who changed what, and when** — A new searchable Audit Log will record every change to your records — by people and by automated jobs — with timestamps, so troubleshooting "who changed this?" becomes easy. You'll also be able to view a record's history from its detail page. (#276)

## Campaigns
- **[Feature]** **Bring back the Campaigns area** — The Campaigns module from the old admin isn't in New Adsmith Frontend yet. This adds it back so you can create, edit, and manage campaigns and their offer groups. High priority. (#200)

## Flows
- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form currently look unstyled or broken (plain textareas, unstyled color pickers, and paired fields stacking oddly). This cleans up the layout so it matches the polished look of other forms. (#152)

## Modals
- **[Feature]** **Make the Modal design tab meaningful** — The entire Modal Design tab currently has no effect on the visitor-facing modal. This either connects those settings so they work or removes them so the tab isn't misleading. (#294)

## Users
- **[Task]** **Compare the Users area to the old system** — A review checking which features from the legacy Users screen are still missing in New Adsmith Frontend, so we can prioritize closing the gaps. (#80)

## Link Testing
- **[Bug]** **Show a clear error for an invalid link** — When you test a link that's invalid, you're currently sent to the dashboard with no explanation. This will instead show a clear failure message so you know the link didn't work. (#239)

## Behind the Scenes
- **[Task]** **Set up a safe test environment** — Standing up a read-only environment using production-like data so testing and verification can happen without any risk of changing live information. (#270)
- **[Feature]** **Automatically turn conversations into tracked tasks** — An internal helper that reads team conversations and files the resulting to-dos automatically, reducing manual copying so nothing falls through the cracks. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
