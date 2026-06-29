# Open Issues — Plain-Language Overview

_Last updated 2026-06-29 22:24:17 UTC · 33 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a proper start- and end-date picker, so you can view dashboard data for any range you like instead of only the preset options. (#58)
- **[Task]** **Bring back the missing dashboard sections** — Restores the campaign stats, top offers, and watch-list sections so the Dashboard shows full reporting again, with the date range updating them as expected. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds dedicated views for long-running ("Offers with Legs") and CLP offer performance, highlights CLP offers converting under 30%, and gives admins a searchable record of changes like pausing offers or editing caps. (#256)
- **[Task]** **A consistent dashboard color scheme** — The Dashboard will adopt a defined set of colors applied across all views to make the numbers easier to read at a glance. (#263)
- **[Feature]** **Pick report dates without editing the web address** — Adds date controls right in the dashboard toolbar so you can pull daily or custom-range reports through the interface; the address bar still updates so links stay shareable. (#268)
- **[Feature]** **Dashboard links open in a new tab** — Clicking a link on the Dashboard opens it in a new browser tab so you don't lose your place or current view. (#269)

## General / Across the App

- **[Feature]** **Light mode for the Admin area** — Adds a switch to toggle between the current dark theme and a new light theme, with your choice remembered across sessions for comfort in any lighting. (#59)
- **[Task]** **Review of the Users screens vs. the old system** — A behind-the-scenes comparison of the legacy Users area against the new one to map out what's missing (like bulk actions and last-login info) and plan what to add. (#80)
- **[Bug]** **Invalid links should show an error, not send you to the Dashboard** — Testing a bad link will return a clear failure message in Link Testing instead of quietly dropping you on the Dashboard. (#239)
- **[Task]** **Stronger brand guidelines for AI-generated content** — Establishes a single, detailed brand-guidelines document to feed the AI, improving the quality and consistency of its output. (#264)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is already editing a record, others will see it as locked with a clear note of who has it open, and a safeguard will warn you if a record changed while you had it open—so no one's work gets silently overwritten. (#267)

## Pre-Pings

- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping runs before a lead is pushed, leads missing required information will be stopped up front rather than relying on the advertiser to reject them. (#218)
- **[Bug]** **Close a gap where hidden offers still recorded a lead** — Fixes a case where an auto-register offer was correctly hidden by its pre-ping check but still recorded a successful lead and revenue; the same field check will now apply to both paths. (#274)
- **[Task]** **Side-by-side testing of the new pre-ping system** — The new pre-ping process will run alongside the existing one and have its results compared, so any differences are caught and fixed before it fully takes over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Each active advertiser's pre-ping will be verified for correct field mapping and pass/fail handling, ensuring leads are evaluated accurately for every advertiser. (#41)

## Reports

- **[Feature]** **Live "today" numbers** — Adds up-to-the-hour impressions, clicks, leads, and revenue for the current day so the "today" view reflects what's happening right now (in Eastern Time). (#34)
- **[Feature]** **Reliable historical totals** — Rolls up daily activity into a stored history so past-date reports load consistently and accurately over time. (#35)
- **[Task]** **Confirm new reports match the old system** — An investigation comparing report numbers between the legacy and new platforms over a fixed date range to find and explain any differences, building trust in the new figures. (#271)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Fixes styling on the Flow form so text boxes, color pickers, checkboxes, and paired fields display cleanly and consistently with the Placement and Modal forms. (#152)
- **[Feature]** **Explain what "Step order" does** — Adds a clearer label and inline help text so you can understand what the Step order setting controls and what its values mean, without needing outside documentation. (#226)

## Offers

- **[Task]** **Quick action links under each offer** — Brings back handy per-offer links like Edit, Quick Edit, Trash, View, Preview, Details, and Trends—where Trends opens a performance page showing leads, revenue, and a daily breakdown. (#252)

## Placements

- **[Feature]** **Reorder selected offers by hand** — When choosing offers for a placement, you'll be able to set a manual order, drag offers into the sequence you want, remove them with an X, and filter the list by category. (#235)

## Campaigns

- **[Feature]** **Add the missing Campaigns area** — Brings the Campaigns module into the new platform so you can view, create, edit, and configure campaigns and their offer groups—matching what the legacy admin offered today. (#200)

## Behind the Scenes

- **[Task]** **Review of an older stats job** — Checking whether a legacy statistics process is still needed or can be retired, with the decision documented. (#33)
- **[Task]** **Faster Survey loading** — Adding a caching layer so survey configurations, offers, and caps load more quickly during real-time checks. (#42)
- **[Task]** **Prepare new scheduled jobs in production** — Running the new automated jobs alongside the existing ones so they can be monitored before any switchover. (#43)
- **[Task]** **Retire older scheduled jobs (first group)** — Turning off a set of lower-risk legacy survey-stats jobs once their replacements prove stable, with monitoring in place. (#44)
- **[Task]** **Retire older scheduled jobs (second group)** — Turning off additional legacy stats jobs after the first group is confirmed stable, monitored over a week. (#45)
- **[Task]** **Retire the most critical scheduled jobs (final group)** — Carefully switching off the most important legacy jobs last, with close monitoring and the ability to roll back immediately if needed. (#46)
- **[Task]** **Documented recovery steps** — Writing and testing clear roll-back procedures for each production system so issues can be reversed quickly. (#48)
- **[Task]** **Troubleshooting guides for the team** — Creating step-by-step guides for handling common operational issues like lead-processing or stats hiccups. (#49)
- **[Task]** **A safe testing environment with real data** — Setting up a staging environment loaded with May and June data so reports can be validated without touching live information. (#270)
- **[Feature]** **Auto-create tasks from team chats** — A helper that reads team conversations and turns action items into tracked tasks automatically, reducing manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 56ddbb502ca50defbf7da98b1a4c3995bb155bd4db5eb9d09e35f32e9f7b0d9e -->
