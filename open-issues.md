# Open Issues — Plain-Language Overview

_Last updated 2026-07-03 11:47:01 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record to edit, others will see it's already being worked on, and you'll get a clear warning if a record changed since you opened it — so no one's changes get silently wiped out. Works across every entity screen. (#267)
- **[Feature]** **Searchable activity history for every change** — A new admin "Audit Log" will record who changed what and when — across offers, placements, advertisers, and more, including automated updates. You'll be able to search by record, person, action, or date, and view a history right from each record. (#276)
- **[Feature]** **Tidy up controls that don't actually do anything** — Several admin settings currently save but have no effect (some Advertiser Web Presence fields, a couple of user-permission toggles, and a few Data Client and Pre-Ping options). These will be removed or hidden so the screens only show controls that really work. (#296)
- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link currently dumps you on the Dashboard with no explanation. This fix shows a proper error message so you know the link failed. (#239)
- **[Task]** **Review of the Users area against the old system** — A behind-the-scenes comparison of the new Users screens versus the legacy version, to catch missing pieces (like bulk actions and last-login info) and prioritize what to add next. (#80)

## Surveys

- **[Feature]** **Make sure every survey design option actually changes the survey** — A full sweep to confirm each customization you set on the Design tab (colors, buttons, headers, and more) truly appears in the live survey, with any unused options fixed or removed. (#288)
- **[Bug]** **Connect the remaining survey styling settings to the live survey** — Today only a couple of Design-tab settings reach visitors; the rest save but do nothing. This wires up the missing colors, buttons, headers, question text, and legal text so what you configure is what visitors see. (#290)
- **[Bug]** **Show the voucher code and info links on the live survey** — Configured items like the voucher code line and the privacy/terms/details links aren't appearing on the new survey page (they show in the old one). This restores them for the affected clients. (#291)
- **[Feature]** **Finish wiring the last few survey Design-tab settings** — A follow-up to complete the remaining styling and behavior options (such as survey height and display format) so every setting either works in the live survey or is removed from the form. (#293)

## Dashboard

- **[Feature]** **Pick report dates right in the Dashboard** — Instead of hand-editing the web address to change the reporting range, you'll get date controls built into the Dashboard toolbar to pull daily or custom ranges easily. Shareable links still work. (#268)
- **[Feature]** **Download the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (for example, to a spreadsheet). High priority. (#286)
- **[Task]** **Confirm Dashboard numbers match the old system** — An investigation into why some Dashboard report figures differ from the legacy app, to pin down the cause and either fix it or confirm the numbers are correct. (#271)

## Leads & Compliance

- **[Feature]** **TrustedForm compliance for lead handling** — Ongoing work to properly claim and retain compliance certificates for leads, with per-client controls and stronger safeguards in the lead pipeline. (#309)
- **[Bug]** **Prevent a lead being sent to an advertiser twice** — Fixes a situation where a lead could be delivered more than once if a later step hiccupped, avoiding double-billing and advertiser-trust issues. High priority. (#303)
- **[Bug]** **Stop retrying leads that can never succeed** — Leads that are permanently rejected (for example, duplicates or "do not call") are currently retried several times before being set aside. This makes the system recognize a final rejection and stop retrying unnecessarily. (#304)

## Offers

- **[Bug]** **Make sure success tracking pixels actually fire** — Conversion pixels set on offers currently never fire because of a format mismatch, quietly losing tracking data. This fixes them so configured pixels fire as expected. High priority. (#297)
- **[Bug]** **Stop offer settings from being lost before they reach the live page** — Several saved offer options (including Modal-tab fields and a few others) never make it to the live experience. Each will be properly connected or removed so nothing silently disappears. (#295)

## Placements

- **[Feature]** **Better default sorting and filtering when picking offers** — Follow-up work so newly built placements can default to your manual offer order, and so you can filter the available-offers list by category instead of only searching by text. (#275)
- **[Feature]** **Preview your unsaved changes on placements and offers** — The Preview button will show your current edits before you save, so you no longer have to save first just to see how a change looks. (#292)

## Behind the Scenes

- **[Task]** **Set up a safe, look-only test environment** — Stand up a staging copy of the product using production-like data, locked to read-only, so the team can validate behavior without any risk of changing real data. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — An internal helper that reads designated Slack channels and automatically files action items as tracked issues, cutting out manual copy-and-paste. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — All six Modal Design settings currently save but never appear to visitors. They'll either be connected to the live modal or removed from the form. (#294)

## Properties

- **[Bug]** **Make domain restrictions on Properties actually take effect** — Domain allow-listing set on a Property currently has no effect at runtime because of a naming mismatch. This aligns the settings so your restrictions are enforced, and updates existing records. (#300)

## Campaigns

- **[Feature]** **Bring the Campaigns area into the new product** — The Campaigns module from the old admin isn't in the new platform yet. This adds it back so you can view, create, edit, and configure campaigns and their offer groups. Critical, high priority. (#200)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or awkwardly stacked. This cleans up the layout and styling so it matches the polished look of the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d38d8ca1795a452a0f0d67dcfaeace8d181daef5615cf577e333d88f335aa7ae -->
