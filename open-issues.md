# Open Issues — Plain-Language Overview

_Last updated 2026-06-28 12:26:38 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Restore the missing dashboard sections** — Right now only the system overview loads. This will bring back campaign stats, top offers, and watch lists, and make sure the date-range selection actually updates them. High priority. (#240)
- **[Task]** **Custom date range on the dashboard filter** — Choosing "Custom" will now open a proper start/end date picker so you can view dashboard data for any range you like, not just the preset options. (#58)
- **[Feature]** **New "Other Dashboard" views plus an activity log** — Adds an "Offers with Legs" view and a "CLP Performance" view (highlighting offers converting under 30%), along with a searchable record of changes like pausing offers or adjusting caps, so admins can see who changed what and when. (#256)
- **[Feature]** **Dark/light mode toggle** — You'll be able to switch the whole admin between dark and light themes from your user menu, and your choice will stick across sessions. (#59)
- **[Task]** **Consistent dashboard colors** — A defined color palette will be applied across dashboard views for easier reading and a more polished look. (#263)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain-language label and helpful inline text so you can understand what it controls without needing outside documentation. (#226)
- **[Task]** **Tidy up the Flow form's appearance** — Fixes styling gaps on the Flow form so text boxes, color pickers, checkboxes, and paired fields display correctly and match the look of the Placement and Modal forms. (#152)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is editing a record (an offer, flow, placement, advertiser, and so on), others will see it's locked and by whom, and the system will warn you if a record changed while you had it open—so no one's work gets silently erased. (#267)
- **[Task]** **Adopt brand guidelines for AI output** — A single, comprehensive brand-guidelines document will be used to guide AI-generated content, improving the quality and consistency of results. (#264)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — The Campaigns area from the legacy admin isn't available yet. This adds it back so you can create, edit, and manage campaigns and offer groups as before. Critical, high priority. (#200)

## Pre-Pings

- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping is set to run before a data push, leads missing required information will now be stopped up front instead of being sent out and relying on the advertiser to catch the problem. (#218)

## Placements

- **[Feature]** **Better control over selected offers** — Selected offers will default to manual ordering with drag-and-drop reordering, a clear "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)

## Link Testing

- **[Bug]** **Show a clear error for invalid links** — Testing an invalid link currently dumps you on the dashboard. This fix will show a proper failure message in the Link Testing screen instead. (#239)

## Users

- **[Task]** **Compare the new Users area to the legacy version** — A review identifying which Users features still need to be added (such as bulk actions, last-login info, and password options) so the new screen can match what users had before. Documentation/planning work. (#80)

## Behind the Scenes

- **[Feature]** **Faster, accurate "today" stats** — Behind-the-scenes work to pull current-day numbers (impressions, clicks, leads, revenue) more reliably for the dashboard's "today" view. (#34)
- **[Feature]** **Reliable historical reporting totals** — Maintenance to roll up daily numbers correctly so longer-term reports stay accurate. (#35)
- **[Task]** **Speed improvements for surveys** — Adds a caching layer so survey-related screens load faster. High priority. (#42)
- **[Feature]** **Pre-ping checks for each advertiser** — Verifying that pre-ping setup works correctly for every active advertiser before switching over. (#41)
- **[Task]** **Side-by-side pre-ping testing** — Running the new pre-ping process alongside the old one to confirm results match before the switch. (#40)
- **[Task]** **Run new scheduled jobs alongside the old ones** — Deploying the new background jobs in parallel with the existing ones and monitoring for any differences. (#43)
- **[Task]** **Phased switch-over of scheduled jobs (lower risk)** — Retiring the lower-priority background jobs once their replacements prove stable. (#44)
- **[Task]** **Phased switch-over of scheduled jobs (mid-tier)** — Retiring the next set of background jobs, including stats aggregation and reporting, after monitoring. (#45)
- **[Task]** **Phased switch-over of scheduled jobs (critical)** — Carefully retiring the most critical background jobs (lead processing and offer-cap resets) last, with the ability to roll back instantly. Critical. (#46)
- **[Task]** **Review an old stats job** — Checking whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Document rollback steps** — Writing and testing clear recovery procedures for each system in case something needs to be reverted. (#48)
- **[Task]** **Troubleshooting guides for support** — Creating step-by-step guides for handling common issues like lead-processing or stats hiccups. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
