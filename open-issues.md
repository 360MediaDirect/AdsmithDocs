# Open Issues — Plain-Language Overview

_Last updated 2026-06-26 19:33:33 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Reviewing an older stats job** — Checking whether a legacy background job that tracks certain sub-ID stats is still needed or can be retired, to keep reporting tidy. (#33)
- **[Feature]** **Rolling up historical performance data** — A new automated process will summarize daily performance into long-term totals so historical reports stay accurate and load reliably. (#35)
- **[Task]** **Side-by-side testing of the new lead-check system** — Running the new and old pre-ping systems together to confirm the new one behaves identically before switching over. (#40)
- **[Task]** **Speeding up the Survey Engine** — Adding a behind-the-scenes caching layer so placements, offers, and caps load faster during live traffic. High priority. (#42)
- **[Task]** **Running new scheduled tasks alongside the old ones** — The new automated background tasks will run in parallel with the existing ones so results can be compared before we rely on them. (#43)
- **[Task]** **Retiring older background tasks (first group)** — Turning off the lower-risk legacy scheduled jobs once their replacements have proven stable, with monitoring in place. (#44)
- **[Task]** **Retiring more background tasks (second group)** — Switching off additional legacy stats jobs after the first group is confirmed stable. (#45)
- **[Task]** **Retiring the most critical background tasks (final group)** — Carefully switching off the most important legacy jobs (lead processing and offer-cap resets) last, with close monitoring and quick rollback ready. (#46)
- **[Task]** **Documenting rollback steps** — Writing clear instructions to quickly revert any production system if something goes wrong. (#48)
- **[Task]** **Creating troubleshooting guides** — Preparing step-by-step guides for handling common issues such as lead-processing, stats, or offer-cap problems. (#49)

## Dashboard

- **[Feature]** **Live "today" numbers on the Dashboard** — The Dashboard's "today" view will show up-to-date impressions, clicks, leads, and revenue, correctly handled in Eastern time. (#34)
- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open a start and end date picker so you can view data for any specific period instead of only the preset ranges. (#58)
- **[Task]** **Restore missing Dashboard sections** — Bringing back the campaign stats, top offers, and watch list sections, all responding to the date range you select. High priority. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds "Offers with Legs" and CLP performance views (flagging offers converting under 30%), plus a searchable log of changes like pausing offers or adjusting caps. (#256)
- **[Task]** **Consistent Dashboard color scheme** — Applying a defined color palette across the Dashboard for clearer, easier-to-read views. (#263)

## General / Across the App

- **[Feature]** **Dark/light mode toggle** — You'll be able to switch the entire admin between dark and light themes, with your choice remembered between sessions. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, the app will lock it or warn you so one person's changes can't silently erase another's. This works across all entity screens. (#267)
- **[Task]** **Brand guidelines as the main input for AI output** — Establishing one comprehensive brand guide to drive higher-quality, more on-brand AI-generated content. (#264)
- **[Task]** **Users screen gap review** — Comparing the new Users area against the legacy one to identify missing features (such as bulk actions, last-login, and 2FA status) and plan what to add. A documentation/analysis task. (#80)
- **[Bug]** **Invalid link test should show an error** — Testing an invalid link currently sends you back to the dashboard; instead you'll see a clear error message explaining the link failed. (#239)

## Flows

- **[Task]** **Fix Flow form styling** — Correcting unstyled and misaligned elements on the Flow form so text boxes, color pickers, checkboxes, and paired fields look consistent with the other forms. Partially addressed, with the rest in progress. (#152)
- **[Feature]** **Clearer "Step order" setting** — Adding a plain-language label and inline help that explains what Step order controls and what its values mean, so it's understandable without outside documentation. (#226)

## Pre-Pings

- **[Feature]** **Per-advertiser pre-ping checks** — Validating each active advertiser's pre-ping setup (field mapping and success criteria) before it goes live, so issues are caught early. (#41)
- **[Feature]** **Enforce required fields before sending** — Leads missing required information will be stopped before a "Before Data Push" pre-ping is sent, rather than relying on the advertiser's system to reject them. (#218)

## Placements

- **[Feature]** **Better offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — Restores the ability to view, create, edit, and configure campaigns and offer groups (titles, questions, CTAs, offer handling, and more), matching the legacy system. High priority. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
