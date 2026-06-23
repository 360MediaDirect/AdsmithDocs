# Open Issues — Plain-Language Overview

_Last updated 2026-06-23 01:40:22 UTC · 50 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open a proper start- and end-date picker so you can view dashboard data for any period you like, not just the preset ranges. (#58)
- **[Feature]** **Light mode option** — You'll be able to switch the Admin between the current dark look and a new light theme, with your choice remembered for next time. (#59)
- **[Feature]** **Make Edit, Preview, and Pull Leads buttons work** — On Placement, Modal, Offer, and Advertiser detail pages these buttons currently do nothing; once fixed they'll take you straight to the right place. (#154)
- **[Feature]** **Sub-ID stats move to the Dashboard** — Sub-ID statistics will live in the Dashboard reporting area instead of being buried in the placement form, making them easier to find. (#236)
- **[Bug]** **Bring back missing Dashboard sections** — Campaign stats, top offers, and watch lists will load again and respond to your date-range selection, rather than only showing the system overview. (#240)
- **[Feature]** **New monitoring views and an activity log** — Adds "Offer with Legs" and CLP performance views (flagging offers converting under 30%) plus a searchable record of changes like pausing offers or adjusting caps. (#256)
- **[Feature]** **Show full advertiser and placement names** — Long names will no longer be cut off with "…", so you can read them in full. (#260)
- **[Feature]** **Remove the ID column** — Dropping the ID/number column frees up screen space for the information you actually use. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon (e.g. "Acme Publishing" instead of "Foo: Bar: Acme Publishing"). (#262)
- **[Feature]** **Standardized dashboard colors** — A defined color palette will be applied consistently across the Dashboard for better readability. (#263)

## Offers
- **[Feature]** **Set more fields when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP-code targeting will be available right when you create an offer, instead of having to save first and then edit. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — Leads missing required fields will be stopped up front rather than being sent out and relying on the advertiser to reject them. (Decision needed before building.) (#218)
- **[Feature]** **Clearer status colors** — Paused will be red, Active green, and Capped yellow/orange so the three states are easy to tell apart in offer lists and dashboard indicators. (#246)
- **[Bug]** **Offer images not showing** — Images that currently fail to appear in the offer form will display correctly. (#247)
- **[Feature]** **Easier offer form entry** — Adds a type-to-search box to the Advertiser selector and lets you paste a comma-separated list of states for targeting. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab you'll be able to add every offer in a group to the conflicting list in one step, saving a lot of manual work. (#250)
- **[Task]** **Quick action links under each offer** — Restores handy links like Edit, Quick Edit, View, Preview, Trends, and Details beneath offer titles, with Trends opening an offer performance page. (#252)
- **[Bug]** **Fix HTML and linkout in offer previews** — More Info and TCPA fields will show formatted links and styling instead of raw code, and linkout offers will work from the preview. (#259)

## Flows & Surveys
- **[Task]** **Fix the look of the Flow form** — Textareas, color pickers, checkboxes, and paired fields will be styled properly and laid out side-by-side instead of appearing plain or stacked. (#152)
- **[Feature]** **"Add all fields" button** — Add every available form field to a flow in a single click instead of one at a time. (#224)
- **[Feature]** **Explain the "Step order" setting** — Adds labels and help text so it's clear what this control orders and what the values mean. (#226)
- **[Feature]** **Skip the extra "Claim your offers" page** — Visitors will land directly on the form fields instead of having to click through an intro screen first. (#228)
- **[Feature]** **Nicer TCPA consent checkbox** — The consent checkbox will be larger, rounded, and properly aligned with its text on the live lander. (#229)
- **[Feature]** **Footer copyright and site name** — The lander footer will show the copyright line and site name pulled from General Information. (#232)
- **[Bug]** **Don't trap visitors on CPA offers** — Visitors will be able to decline or move past a CPA offer instead of being forced to click "Yes" to continue. (#233)

## Reports
- **[Bug]** **Show advertiser info on the Offers report** — Every offer will display its advertiser, fixing the gap that remained after the earlier data update. (#242)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail chart will return to 15-minute increments so you can spot errors and partner-server issues quickly. (#243)
- **[Bug]** **Status filter on the Offers report** — You'll be able to narrow the report to Active, Paused, or Capped offers instead of seeing everything at once. (#244)

## Placements
- **[Bug]** **Tidy up the placement form** — Unfamiliar new fields will be reviewed (removed, relabeled, or explained) and missing links like Preview and Details will be restored. (#234)
- **[Feature]** **Reorder assigned offers easily** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove, and the ability to filter the list by taxonomy. (#235)
- **[Feature]** **Drag-and-drop offer assignment (UAT follow-up)** — Same improvement tracked from formal testing: manual ordering, drag-and-drop, remove button, and taxonomy filtering on the placement offer transfer list. (#255)

## Link Testing
- **[Feature]** **Pre-select the placement you came from** — Opening Link Testing from a placement will automatically choose that placement instead of making you pick. (#238)
- **[Bug]** **Show an error for invalid links** — Testing a bad link will return a clear failure message rather than bouncing you to the dashboard. (#239)

## General / Across the App
- **[Feature]** **Bring back the Campaigns module** — A high-priority addition so you can view, create, edit, and configure campaigns and their offer groups, matching what's available in the current system. (#200)
- **[Task]** **Users area review** — A behind-the-scenes comparison of the Users screens against the previous system to plan which missing features (such as bulk actions and extra columns) to add next. (#80)

## Properties
- **[Feature]** **Search box for the publisher selector** — Type to find a publisher on the property form instead of scrolling through the whole list. (#237)

## Behind the Scenes
- **[Bug]** **Fix data sync that wipes out stats** — Resolves the data-transfer problem behind empty "yesterday" stats, mismatched property counts, and blank offer data, so the numbers you see are accurate. (#241)
- **[Task]** **Faster "today" stats** — Work to power up-to-the-moment figures for the Dashboard's "today" view. (#34)
- **[Task]** **Reliable historical stats** — Behind-the-scenes work to roll up data into accurate day-by-day totals for reporting. (#35)
- **[Task]** **Speed up survey performance** — Adds a caching layer so offers and placements load faster for visitors. (#42)
- **[Task]** **Pre-ping safety testing** — Running the new pre-ping process alongside the existing one to confirm it behaves identically before switching over. (#40)
- **[Task]** **Per-advertiser pre-ping checks** — Verifying pre-ping works correctly for each active advertiser before the switch. (#41)
- **[Task]** **Review an old stats job** — Checking whether a legacy scheduled task is still needed or can be retired. (#33)
- **[Task]** **Roll out new scheduled jobs safely** — Running new and old scheduled tasks side-by-side in production and watching for differences. (#43)
- **[Task]** **Retire old scheduled tasks (low risk)** — Carefully switching off the least critical legacy jobs once replacements prove stable. (#44)
- **[Task]** **Retire old scheduled tasks (medium risk)** — Switching off the next set of legacy stats jobs after monitoring. (#45)
- **[Task]** **Retire old scheduled tasks (most critical)** — Switching off the most important legacy jobs last, with close monitoring and instant rollback ready. (#46)
- **[Task]** **Document how to roll back** — Writing clear recovery steps for each system in case something needs to be reversed. (#48)
- **[Task]** **Troubleshooting guides** — Creating reference guides for handling common issues like lead-processing or stats problems. (#49)
- **[Feature]** **Stronger brand guidelines for AI output** — Establishing a comprehensive brand guide as the main reference to improve the quality of AI-generated results. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: e5b525ea5deaae522eb5c0b96bdc06719dcba9b7faa6fb95d679ecf984c97411 -->
