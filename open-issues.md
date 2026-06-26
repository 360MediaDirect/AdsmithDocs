# Open Issues — Plain-Language Overview

_Last updated 2026-06-26 21:29:35 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Review of an older stats tracking job** — We're checking whether a scheduled background process for certain tracking stats is still needed or can be retired, to keep things lean. (#33)
- **[Feature]** **More reliable historical reporting data** — Behind-the-scenes work to roll up daily numbers so historical reports stay accurate and load dependably. (#35)
- **[Task]** **Speed boost for Surveys** — Adding a caching layer so survey settings and offer data load faster during real-time use. This is high priority. (#42)
- **[Task]** **Running new background jobs alongside the old ones** — The updated scheduled jobs will run in parallel with the existing ones so we can confirm they match before fully switching over. (#43)
- **[Task]** **Switchover of lower-risk scheduled jobs** — Retiring an older survey-stats job once its replacement is proven stable, with the ability to switch back if needed. (#44)
- **[Task]** **Switchover of mid-tier scheduled jobs** — Retiring several stats-related background jobs after the first batch runs cleanly, with a week of monitoring. (#45)
- **[Task]** **Switchover of the most critical scheduled jobs** — Carefully retiring the most important background jobs (lead processing and offer-cap resets) last, with close monitoring and instant rollback ready. (#46)
- **[Task]** **Documented recovery steps** — Writing and testing clear procedures to safely roll back each major system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides for the support team** — Creating step-by-step guides for common issues like lead-processing or stats problems, so they can be resolved quickly. (#49)

## Dashboard

- **[Task]** **Restore missing dashboard sections** — Campaign stats, top offers, and watch lists will return to the dashboard and update when you change the date range. This is high priority. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — You'll get dedicated views for long-running ("Offers with Legs") and CLP offers, with under-30% converters flagged for attention, plus a searchable log of who changed what and when. (#256)
- **[Feature]** **Up-to-date "today" numbers** — The dashboard's "today" view will show current impressions, clicks, leads, and revenue so you can monitor performance live. (#34)
- **[Task]** **Custom date range on the dashboard** — Choosing "Custom" will open start and end date pickers so you can view any range you like, not just the preset options. (#58)
- **[Task]** **Consistent dashboard colors** — A defined color palette will be applied across the dashboard to make it easier to read at a glance. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole Admin between dark and light themes, with your choice remembered for next time. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — When someone else is already editing a record, you'll see who has it open and be prevented from silently saving over their changes. (#267)
- **[Bug]** **Clear error for invalid link tests** — Testing an invalid link currently drops you back on the dashboard; instead you'll see a clear failure message in the Link Testing screen. (#239)
- **[Task]** **Users screen review against the old system** — A documentation effort comparing the old and new Users management screens to plan which features still need to be carried over. (#80)
- **[Task]** **Brand guidelines for AI-generated output** — Establishing a thorough brand-guidelines document to use as the main input for AI features, improving the quality of generated content. (#264)

## Pre-Pings

- **[Feature]** **Block leads missing required information** — When a pre-ping runs before sending data, a lead that's missing required fields will be stopped upfront instead of relying on the advertiser to reject it. (#218)
- **[Feature]** **Per-advertiser pre-ping checks before go-live** — Each active advertiser's pre-ping setup will be validated so field mapping and success rules work correctly. (#41)
- **[Task]** **Side-by-side testing of the new pre-ping system** — Running the new and old systems together to compare results and fix any differences before the full switch. (#40)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain-language label and helpful inline text so you can tell exactly what it does and what its values mean. (#226)
- **[Task]** **Fix the Flow form's appearance** — Tidying up styling on the Flow form so text boxes, color pickers, checkboxes, and paired fields display correctly instead of looking unstyled or stacked. (#152)

## Placements

- **[Feature]** **Better control over offer order on placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — The new Admin will gain a full Campaigns area to create, edit, and manage campaigns and offer groups, matching what's available in the legacy system. This is high priority. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
