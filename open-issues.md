# Open Issues — Plain-Language Overview

_Last updated 2026-07-03 05:17:26 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make survey Design-tab options actually change the survey** — Today many styling and behavior choices on the survey Design tab are saved but have no effect on what visitors see. This work connects those options end-to-end and audits every entity's form options so nothing is left doing nothing. (#288)
- **[Bug]** **Connect the remaining survey styling controls to the live survey** — Right now only a couple of the roughly 30 survey design settings (like colors, the continue button, header text, and legal text) actually reach the published survey. Once fixed, the choices you make in the Design tab will show up for real visitors. (#290)
- **[Bug]** **Finish wiring the last few Placement Design-tab settings** — A handful of design settings (such as height and display format) still don't reach the live survey. This finishes connecting them, and decides for the rest whether to make them work or remove them so nothing misleading is left in the form. (#293)
- **[Bug]** **Show voucher codes and info links on the live survey** — Custom questions (like a voucher code) and privacy/terms/details links are set up in the admin but aren't appearing on the new survey page, even though they showed in the old system. This restores them so visitors see the required voucher and compliance links. (#291)

## General / Across the App

- **[Feature]** **A full history of who changed what** — A new searchable Audit Log will record every change to offers, placements, advertisers, and other records — both manual edits and automated updates — with a timestamp and who made it, so you can always trace "who changed this and when." (#276)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record to edit it, others will see it's locked, and the system will warn you if a record changed while you had it open, so nobody's changes get silently lost. (#267)
- **[Feature]** **Tidy up controls that don't do anything** — Some admin settings (like certain Advertiser web-presence fields, user permission toggles, and a few Data-Client and Pre-Ping options) are saved but never actually used. These will be hidden or removed so the screens only show controls that truly work. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you back on the dashboard with no explanation. Once fixed, you'll get a clear failure message so you know the link didn't pass. (#239)

## Dashboard

- **[Feature]** **Pick report dates right in the dashboard** — Instead of editing the web address to change the reporting range, you'll get date controls built into the dashboard to pull a specific day or range. Shareable links still update automatically. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (for example to a spreadsheet) for your own analysis. This is a high-priority addition. (#286)
- **[Task]** **Confirm report numbers match the legacy system** — During testing, some dashboard figures didn't line up with the old system. This investigation compares the two over a fixed date range to find and explain any differences and confirm the numbers can be trusted. (#271)

## Offers

- **[Bug]** **Fix success pixels that never fire** — Conversion tracking pixels set up on offers aren't firing because of a format mismatch, meaning some conversions go unrecorded. This corrects it so configured pixels actually fire, with a test to prove it. High priority. (#297)
- **[Bug]** **Stop offer settings from being dropped before going live** — Several saved offer options (including modal fields, a display URL, and some data-client flags) never reach the live experience. Each will be either connected properly or cleared from the form so what you save is what you get. (#295)
- **[Feature]** **Preview your unsaved offer and placement edits** — The Preview button currently shows the last saved version, so you have to save before you can see a change. This upgrade lets the preview reflect your current, unsaved edits. (#292)

## Transactions & Compliance

- **[Feature]** **TrustedForm compliance for leads** — A coordinated effort to properly claim and retain compliance certificates when leads come in, and to make the lead-processing pipeline more reliable before it goes live. (#309)
- **[Bug]** **Prevent a lead from being sent to an advertiser twice** — Under certain retry conditions a lead could be delivered more than once, risking double-billing. This adds a safeguard so each lead is only sent once. High priority. (#303)
- **[Bug]** **Stop retrying leads that can never succeed** — Leads that are permanently rejected (for example duplicates or do-not-call) are currently retried repeatedly before being set aside. This teaches the system to tell permanent rejections from temporary hiccups so it stops wasting retries and keeps alerts meaningful. (#304)

## Placements

- **[Feature]** **Better default ordering and filtering for placement offers** — Builds on the recent drag-to-reorder work: new placements would default to your manual offer order (so your arrangement is actually used), and the available-offers list would gain a category/vertical filter to find offers faster. (#275)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — Every field on the Modal Design tab is currently saved but has no effect on the visitor's modal. This will either connect those fields so they work or remove the tab so it isn't misleading. (#294)

## Properties

- **[Bug]** **Make property domain restrictions actually apply** — Domain allow-listing set on a Property is currently ignored at run time because of a naming mismatch, so restrictions have no effect. This fixes it (and updates existing records) so domain settings take hold. (#300)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — The Campaigns feature from the old admin — creating and editing campaigns, offer groups, and their settings — isn't in New Adsmith Frontend yet. This adds it so you can manage campaigns as before. This is a critical, high-priority addition. (#200)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or awkwardly stacked compared with other forms. This cleanup restores proper styling for things like text boxes, color pickers, and side-by-side fields. Partly done, with the riskier layout changes handled carefully to avoid breaking other tabs. (#152)

## Users

- **[Task]** **Compare the new Users area to the old one** — A review of the old Users screen versus the new one to catalog what's missing (such as bulk actions, last-login and two-factor status, and password fields on new users) so the team can prioritize closing the gaps. (#80)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a separate environment that mirrors real data for testing and verification, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads team chat discussions and files the resulting action items as tracked issues, cutting out manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d38d8ca1795a452a0f0d67dcfaeace8d181daef5615cf577e333d88f335aa7ae -->
