# Open Issues — Plain-Language Overview

_Last updated 2026-06-23 00:48:26 UTC · 50 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Bug]** **Custom date range on the Dashboard** — Choosing "Custom" in the date filter will open a proper start/end date picker so you can view results for any range you like, not just the preset options. (#58)
- **[Bug]** **Missing dashboard sections restored** — High priority. Campaign stats, top offers, and watch lists will load again alongside the system overview, and they'll update when you change the date range. (#240)
- **[Feature]** **Light mode option** — You'll be able to switch the Admin between the current dark look and a new light theme, with your choice remembered next time you log in. (#59)
- **[Feature]** **Working Edit, Preview, and Pull Leads buttons** — On Placement, Modal, Offer, and Advertiser detail pages, these buttons currently do nothing; they'll be wired up so they take you where you expect. (#154)
- **[Feature]** **Sub-ID stats moved to the Dashboard** — The Sub-ID Stats view will live in the Dashboard reporting area instead of inside the placement form, where it's easier to find. (#236)
- **[Feature]** **New monitoring views and an activity log** — An "Other Dashboard" area will add "Offer with Legs" and CLP performance views (flagging offers converting under 30%), plus a searchable log of changes like pausing offers or editing caps. (#256)
- **[Feature]** **Full advertiser and placement names** — Long names will no longer be cut off with "…", so you can read them in full on dashboard views. (#260)
- **[Feature]** **Cleaner tables without the ID column** — The ID/number column will be removed from dashboard tables to free up screen space. (#261)
- **[Feature]** **Tidier publisher and property names** — Names will display only the part after the last colon (e.g. "Foo: Bar: Acme Publishing" shows as "Acme Publishing") for easier reading. (#262)
- **[Feature]** **Consistent dashboard colors** — A defined color palette will be applied across the dashboard to improve readability. (#263)

## Offers
- **[Bug]** **Offer images not showing** — Images on the offer form aren't appearing; this will be investigated and fixed so offer creatives display properly. (#247)
- **[Bug]** **Formatted text and link-out in offer preview** — Fields like More Info and TCPA content currently show raw code instead of styled text and links, and link-out offers don't work from the preview. Both will be corrected. (#259)
- **[Bug]** **Advertiser names in the Offers report** — Some offers still show no advertiser; this data issue will be resolved so every offer lists its advertiser. (#242)
- **[Feature]** **Set more fields when creating an offer** — High priority. Piggyback offers, HD pixel placements, and ZIP code targeting will be available right when you create an offer, instead of having to save first and then edit. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — When a pre-ping runs before pushing data, leads missing required fields will be stopped up front rather than relying on the advertiser's response. (Confirmation needed before this change.) (#218)
- **[Feature]** **15-minute detail on offer stats** — The offer detail timespan chart will show 15-minute increments again, helping you spot offer or partner issues quickly. (#243)
- **[Feature]** **Clearer offer status colors** — Paused will be red, Active green, and Capped yellow/orange so the three are easy to tell apart at a glance. (#246)
- **[Feature]** **Faster advertiser and state entry on offers** — The Advertiser selector gets a type-to-search box, and state targeting will accept a typed or pasted comma-separated list like "CA, TX, FL". (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab you'll be able to add every offer in a group to the conflicting list in one step, saving lots of manual work. (#250)
- **[Task]** **Quick action links under each offer** — Legacy-style links (Edit, Quick Edit, Trash, View, Preview, Trends, Details) will appear beneath each offer, with Trends opening an offer activity/performance page. (#252)

## Flows
- **[Bug]** **Turn header and footer on or off** — The flow form will get controls to enable or disable the header, footer, and other sections, which is currently not possible. (#225)
- **[Task]** **Flow form styling fixes** — The Flow form has unstyled text boxes, color pickers, and stacked fields; this cleanup brings its look in line with the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button** — Instead of adding form fields one at a time, you'll be able to add every available field at once. (#224)
- **[Feature]** **Clearer step-order setting** — The step-order control will get plain-language labels and help text so it's obvious what it does. (#226)

## Surveys
- **[Bug]** **Visitors stuck on CPA offers** — High priority. Right now a visitor must click "Yes" to continue with no way to decline or move on; this will be fixed so they can proceed or exit. (#233)
- **[Feature]** **Skip the extra "Claim your offers" page** — Visitors will land directly on the form fields instead of seeing an intro page first. (#228)
- **[Feature]** **Better TCPA consent checkbox** — The consent checkbox will be larger, rounded, and properly aligned with its text. (#229)
- **[Feature]** **Footer copyright and site name** — The landing page footer will show the copyright line and site name pulled from your General Information. (#232)

## Placements
- **[Bug]** **Familiar placement form and missing links** — The create/edit form will be reviewed against the legacy version to clear up unrecognized fields and restore missing links like Preview and Details. (#234)
- **[Feature]** **Reorder assigned offers easily** — Offer assignment will default to Manual Order with drag-and-drop reordering, an "X" to remove offers, and the ability to filter by taxonomy. (#235)
- **[Feature]** **Drag-and-drop offer assignment (from UAT)** — The same offer transfer improvements raised in testing: manual ordering, drag-and-drop, an "X" to remove, and taxonomy filtering. (#255)

## General / Across the App
- **[Feature]** **Campaigns module** — Critical, high priority. The Campaigns area from the legacy system will be added so you can create, edit, and manage campaigns and offer groups in New Adsmith Frontend. (#200)
- **[Task]** **Users management review** — A review comparing the legacy and new Users screens to plan which missing options (bulk actions, last login, and more) to bring over. (#80)
- **[Feature]** **Brand guidelines as a standard** — A comprehensive brand-guidelines document will be created and used to drive more consistent, on-brand output. (#264)

## Link Testing
- **[Bug]** **Clear error for invalid links** — Testing an invalid link will show a proper failure message instead of bouncing you to the dashboard. (#239)
- **[Feature]** **Remember the placement you started from** — Opening Link Testing from a placement will pre-select that placement so you don't have to pick it each time. (#238)

## Properties
- **[Feature]** **Search the publisher list** — The publisher selector on the property form gets a type-to-search box so you don't have to scroll to find one. (#237)

## Behind the Scenes
- **[Bug]** **Data sync and stats accuracy** — Critical blocker. The process that copies production data to the test environment is overwriting records and leaving some stats and offer details blank; this work fixes data accuracy so yesterday's stats and offer information show correctly. (#241)
- **[Task]** **Today's live stats** — Behind-the-scenes work to power up-to-the-day impression, click, lead, and revenue figures for the dashboard. (#34)
- **[Task]** **Rolling up historical stats** — Maintenance to summarize live stats into daily totals for reliable historical reporting. (#35)
- **[Task]** **Review of an old stats job** — Checking whether a legacy subid-a stats process is still needed or can be retired. (#33)
- **[Task]** **Pre-ping accuracy testing** — Running the new pre-ping process alongside the old one to confirm results match before switching over. (#40)
- **[Task]** **Per-advertiser pre-ping checks** — Verifying each active advertiser's pre-ping works correctly ahead of the switch. (#41)
- **[Task]** **Faster survey performance** — High priority. Adding a caching layer so surveys, offers, and caps load and check more quickly. (#42)
- **[Task]** **Parallel run of scheduled jobs** — Running new and old background jobs side by side in production to compare results. (#43)
- **[Task]** **Retiring background jobs, group 3** — Switching off the lowest-risk legacy survey-stats job after the replacement proves stable. (#44)
- **[Task]** **Retiring background jobs, group 2** — Switching off additional legacy stats jobs once the prior group is stable. (#45)
- **[Task]** **Retiring background jobs, group 1** — Critical. Switching off the most important legacy lead-processing and cap-reset jobs last, with close monitoring. (#46)
- **[Task]** **Rollback procedures** — Documenting how to safely revert each production system if something goes wrong. (#48)
- **[Task]** **Troubleshooting runbooks** — Creating step-by-step guides for handling common issues like lead-processing or stats failures. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 56a32f4c7fb7a8cf5da851848990923ce422a0050b61e7812ca5d1ca22f7aaa6 -->
