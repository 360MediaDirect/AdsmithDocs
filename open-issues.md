# Open Issues — Plain-Language Overview

_Last updated 2026-06-28 07:19:57 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard date filter** — Choosing "Custom" will open a proper start- and end-date picker so you can view Dashboard data for any range you like, instead of being limited to preset options like Today or This Month. (#58)
- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the Admin area between the current dark theme and a new light theme, with your choice remembered next time you sign in. (#59)
- **[Task]** **Restore missing Dashboard sections** — A high-priority fix to bring back the campaign stats, top offers, and watch list sections, so the Dashboard shows full reporting again and responds to your date-range selection. (#240)
- **[Feature]** **New "Other Dashboard" views and change history** — Adds dedicated views for "Offers with Legs" and CLP offer performance (flagging offers converting under 30%), plus a searchable log of offer and system changes for easier auditing. (#256)
- **[Task]** **Consistent Dashboard color scheme** — A defined set of colors will be applied across the Dashboard for cleaner, easier-to-read visuals. (#263)

## Behind the Scenes

- **[Feature]** **Up-to-date "today" stats** — Behind-the-scenes work so today's impressions, clicks, leads, and revenue display accurately and in the correct time zone. (#34)
- **[Feature]** **Faster historical reporting** — Maintenance that rolls up daily totals so historical stats load reliably. (#35)
- **[Task]** **Performance caching for Surveys** — Behind-the-scenes speed improvements so survey-related screens respond faster. High priority. (#42)
- **[Task]** **Pre-ping accuracy testing** — Running the new pre-ping process alongside the existing one to confirm results match before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each advertiser's pre-ping behaves correctly ahead of the switchover. (#41)
- **[Task]** **Review an older stats job** — Checking whether a legacy scheduled stats process is still needed or can be retired. (#33)
- **[Task]** **Roll out updated scheduled jobs** — Running the new automated jobs alongside the current ones to confirm they behave identically. (#43)
- **[Task]** **Switch over scheduled jobs (group 3)** — Retiring the lowest-risk legacy scheduled job once its replacement is proven stable. (#44)
- **[Task]** **Switch over scheduled jobs (group 2)** — Retiring the next set of legacy stats jobs after a monitoring period. (#45)
- **[Task]** **Switch over scheduled jobs (group 1, critical)** — Retiring the most critical legacy jobs last, with close monitoring and a quick way to revert. (#46)
- **[Task]** **Document recovery procedures** — Writing and testing step-by-step recovery plans for each core system. (#48)
- **[Task]** **Create troubleshooting guides** — Preparing reference guides for quickly resolving common operational issues. (#49)

## General / Across the App

- **[Feature]** **Prevent overwriting each other's edits** — When two people open the same record, the app will warn that someone else is editing and stop one person's changes from silently wiping out another's, across all entity screens. (#267)
- **[Task]** **Brand guidelines to improve AI output** — Establishing a single, detailed brand-guidelines document to feed AI-generated content, so results are more on-brand. (#264)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — A styling fix so text boxes, color pickers, checkboxes, and paired fields look consistent with the rest of the app instead of appearing unstyled or misaligned. (#152)
- **[Feature]** **Make the "Step order" setting understandable** — A clearer label and inline help text will explain what Step order controls and what its values do, so it's no longer confusing. (#226)

## Pre-Pings

- **[Feature]** **Enforce required fields before sending** — When a pre-ping is set to run before a data push, leads missing required fields will be stopped right away rather than relying on the advertiser's response, preventing incomplete leads from slipping through. (#218)

## Placements

- **[Feature]** **Better control over selected offers** — Selected offers will default to manual order, support drag-and-drop reordering, include an "X" to remove an offer, and allow filtering the offer list by taxonomy. (#235)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — A high-priority addition to recreate campaign management in New Adsmith Frontend, letting you view, create, edit, and configure campaigns and offer groups as in the previous system. (#200)

## Users

- **[Task]** **Compare the Users area to the previous version** — A documentation review identifying which Users features from the older system are still missing, to guide future work. (#80)

## Link Testing

- **[Bug]** **Show an error for invalid links** — Testing an invalid link will now display a clear error instead of unexpectedly sending you to the Dashboard. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
