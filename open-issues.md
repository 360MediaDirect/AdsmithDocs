# Open Issues — Plain-Language Overview

_Last updated 2026-06-29 20:37:04 UTC · 33 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Tidy up an outdated background reporting job** — We're checking whether an older stats-tracking job is still needed or can be retired now that newer reporting handles the same work. No change you'll see; it keeps reporting lean and reliable. (#33)
- **[Feature]** **Faster "today" numbers on the Dashboard** — Behind-the-scenes work so that today's impressions, clicks, leads, and revenue can be pulled in real time for the Dashboard's "today" view. (#34)
- **[Feature]** **Smarter rollups for historical reporting** — Day-to-day stats will be summarized automatically so longer-range reports load accurately and quickly. (#35)
- **[Task]** **Safety testing for pre-ping before go-live** — We'll run the new pre-ping system alongside the existing one and compare results to make sure offers are checked correctly before any switchover. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — We're verifying pre-ping works correctly for each active advertiser so lead validation behaves as expected once live. (#41)
- **[Task]** **Speed improvements for the Survey engine** — Adding a caching layer so surveys, offers, and caps respond faster during real-time use. (#42)
- **[Task]** **Roll out new automated background jobs** — Deploying the new scheduled jobs to run side-by-side with the current ones while we confirm they match. (#43)
- **[Task]** **Retire older background jobs — group 3** — Switching off a lower-risk set of legacy scheduled jobs once their replacements prove stable. (#44)
- **[Task]** **Retire older background jobs — group 2** — Turning off another set of legacy stats jobs after the first group is confirmed healthy. (#45)
- **[Task]** **Retire the most critical background jobs — group 1** — Carefully switching off the most important legacy jobs (lead processing and offer-cap resets) last, with close monitoring. (#46)
- **[Task]** **Write step-by-step recovery procedures** — Documenting how to safely roll back each system if something goes wrong, so issues can be resolved quickly. (#48)
- **[Task]** **Create troubleshooting guides for the support team** — Practical guides for handling common situations like lead-processing or stats hiccups. (#49)
- **[Task]** **Set up a safe testing environment with May & June data** — A staging copy loaded with real past data so reports can be validated without touching live information. (#270)
- **[Task]** **Confirm new reports match the legacy system** — Investigating any differences between old and new report numbers to pin down and fix the cause, so you can trust the figures. (#271)
- **[Feature]** **Auto-create tasks from Slack conversations** — An internal helper that turns discussion points into tracked work items, so requests don't get lost. (#272)
- **[Task]** **Streamline the testing checklist** — Trimming the review list down to outstanding items only, making the next round of testing quicker and clearer. (#273)

## Dashboard

- **[Task]** **Custom date range on the Dashboard** — Selecting "Custom" will open a proper start/end date picker so you can view Dashboard data for any range you choose, with the selected range shown on the filter. (#58)
- **[Task]** **Bring back missing Dashboard sections** — Restores campaign stats, top offers, and watch lists to the Dashboard, with the date range updating them as expected. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds "Offers with Legs" and CLP performance views (flagging offers converting under 30%) plus a searchable log of offer and system changes for easy auditing. (#256)
- **[Task]** **Consistent Dashboard colors** — A defined color palette applied across the Dashboard for cleaner, more readable visuals. (#263)
- **[Feature]** **Change report dates without editing the address bar** — Date controls move right into the Dashboard toolbar, so you can pull daily or custom reports from the screen itself while links stay shareable. (#268)
- **[Feature]** **Dashboard links open in a new tab** — Clicking a Dashboard link will open it in a new tab so you don't lose your place or have to navigate back. (#269)

## General / Across the App

- **[Feature]** **Light mode option** — A toggle to switch between the current dark theme and a new light theme, applied across the whole admin and remembered for next time. (#59)
- **[Task]** **Review the Users area against the old system** — A side-by-side comparison to spot any missing Users features (like bulk role changes or last-login info) and plan what to add. (#80)
- **[Feature]** **Bring back the Campaigns module** — Restores the ability to create, edit, and manage campaigns and offer groups, matching what's available in the legacy admin. (#200)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will show a proper failure message instead of unexpectedly dropping you on the Dashboard. (#239)
- **[Task]** **Use brand guidelines to improve AI output** — Establishing a single, detailed brand guide as the main input so AI-generated content stays on-brand. (#264)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is already editing a record, others will see a clear "locked by" notice, and saves are checked so one person's changes can't silently wipe out another's. Works across offers, flows, placements, advertisers, and more. (#267)

## Offers & Placements

- **[Feature]** **Stop incomplete leads at pre-ping** — Pre-pings set to run before pushing data will block leads that are missing required fields, instead of letting them through. (#218)
- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an X to remove an offer, and the ability to filter the offer list by taxonomy. (#235)
- **[Task]** **Quick action links under each offer** — Adds handy per-offer links (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an offer activity page showing lead and revenue performance over time. (#252)

## Flows

- **[Task]** **Fix the look of the Flow form** — Cleans up styling issues so textareas, color pickers, checkboxes, and paired fields display properly and consistently. (#152)
- **[Feature]** **Make "Step order" easy to understand** — Adds a clear label and inline help explaining what the Step order setting controls and what its values do, so it's no longer confusing. (#226)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f20046605f5d85cfb8232efa7f79ba4ded38c3ba1b38cba2aab08d7c61c24ae9 -->
