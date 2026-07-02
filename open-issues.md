# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 20:29:17 UTC · 31 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit it, others will see it's being worked on, and you'll be warned if someone changed it since you opened it — so nobody's changes get silently wiped out. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when across the app (offers, placements, advertisers, and more), including automated changes, so you can always trace "who edited this and when." (#276)
- **[Feature]** **Clean up controls that don't actually do anything** — Several settings that look active but currently have no effect (Advertiser Web Presence links, some user permission toggles, and a few Data Client and Pre-Ping options) will be either removed or made functional, so the screens only show controls that truly work. (#296)
- **[Task]** **Bring the Users area up to par with the old system** — A review of the legacy Users screens versus the new ones to identify missing pieces (like bulk role changes and password/notification options) and close the gaps. (#80)
- **[Feature]** **Bring back the Campaigns area** — The Campaigns module from the old admin isn't in the new platform yet. This adds it back so you can create, edit, and manage campaigns and offer groups. High priority. (#200)
- **[Bug]** **Clear error when testing an invalid link** — Right now testing a bad link quietly dumps you on the Dashboard. This fix will instead show a proper error so you know the link failed. (#239)

## Ad Serving & Lead Delivery

- **[Bug]** **Success pixels now actually fire** — Conversion/tracking pixels set up on offers currently never fire because of a formatting mismatch, meaning lost tracking. This fixes them so configured pixels reliably fire on success. High priority. (#297)
- **[Bug]** **Pre-Ping "equals" condition works again** — The "equals" match option on Pre-Pings silently never matched, leading to wrong lead-qualification decisions. This fix makes it evaluate correctly. High priority. (#298)
- **[Bug]** **Pausing a publisher or property truly stops it** — One part of the system ignored the paused status, so enforcement was inconsistent. This makes paused publishers and properties reliably blocked everywhere. (#299)
- **[Bug]** **Property domain restrictions take effect** — Domain base/allow-list settings on Properties were being saved but ignored at run time. This connects them so the restrictions actually apply. (#300)
- **[Bug]** **No more duplicate leads sent to advertisers** — In rare retry situations a lead could be delivered to an advertiser more than once. This adds a safeguard so each lead is only posted once. High priority. (#303)
- **[Bug]** **Stop pointlessly retrying leads that can't succeed** — Leads that are permanently rejected (duplicates, do-not-call, validation failures) were being retried repeatedly before failing. This will tell the difference between temporary and permanent failures so only recoverable ones retry. (#304)

## Surveys

- **[Feature]** **Design settings actually change what visitors see** — A full audit to make sure every option on the Design tab (and other entity forms) is wired end-to-end, so a change you make in the admin genuinely shows up in the live survey. (#288)
- **[Bug]** **Most survey styling options now work** — Around 30 Design-tab settings (colors, buttons, header, question text, legal text) were saved but had no effect on the live survey. This connects them so your styling choices appear to visitors. High priority area. (#290)
- **[Bug]** **Voucher code and info links show on the survey** — A configured custom question (voucher code) and the privacy/terms/details links weren't appearing on the live survey even though they're set up in the admin. This restores them, matching the old app. High priority. (#291)
- **[Feature]** **Finish connecting the remaining survey design settings** — A handful of Design-tab settings left over from the earlier work (like iFrame height and display format) will be finished so each one either affects the survey or is removed if unused. (#293)

## Dashboard

- **[Task]** **Custom date range picker** — Choosing "Custom" on the Dashboard date filter will open start- and end-date pickers with Apply/Cancel, so you can view data for any range you want. (#58)
- **[Feature]** **Pick report dates without editing the web address** — You'll be able to choose a day or date range straight from the Dashboard controls instead of hand-editing the URL, while still keeping links shareable. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button will let you download the breakdown-by-day data (e.g. as a spreadsheet) for your own analysis. High priority. (#286)

## Compliance

- **[Feature]** **Turn TrustedForm cert claiming on per Data Client** — The behavior already works behind the scenes, but this adds a simple toggle on the Data Client form so you can opt a client in without needing technical help. (#305)
- **[Task]** **Review how long TrustedForm records are kept** — A policy check on the 2-year retention and stored details of TrustedForm consent records, to confirm we keep the right information for the right length of time. (#306)
- **[Feature]** **Overall TrustedForm compliance effort** — The umbrella item tracking the work to claim and retain compliance certificates and harden the lead pipeline. (#309)

## Placements & Offers

- **[Feature]** **Smarter offer ordering and filtering on Placements** — Follow-up work to default new placements to Manual Order (so your drag-to-reorder is actually respected) and to add a filter for the available offers list by category. (#275)
- **[Feature]** **Preview shows your unsaved edits** — The Preview button on placement and offer edit pages will reflect the changes you're currently making, instead of only the last saved version — so you can preview before saving. (#292)
- **[Bug]** **Offer options reach the live widget** — Several saved offer settings (including Modal-tab fields and some backend flags) were being dropped before they reached the live experience. This ensures each is either delivered and used, or cleanly removed. (#295)

## Reports & Data

- **[Task]** **A safe test environment with May & June data** — Set up a staging area loaded with recent data so report testing can happen without touching live information. (#270)
- **[Task]** **Confirm report numbers match the old system** — An investigation into why some Dashboard report figures differed from the legacy app, to pinpoint the cause and confirm the numbers line up. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab count** — The entire Modal Design tab currently has no effect on what visitors see. This will either wire those six settings through to the live modal or remove the tab if it's not needed. (#294)
- **[Bug]** **Fix the unsavable "In Order" modal sort** — The "In Order" offer sorting choice can't currently be saved. This will either make it save and sort correctly or remove it from the form. (#301)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned (plain text boxes, stacked fields, unstyled color pickers). This brings it in line with the other forms. (#152)

## Behind the Scenes

- **[Feature]** **Automatic issue filing from chat** — An internal helper that reads team conversations and turns action items into tracked issues automatically, reducing manual copy-and-paste. No direct effect on the product UI. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: a3eecca103db7263b87211f38f83acd97ed20068ba99bc5db7c9c86a44b2a676 -->
