# Open Issues — Plain-Language Overview

_Last updated 2026-06-26 09:04:47 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Decide the future of an older stats job** — We're checking whether a legacy job that tracks certain stats is still needed or can be retired now that newer reporting handles it. No visible change; this just keeps reporting tidy. (#33)
- **[Feature]** **Faster "today" numbers** — Groundwork so the Dashboard's "today" view can show up-to-the-hour impressions, clicks, leads, and revenue (in Eastern Time). (#34)
- **[Feature]** **Reliable historical reporting totals** — Behind-the-scenes work to roll up daily numbers so longer-range reports stay accurate and quick. (#35)
- **[Task]** **Safety testing for pre-pings** — We'll run the new pre-ping process alongside the existing one to confirm they produce the same results before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Each active advertiser's pre-ping will be validated for correct field mapping and pass/fail handling before the switchover. (#41)
- **[Task]** **Speed improvements for surveys** — Adding a caching layer so surveys load and respond faster, especially under heavy traffic. High priority. (#42)
- **[Task]** **Run new scheduled jobs in parallel** — New automated jobs will run side-by-side with the current ones so we can confirm everything matches before relying on them. (#43)
- **[Task]** **Gradual switchover of scheduled jobs (first group)** — Retiring the least-risky legacy automated jobs once their replacements prove stable, with monitoring in place. (#44)
- **[Task]** **Gradual switchover of scheduled jobs (next group)** — Retiring the next set of legacy stats jobs after the first group is confirmed stable. (#45)
- **[Task]** **Gradual switchover of scheduled jobs (most critical group)** — Carefully retiring the most important legacy jobs last, with close monitoring and the ability to revert instantly. (#46)
- **[Task]** **Document how to revert safely** — Writing clear step-by-step recovery procedures for each major system in case something needs to be rolled back. (#48)
- **[Task]** **Create troubleshooting guides** — Preparing quick-reference guides so the team can resolve common issues (like lead-processing or stats hiccups) faster. (#49)

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open a start/end date picker so you can view Dashboard data for any range you want, not just preset options. The selected range will show on the filter button. (#58)
- **[Feature]** **Light mode option** — You'll be able to switch between the current dark theme and a new light theme from your user menu, with your choice remembered next time you log in. (#59)
- **[Task]** **Bring back missing Dashboard sections** — Restores the campaign stats, top offers, and watch list sections so the Dashboard shows full reporting again, with the date range updating them. High priority. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds dedicated views for long-running offers and CLP offer performance (flagging those converting under 30%), plus a searchable log of changes like pausing offers or adjusting caps. (#256)
- **[Task]** **Consistent Dashboard colors** — Applies a defined color palette across the Dashboard for cleaner, easier-to-read visuals. (#263)

## General / Across the App

- **[Task]** **Users screen comparison review** — A documentation review comparing the older Users area with the new one to spot missing features (like bulk actions, last-login, and 2FA status) so they can be prioritized. (#80)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper error message in the Link Testing screen instead of sending you back to the Dashboard. (#239)
- **[Task]** **Stronger brand guidelines for AI output** — Establishing a single, detailed brand-guidelines document to use as the main input for AI-generated content, improving the quality and consistency of results. (#264)
- **[Feature]** **Prevent two people from overwriting each other** — When two users open the same record, you'll see who's currently editing it and be warned before saving over someone else's changes. This protection will work across all the main edit screens. (#267)

## Offers, Placements & Campaigns

- **[Feature]** **Campaigns module in the new app** — Brings back full campaign management—creating, editing, and configuring campaigns and offer groups—so you can manage campaigns just like in the previous system. High priority. (#200)
- **[Feature]** **Better control of selected offers on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)
- **[Feature]** **Enforce required pre-ping fields before sending** — A lead missing required pre-ping fields will be stopped before the request is sent, matching how offer display already works, so incomplete leads don't slip through. (#218)

## Flows

- **[Task]** **Fix the look of the Flow form** — Cleans up styling on the Flow form so text boxes, color pickers, checkboxes, and paired fields display correctly and consistently with other forms. (#152)
- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain-language label and helpful inline guidance explaining what it controls, so it's easy to understand without outside help. (#226)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
