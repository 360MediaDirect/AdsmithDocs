# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 13:32:26 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record to edit it, others will see it's already being worked on and be warned before they can accidentally save over those changes. This protects your work across every entity screen (Offers, Flows, Placements, Advertisers, and more). (#267)
- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every change made to records across the app — by people or by automated jobs — with a timestamp and who did it. You'll be able to search it and see a history right on each record, making "who changed this and when?" easy to answer. (#276)
- **[Feature]** **Clean up settings that don't actually do anything** — Certain controls (like the Advertiser Web Presence fields, some user permission toggles, and a few Data Client and Pre-Ping options) currently save but have no effect. These will be removed or hidden so you're never misled by a setting that does nothing. (#296)
- **[Bug]** **Bad links in Link Testing now show a clear error** — Today, entering an invalid link quietly sends you to the dashboard. After this fix you'll get a proper failure message so you know the link didn't work. (#239)
- **[Task]** **Bring the Users area up to par with the old system** — A review comparing the old Users screen to the new one, so missing tools (like bulk actions and extra columns) can be planned and added. (#80)
- **[Task]** **Decide the future of the old file-share page** — A quick check on whether the legacy file-share page is still needed, so it's either rebuilt in the new app or intentionally retired. (#328)

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on an offer's success step currently never fire, meaning some conversions go unrecorded. This high-priority fix makes them fire reliably so your attribution and reporting stay accurate. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several offer options you can set (including Modal-tab fields, Display URL, and certain Data Client flags) are saved but dropped before they reach visitors. Each will be properly wired through or removed so what you save is what actually happens. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently ignore age, gender, state, zip, and device targeting, so they can fire for people who should be excluded. This work makes them follow the same targeting rules as regular offers (once legacy behavior is confirmed). (#333)
- **[Feature]** **Preview offers and placements with your unsaved changes** — The Preview button will show the edits you're currently making, instead of only the last saved version — so you can check a change before committing it. (#292)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool that estimates a new offer's likely performance based on your historical offer data, replacing the informal manual gut-check with a data-driven projection. (#322)

## Surveys

- **[Feature]** **Make every survey design option actually take effect** — A thorough pass to ensure every customization on the Design tab is reflected in the live survey, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live survey** — Options like iFrame Height, Display Format, and a few style toggles are saved but not yet applied. Each will be wired into the survey or removed from the form. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore after-success delivery for data clients** — The legacy post-conversion delivery/redirect behavior wasn't carried over. This adds it back as a reusable, configurable option so your active data clients keep working as before. (#327)
- **[Feature]** **Bring legacy pre-ping validation checks to the new platform** — Hundreds of data clients rely on custom serve-time checks that don't run yet in the new app. This high-priority work reconnects those checks so the right visitors are validated before offers are served. (#338)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging version of the product using production-like data that can't be changed, so testing and verification can happen without touching live data. (#270)
- **[Feature]** **Turn conversations into tracked to-dos automatically** — A helper that reads team chat and files the resulting action items as tracked issues, cutting out manual copy-and-paste. (#272)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — Campaign management from the old admin isn't in the new platform yet. This high-priority work adds the ability to view, create, edit, and configure campaigns and their offer groups. (#200)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or awkwardly stacked. This tidies up the layout so it matches the polished look of the Placement and Modal forms. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design tab's settings currently have no effect on what visitors see. They'll either be connected to the live modal or removed so the tab isn't misleading. (#294)

## Reports

- **[Task]** **Confirm dashboard report numbers match the old system** — An investigation into why some dashboard figures differed from the legacy app, to find the cause and either fix it or confirm the numbers are correct. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
