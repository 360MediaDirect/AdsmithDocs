# Open Issues — Plain-Language Overview

_Last updated 2026-07-05 17:26:32 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Task]** **Bringing the Users area up to parity with the old system** — A review of the older Users management screens against the new ones is underway to spot anything missing, such as bulk role changes, extra list columns, and login-related details. Once complete, the new Users area will do everything the old one did. (#80)
- **[Feature]** **Protection against two people overwriting each other's edits** — When someone opens a record to edit, others will see it's already being worked on and won't accidentally save over their changes. This will apply across all the main entity screens like Offers, Placements, Advertisers, and more. (#267)
- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every change made to records (by both people and automated processes), with a timestamp and who made it, so you can easily answer "who changed this and when." You'll also see a change history right on each record's page. (#276)
- **[Feature]** **Removing settings that don't actually do anything** — Several admin controls currently look like they work but have no effect (for example, the Advertiser Web Presence fields and some user permission toggles). These will be removed or hidden so the screens only show settings that genuinely change something. (#296)
- **[Bug]** **Link testing should show a clear error for bad links** — Today, testing an invalid link quietly sends you to the dashboard. This fix will show a proper error message instead, so you know the link failed. (#239)

## Surveys

- **[Feature]** **Making sure every survey Design option actually works** — A full check is being done so that every customization you set on the Design tab truly shows up in the live survey, with no dead or ignored options. (#288)
- **[Bug]** **Design tab settings that weren't reaching the live survey** — Most survey styling and behavior settings (colors, buttons, header text, legal text, and more) were being saved but never applied to what visitors actually saw. This work connects them so your choices take effect. (#290)
- **[Bug]** **Finishing the last of the survey Design settings** — A remaining handful of survey settings (such as height and display format) still need to be wired up or cleaned out, so every option on the tab either works or is removed. (#293)
- **[Bug]** **Voucher code and info links missing from the live survey** — Some configured items, like a voucher code line and the privacy/terms/details links, aren't appearing on the new survey page even though they show in the old one. This fix restores them, which matters for both the visitor experience and compliance. (#291)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on Placements** — Placements will default to using your manual offer order (so your drag-and-drop arrangement actually takes effect), and you'll be able to filter the available offers list by category to find offers faster. (#275)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — The Preview button will show your current edits before you save, so you no longer have to save just to see how a change looks. (#292)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example as a spreadsheet) for your own analysis. (#286)
- **[Task]** **Confirming dashboard report numbers match the old system** — An investigation is comparing report figures between the new platform and the legacy system to explain any differences and make sure the numbers you see are trustworthy. (#271)

## Behind the Scenes

- **[Task]** **A safe testing environment using real-world data** — Setting up a read-only test environment loaded with production-like data, so changes can be verified confidently without any risk of altering live records. (#270)
- **[Feature]** **Turning meeting notes into tracked work automatically** — A helper that reads team conversations and files the resulting to-dos as tracked items, cutting down on manual copying. This is an internal workflow improvement. (#272)

## Offers

- **[Bug]** **Offer settings that weren't reaching the live widget** — Several saved offer options (including Modal-tab fields and a few backend flags) were being lost before they reached what visitors see. This work makes sure each one is either applied or cleanly removed. (#295)

## Modals

- **[Feature]** **Fixing the Modal Design tab** — Every field on the Modal Design tab is currently saved but has no effect on the visitor modal. This work will either make those header and progress-bar settings work or remove them, so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned compared to other forms. This cleanup will make text boxes, color pickers, checkboxes, and paired fields look consistent and properly laid out. (#152)

## Campaigns

- **[Feature]** **Bringing the Campaigns module into New Adsmith Frontend** — Campaign management isn't yet available in the new platform. This adds it back, letting you view, create, edit, and configure campaigns and their offer groups just as you could before. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
