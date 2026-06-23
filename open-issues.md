# Open Issues — Plain-Language Overview

_Last updated 2026-06-23 18:40:34 UTC · 49 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Set piggyback offers, HD pixel placements, and ZIP targeting when creating an offer** — Right now you have to create an offer first and then edit it to add these. This change lets you set everything during initial creation. High priority. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending a lead** — When a pre-ping runs before pushing data, leads missing required information will be stopped up front instead of being sent on and judged solely by the partner. A decision is needed before this is finalized. (#218)
- **[Bug]** **Advertiser info missing on the Offers report** — Some offers still don't show their advertiser even after a data fix. This resolves the remaining gap so every offer displays its advertiser. (#242)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will show activity in 15-minute increments again, making it easier to spot and react to problems with offers or partner servers. (#243)
- **[Bug]** **Status filter on the Offers report** — You'll be able to narrow the Offers report to just Active, Paused, or Capped offers instead of seeing everything at once. (#244)
- **[Feature]** **Distinct status colors for offers** — Paused will be red, Capped yellow/orange, and Active green, so you can tell them apart at a glance in lists and dashboard indicators. (#246)
- **[Bug]** **Offer images not displaying in the offer form** — Images attached to offers currently don't appear. This fixes the rendering (or missing-image data) so they show correctly. (#247)
- **[Feature]** **Easier advertiser and state targeting on the offer form** — Adds type-to-search to the Advertiser picker and lets you type or paste a comma-separated list of states (e.g. CA, TX, FL) for targeting. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers at once** — On the Delivery & Settings tab, you'll be able to add every offer in a group to the Conflicting Offers list in one step, saving significant time. (#250)
- **[Task]** **Quick action links under each offer** — Adds the familiar row actions (Edit, Quick Edit, Trash, View, Preview, Trends, Details) beneath offer titles, with Trends opening an offer activity and performance page. (#252)
- **[Bug]** **Formatted content and link-out offers in Offer Preview** — Headline, More Info, and TCPA fields will display their links and styling properly instead of raw code, and link-out offers will work correctly from the preview. (#259)

## Dashboard

- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open a date range picker with start and end dates so you can view dashboard data for any period you like. (#58)
- **[Feature]** **Light/Dark mode toggle** — You'll be able to switch between dark and light themes from the Admin UI, with your choice remembered across sessions. (#59)
- **[Feature]** **Working Edit, Preview, and Pull Leads buttons on detail pages** — These buttons currently do nothing on several detail screens. They'll be wired up so clicking them takes the expected action. (#154)
- **[Feature]** **Move Sub-ID Stats into the Dashboard** — Sub-ID statistics will be relocated from the placement form into the Dashboard reporting area where they belong. (#236)
- **[Bug]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will load again alongside the system overview, and the date range selector will update them. High priority. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds "Offer with Legs" and CLP performance views (flagging offers converting under 30%) plus a searchable record of changes like pausing offers or adjusting daily caps. (#256)
- **[Feature]** **Show full advertiser and placement names** — Long advertiser and placement names will no longer be cut off in dashboard views, so you can read them in full. (#260)
- **[Feature]** **Remove the ID/number column** — Dropping this column from dashboard tables frees up screen space for the information that matters. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the text after the last colon (e.g. "Foo: Bar: Acme Publishing" shows as "Acme Publishing") for easier reading. (#262)
- **[Feature]** **Standardized dashboard color scheme** — A defined color palette will be applied consistently across the dashboard to improve readability. (#263)

## Flows

- **[Task]** **Fix Flow form styling** — Several parts of the Flow form (textareas, color pickers, checkboxes, paired fields) currently look unstyled or stack awkwardly. This brings the form's appearance in line with the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field in a single click. (#224)
- **[Feature]** **Clearer "Step order" setting** — Adds labels and help text so it's obvious what the step-order control does and what its values mean. (#226)
- **[Feature]** **Skip the "Claim your offers" intro page** — New flows will take visitors straight to the form fields instead of showing an extra starting page. (#228)
- **[Feature]** **Better TCPA consent checkbox styling** — The consent checkbox on the lander will be larger, rounded, and properly aligned with its text. (#229)
- **[Feature]** **Footer with copyright and site name** — The lander footer will include the copyright line and site name pulled from your General Information. (#232)
- **[Bug]** **Visitors stuck on CPA offers** — On CPA offer flows, visitors are currently forced to click "Yes" with no way to decline or move on. This fixes the flow so they can decline, continue, or exit. High priority. (#233)

## General / Across the App

- **[Task]** **Users module review** — A review comparing the legacy Users area to the new one, identifying missing pieces (like bulk role changes and last-login info) to guide upcoming improvements. (#80)
- **[Feature]** **Bring back the Campaigns module** — Campaign management isn't yet available in New Adsmith Frontend. This adds the ability to view, create, edit, and configure campaigns and offer groups, matching the legacy system. Critical, high priority. (#200)
- **[Feature]** **Link Testing remembers the placement you opened it from** — When you start Link Testing from a specific placement, that placement will be pre-selected for you. (#238)
- **[Bug]** **Clear error for invalid links in Link Testing** — Testing an invalid link will show a proper failure message instead of dropping you back on the dashboard. (#239)
- **[Feature]** **Brand guidelines as the primary AI input** — Establishes a comprehensive brand-guidelines document to be used as the main reference for AI-generated output quality. (#264)

## Placements

- **[Bug]** **Tidy up the placement create/edit form** — Unfamiliar new fields will be reviewed (removed, relabeled, or documented) and missing links like Preview and Details will be restored. (#234)
- **[Feature]** **Reorder and filter assigned offers** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove each one, and the ability to filter the offer list by taxonomy. (#235)
- **[Feature]** **Manual reordering on the offer transfer list** — A related UAT request to make offer assignment default to manual order with drag-and-drop and a remove button, so your chosen order is kept. (#255)

## Properties

- **[Feature]** **Search the publisher selector** — Adds type-to-search to the publisher dropdown on the property form so you don't have to scroll to find one. (#237)

## Behind the Scenes

- **[Task]** **Review of an older stats job** — Checking whether a legacy stats process is still needed or can be retired. (#33)
- **[Feature]** **Real-time "today" stats** — Behind-the-scenes work so today's impressions, clicks, leads, and revenue show up promptly in the dashboard. (#34)
- **[Feature]** **Faster historical stats** — Groundwork to roll up activity into daily totals for quicker historical reporting. (#35)
- **[Task]** **Side-by-side pre-ping testing** — Running the new and old pre-ping systems together to confirm the new one matches before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each advertiser's pre-ping works correctly ahead of the switchover. (#41)
- **[Task]** **Speed improvements for surveys** — Adding a caching layer so survey landers load and respond faster. High priority. (#42)
- **[Task]** **Parallel run of scheduled jobs** — Running the new scheduled jobs alongside the existing ones to confirm they match before relying on them. (#43)
- **[Task]** **Scheduled-job switchover, group 3** — Retiring the first batch of older scheduled jobs once their replacements are proven stable. (#44)
- **[Task]** **Scheduled-job switchover, group 2** — Retiring the next batch of scheduled jobs after the first group is confirmed stable. (#45)
- **[Task]** **Scheduled-job switchover, group 1 (critical)** — Retiring the most critical scheduled jobs last, with close monitoring and quick rollback ready. (#46)
- **[Task]** **Documented rollback steps** — Writing clear recovery procedures for each system in case anything needs to be reverted. (#48)
- **[Task]** **Troubleshooting guides** — Creating step-by-step guides for resolving common operational issues quickly. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 2193e483427bbca7ef4a993b1881469ca39305841dcaa1ee15d37bf610c688fa -->
