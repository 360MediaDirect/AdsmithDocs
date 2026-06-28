# Open Issues — Plain-Language Overview

_Last updated 2026-06-28 20:26:03 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Feature]** **Faster "today" numbers on the Dashboard** — Today's impressions, clicks, leads, and revenue will be pulled from a new live data source so the Dashboard reflects up-to-the-hour activity in the correct (Eastern) time. (#34)
- **[Feature]** **Automatic roll-up of daily history** — Activity data will be tallied into daily totals automatically, keeping historical reports accurate and quick to load. (#35)
- **[Task]** **Faster surveys and offer checks** — Behind-the-scenes caching will speed up how survey placements, offer details, and caps are looked up, making the experience snappier. High priority. (#42)
- **[Task]** **Smarter, more reliable pre-ping testing** — The new pre-ping system will be run alongside the existing one and compared to confirm it behaves correctly before switchover. (#40)
- **[Task]** **Pre-ping checks verified for every advertiser** — Each advertiser's pre-ping setup will be tested individually to confirm fields and pass/fail rules work as expected. (#41)
- **[Task]** **Review of an older stats job** — Behind-the-scenes review to decide whether a legacy tracking job is still needed or can be retired. (#33)
- **[Task]** **Phased switchover of scheduled jobs** — Updated scheduled processes will run in parallel with the old ones, with daily monitoring to catch any differences before fully relying on the new system. (#43)
- **[Task]** **Retiring the lowest-risk scheduled jobs first** — Older survey-stats jobs will be turned off after the replacements prove stable, with the ability to switch back if needed. (#44)
- **[Task]** **Retiring the mid-tier scheduled jobs** — A second batch of older stats jobs will be turned off and monitored for a week once the first round is proven. (#45)
- **[Task]** **Retiring the most critical scheduled jobs last** — The most important lead-processing and offer-cap jobs will be switched over carefully, with immediate rollback ready if anything looks off. Critical. (#46)
- **[Task]** **Documented recovery steps** — Clear rollback instructions will be written and tested for each major system so issues can be reversed quickly and safely. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Step-by-step guides will be created for handling lead-processing, stats, offer-cap, and connection problems. (#49)

## Dashboard

- **[Task]** **Custom date range on the Dashboard** — Choosing "Custom" in the date filter will open a start/end date picker so you can view results for any specific range, not just the preset options. (#58)
- **[Task]** **Restore the missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date-range selector will update them. High priority. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds an "Offers with Legs" view, a CLP performance view that flags offers converting under 30%, and a searchable log of changes like pausing offers or editing caps. (#256)
- **[Task]** **Cleaner, consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for easier reading at a glance. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch between dark and light themes from your account menu, and your choice will be remembered next time you sign in. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, the app will warn you if someone else is editing it and prevent one person's changes from silently replacing another's. (#267)
- **[Task]** **Brand guidelines to improve AI-generated output** — A complete brand-guidelines document will be used as the main input for AI features, leading to more on-brand results. (#264)

## Flows

- **[Task]** **Polished, consistent Flow form styling** — The Flow form's text boxes, color pickers, checkboxes, and side-by-side fields will be styled to match the rest of the app instead of appearing plain or broken. (#152)
- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain-language label and inline help explaining what it controls, so it's easy to understand without outside guidance. (#226)

## Campaigns

- **[Feature]** **Campaigns module added to the new app** — You'll be able to view, create, edit, and configure campaigns and offer groups in New Adsmith Frontend, matching what the legacy admin offered. Critical, high priority. (#200)

## Placements

- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and filtering by taxonomy to find offers faster. (#235)

## Pre-Pings

- **[Feature]** **Required fields enforced before sending** — When a pre-ping requires certain fields, a lead missing those fields will be stopped up front instead of being sent out and left to the advertiser to reject. (#218)

## Link Testing

- **[Bug]** **Clear error for invalid links** — Testing an invalid link will show a proper failure message in Link Testing rather than sending you back to the Dashboard. (#239)

## Users

- **[Task]** **Review of Users screen against the legacy version** — A comparison of the old and new Users screens to identify missing features (like bulk actions and extra columns) and plan what to bring over. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
