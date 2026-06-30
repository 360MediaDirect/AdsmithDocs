# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 00:35:01 UTC · 33 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard** — Choosing "Custom" in the date filter will open a proper start/end date picker, so you can view Dashboard data for any range you like instead of only preset options like Today or This Month. (#58)
- **[Feature]** **Light mode option for the Admin** — A new theme switcher will let you flip between the current dark look and a new light look, with your choice remembered next time you sign in. (#59)
- **[Task]** **Bring back the missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date selector will update them. A high-priority fix so the Dashboard once again shows the full picture rather than just the system overview. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — You'll get dedicated views for "Offers with Legs" and CLP offer performance (flagging offers converting under 30%), plus a searchable log of every offer change so you can see who paused an offer or adjusted a cap and when. (#256)
- **[Task]** **Consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for cleaner, easier-to-read visuals. (#263)
- **[Feature]** **Pick report dates without touching the address bar** — Date and day selection will live right in the Dashboard toolbar, so you no longer have to hand-edit the web address to pull a specific day's report. The link still updates so you can share or bookmark it. (#268)
- **[Feature]** **Dashboard links open in a new tab** — Clicking a link on the Dashboard will open it in a new browser tab, so you keep your place and don't lose your current view. (#269)

## Offers & Placements

- **[Feature]** **Stop incomplete leads at the pre-ping step** — When a pre-ping is set to run before data is pushed, leads missing required fields will now be blocked up front rather than slipping through to the advertiser. (#218)
- **[Feature]** **Better offer ordering on Placements** — The selected-offers list will default to manual order with drag-and-drop reordering, a clear "X" to remove an offer, and the ability to filter the offer list by taxonomy — making it much easier to arrange offers exactly how you want. (#235)
- **[Task]** **Quick action links under each offer** — Familiar shortcuts (Edit, Quick Edit, Trash, View, Preview, Trends, Details) will appear beneath each offer title, with Trends opening an Offer Activity page showing lead and revenue trends and a daily performance breakdown. (#252)
- **[Bug]** **Hidden offers should not record as successful** — Fixes a case where an offer correctly hidden by a pre-ping could still auto-submit and record a successful lead. This ensures hidden offers don't quietly generate transactions. (#274)

## General / Across the App

- **[Feature]** **Campaigns management is coming to the new app** — The Campaigns module from the legacy admin will be rebuilt here, letting you view, create, edit, and configure campaigns and their offer groups. A high-priority addition since campaign management isn't yet possible in the new app. (#200)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit, others will see it's locked, and a safety check on save will warn you if someone changed it while you had it open — so edits no longer get silently lost. (#267)
- **[Task]** **Users area review** — A side-by-side comparison of the legacy Users screens against the new ones, used to plan which Users features (like bulk actions and additional columns) still need to be added. (#80)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper failure message instead of unexpectedly sending you back to the Dashboard. (#239)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Cleans up styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields display neatly and consistently, matching the look of the Placement and Modal forms. (#152)
- **[Feature]** **Explain the "Step order" setting** — The Step order control will get a clear label and helpful inline text explaining what it does and what its values mean, so it's no longer a mystery to users. (#226)

## Behind the Scenes

- **[Feature]** **Faster "today" numbers** — Behind-the-scenes work to power the Dashboard's "today" view with up-to-date impressions, clicks, leads, and revenue in Eastern Time. (#34)
- **[Feature]** **Reliable historical totals** — Maintenance to roll up activity into daily totals so historical reports stay accurate. (#35)
- **[Task]** **Speed improvements for surveys** — Adds a caching layer so survey placements and offers load faster during live traffic. (#42)
- **[Task]** **Review an old stats job** — Checking whether a legacy background task is still needed or can be retired. (#33)
- **[Task]** **Side-by-side pre-ping testing** — Running the new pre-ping process alongside the old one to confirm it behaves identically before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each advertiser's pre-ping works correctly ahead of the switchover. (#41)
- **[Task]** **Run new and old scheduled jobs together** — Deploying the new background jobs to run in parallel with the existing ones, watching for any differences. (#43)
- **[Task]** **Switch over the lightest background jobs first** — Retiring the lowest-risk legacy survey-stats job once its replacement is proven stable. (#44)
- **[Task]** **Switch over the mid-tier background jobs** — Retiring several legacy stats jobs after the first wave is confirmed stable. (#45)
- **[Task]** **Switch over the most critical background jobs last** — Carefully retiring the core lead-processing and offer-cap jobs, with monitoring and the ability to roll back instantly. (#46)
- **[Task]** **Document how to undo changes** — Writing clear rollback steps for each major system in case something needs to be reversed. (#48)
- **[Task]** **Troubleshooting guides** — Creating step-by-step guides for handling common issues like lead-processing or stats problems. (#49)
- **[Task]** **Adopt brand guidelines for AI output** — Establishing a comprehensive brand guide to use as the main input for AI-generated content, improving quality and consistency. (#264)
- **[Task]** **Set up a safe testing environment** — Standing up a staging area loaded with May and June data so reports can be checked without touching live information. (#270)
- **[Task]** **Confirm the numbers match the legacy system** — Comparing reports between the old and new platforms to find and explain any differences and confirm the data lines up. (#271)
- **[Feature]** **Turn meeting notes into tracked tasks automatically** — A helper that reads team conversations and files them as tracked issues, reducing manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 56ddbb502ca50defbf7da98b1a4c3995bb155bd4db5eb9d09e35f32e9f7b0d9e -->
