# Open Issues — Plain-Language Overview

_Last updated 2026-06-29 21:47:31 UTC · 33 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Task]** **Custom date range picker** — When you choose "Custom" on the dashboard date filter, you'll get start and end date selectors so you can view data for any range you want, not just preset options like Today or This Month. (#58)
- **[Task]** **Restore missing dashboard sections** — Brings back the campaign stats, top offers, and watch list sections so the dashboard shows full reporting again instead of only the system overview, with the date range controlling what's displayed. (#240)
- **[Feature]** **New "Other Dashboard" views and activity log** — Adds views for "Offers with Legs" and CLP offer performance (flagging offers converting under 30%), plus a searchable record of every offer change so you can see who paused an offer or adjusted caps and when. (#256)
- **[Task]** **Consistent dashboard colors** — Applies a defined color palette across the dashboard so charts and sections are easier to read at a glance. (#263)
- **[Feature]** **Pick report dates without editing the web address** — Adds proper date controls to the dashboard so you can pull a specific day or range from the toolbar, while shareable links still update behind the scenes. (#268)
- **[Feature]** **Dashboard links open in a new tab** — Clicking a link from the dashboard opens it in a new browser tab so you don't lose your place. (#269)

## General / Across the App
- **[Feature]** **Light mode option** — Adds a toggle to switch the Admin between dark and light themes, with your choice remembered between visits. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, the app will warn that someone else is editing it and prevent one person from silently saving over another's changes. (#267)
- **[Bug]** **Invalid links now show an error** — Testing a broken link will return a clear failure message instead of quietly sending you back to the dashboard. (#239)
- **[Task]** **Users screen feature review** — A review comparing the Users area to the older system to identify missing capabilities (like bulk role changes and last-login info) so they can be prioritized. (#80)
- **[Task]** **Brand guidelines for AI output** — Establishing a clear brand guidelines document to use as the main reference for AI-generated content, improving the quality and consistency of results. (#264)

## Pre-Pings
- **[Feature]** **Enforce required fields before sending** — A "Before Data Push" pre-ping will now stop a lead with missing required information before it's sent out, rather than letting it through and relying on the partner to reject it. (#218)
- **[Bug]** **Close a gap in auto-register offers** — Fixes a case where an offer hidden by its pre-ping could still be auto-submitted and recorded as a success; the same checks will now apply so leads aren't sent when required information is missing. (#274)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifies each active advertiser's pre-ping behaves correctly so leads are matched and passed accurately. (#41)
- **[Task]** **Side-by-side pre-ping testing** — Runs the new pre-ping process alongside the existing one to confirm results match before fully switching over. (#40)

## Reports
- **[Feature]** **Up-to-the-hour "today" numbers** — Reports and the dashboard will show current-day impressions, clicks, leads, and revenue in real time, using the correct Eastern time zone. (#34)
- **[Task]** **Confirm report numbers match the old system** — An investigation comparing report figures between the new platform and the legacy system to find and explain any differences, so you can trust the numbers. (#271)

## Flows
- **[Feature]** **Clearer "Step order" setting** — The Flow form's step order field will get a plain-language label and helper text explaining what it controls, so it's no longer confusing. (#226)
- **[Task]** **Fix Flow form styling** — Cleans up visual issues on the Flow form, such as plainly styled text boxes, color pickers, and fields that should sit side by side, so it matches the look of other forms. (#152)

## Offers
- **[Task]** **Quick action links under each offer** — Adds familiar shortcuts (Edit, Quick Edit, Trash, View, Preview, Trends, Details) beneath each offer, with Trends opening an offer activity page showing lead and revenue trends over time. (#252)

## Placements
- **[Feature]** **Easier offer ordering on placements** — You'll be able to drag selected offers into the exact order you want, remove them with an "X" button, and filter the offer list by category. (#235)

## Campaigns
- **[Feature]** **Bring back the Campaigns module** — Adds the missing Campaigns area so you can create, edit, and manage campaigns and offer groups in the new platform, matching what the old admin offered. (#200)

## Behind the Scenes
- **[Task]** **Faster surveys** — Setting up a caching layer so survey placements and offers load more quickly. High priority. (#42)
- **[Task]** **Staging environment with recent data** — Creating a safe test environment loaded with May and June data so reports can be validated without touching live information. (#270)
- **[Feature]** **Automated Slack-to-issues helper** — A bot that turns action items from team conversations into tracked work items automatically. (#272)
- **[Feature]** **Daily and historical stats roll-up** — Behind-the-scenes work to combine daily activity into long-term totals for historical reporting. (#35)
- **[Task]** **Phasing in new automated background jobs** — Running the new scheduled processes alongside the existing ones, then gradually retiring the old ones in stages while monitoring closely. (#43, #44, #45, #46)
- **[Task]** **Reviewing an old stats job** — Checking whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Recovery and troubleshooting guides** — Documenting how to safely roll back changes and resolve common issues to keep the system reliable. (#48, #49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f4270bdd0b31f8e2616cac8fcf7e170b6cc49a2bf509514aac88ea987a3291d0 -->
