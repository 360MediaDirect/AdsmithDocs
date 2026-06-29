# Open Issues — Plain-Language Overview

_Last updated 2026-06-29 11:39:42 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes
- **[Task]** **Review an older stats-tracking job** — Checking whether a long-running background process that records certain stats is still needed or can be retired, with no change to what you see. (#33)
- **[Feature]** **Up-to-the-hour numbers for "today"** — Lays the groundwork to show current-day figures (impressions, clicks, leads, revenue) more accurately on the Dashboard. (#34)
- **[Feature]** **Faster historical reporting** — A behind-the-scenes routine that summarizes daily stats so historical reports load more quickly. (#35)
- **[Task]** **Side-by-side test of the new lead pre-check** — Running the new pre-ping process alongside the current one to confirm they produce matching results before switching over. (#40)
- **[Feature]** **Pre-ping verification for each advertiser** — Confirming lead pre-checks behave correctly for every active advertiser before the switch, so nothing breaks at go-live. (#41)
- **[Task]** **Speed boost for the Survey engine** — Adding a fast-access layer so surveys, offers, and caps respond more quickly. A high-priority improvement. (#42)
- **[Task]** **Run new scheduled jobs in parallel** — Operating the new automated jobs alongside the existing ones and watching for any differences before relying on them. (#43)
- **[Task]** **Switch over lower-risk scheduled jobs first** — Turning off the older survey-stats job once its replacement proves stable, with the ability to switch back if needed. (#44)
- **[Task]** **Switch over the next group of scheduled jobs** — Retiring several older stats jobs once the earlier round is confirmed stable, monitored over a week. (#45)
- **[Task]** **Switch over the most critical scheduled jobs last** — Carefully retiring the core lead-processing and offer-cap jobs, watched closely with an immediate fallback ready. (#46)
- **[Task]** **Document recovery steps** — Writing clear "how to undo" procedures for each major system so the team can quickly restore service if something goes wrong. (#48)
- **[Task]** **Create troubleshooting guides** — Step-by-step guides for handling common issues like lead-processing or stats problems, helping the team resolve incidents faster. (#49)

## Dashboard
- **[Task]** **Restore the missing Dashboard sections** — Bringing back campaign stats, top offers, and watch lists so the Dashboard shows full reporting again, with the date range updating them. A high-priority fix. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds an "Offers with Legs" view and a CLP performance view (flagging offers converting under 30%), plus a searchable log of changes like pausing offers or editing caps, showing who changed what and when. (#256)
- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open a start/end date picker so you can view Dashboard data for exactly the period you want. (#58)
- **[Task]** **Consistent Dashboard colors** — Applying a defined color palette across the Dashboard for cleaner, easier-to-read visuals. (#263)

## General / Across the App
- **[Feature]** **Light and dark mode toggle** — You'll be able to switch the entire Admin between dark and light themes from your account menu, with your choice remembered next time. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, you'll see who's currently editing it and be warned if it changed since you opened it, preventing accidental loss of someone's work across offers, flows, placements, advertisers, and more. (#267)
- **[Task]** **Stronger brand guidelines for AI output** — Establishing a thorough brand-guidelines document to use as the main input for AI-generated content, improving quality and consistency. (#264)

## Flows
- **[Task]** **Tidy up the Flow form's appearance** — Fixing styling so text boxes, color pickers, checkboxes, and paired fields look polished and consistent with the Placement and Modal forms instead of appearing unstyled. (#152)
- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain-language label and helpful inline text explaining what it controls, so it's no longer confusing to use. (#226)

## Campaigns
- **[Feature]** **Bring back the Campaigns module** — Adds the missing Campaigns area so you can view, create, edit, and configure campaigns and their offer groups, matching what the legacy admin offered. A critical, high-priority addition. (#200)

## Placements
- **[Feature]** **Better offer selection and ordering** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer (so clicking no longer removes it), and a way to filter the offer list by taxonomy. (#235)

## Pre-Pings
- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping runs before pushing data, leads missing required fields will be stopped right away instead of being sent on, preventing incomplete leads from slipping through. (#218)

## Link Testing
- **[Bug]** **Show an error for invalid links** — Testing an invalid link will now display a clear failure message instead of unexpectedly sending you to the Dashboard. (#239)

## Users
- **[Task]** **Compare the Users area to the legacy version** — A review documenting which Users features are still missing (such as bulk actions and certain columns) to guide upcoming improvements. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
