# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 03:05:07 UTC · 47 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a proper start- and end-date picker so you can view dashboard data for any range you like, instead of being limited to presets. (#58)
- **[Feature]** **Light mode option for the Admin** — You'll be able to switch between the current dark theme and a new light theme from your user menu, with your choice remembered next time you sign in. (#59)
- **[Feature]** **Working Edit, Preview, and Pull Leads buttons on detail pages** — Buttons on the Placement, Modal, Offer, and Advertiser detail pages that currently do nothing when clicked will take you where you expect. (#154)
- **[Feature]** **Sub-ID Stats moved to the Dashboard** — Sub-ID statistics will live in the Dashboard reporting area instead of being buried inside the placement form, making them easier to find. (#236)
- **[Bug]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will load again alongside the system overview, and the date-range selector will update them. (#240)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will show data in 15-minute increments, restoring the fine-grained view used to spot offer and partner-server issues quickly. (#243)
- **[Feature]** **Clearer offer status colors** — Paused will show red, Capped will show yellow/orange, and Active will stay green, so you can tell statuses apart at a glance across the offer list and dashboard. (#246)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds "Offer with Legs" and "CLP Performance" views (flagging offers converting under 30%) plus a searchable record of every change, like pausing an offer or editing a daily cap. (#256)
- **[Feature]** **Show full advertiser and placement names** — Names will no longer be cut off with an ellipsis in dashboard views, so you can read them in full. (#260)
- **[Feature]** **Remove the ID number column** — The ID/number column will be dropped from dashboard tables to free up screen space for the information that matters. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon (for example, "Foo: Bar: Acme Publishing" becomes "Acme Publishing"), making them easier to read. (#262)
- **[Feature]** **Standardized dashboard colors** — A defined color palette will be applied consistently across the dashboard to improve readability. (#263)

## Behind the Scenes
- **[Task]** **Review an old stats job** — Behind-the-scenes review of whether a legacy statistics process is still needed or can be retired. (#33)
- **[Task]** **Today's real-time stats** — Groundwork so the Dashboard's "today" view reflects up-to-the-hour impressions, clicks, leads, and revenue in Eastern Time. (#34)
- **[Task]** **Historical stats roll-up** — Behind-the-scenes work to summarize daily data so historical reports stay fast and accurate. (#35)
- **[Task]** **Side-by-side pre-ping testing** — The new pre-ping system will run alongside the old one and have its results compared before any switchover, to ensure accuracy. (#40)
- **[Task]** **Per-advertiser pre-ping checks** — Each active advertiser's pre-ping will be validated to confirm correct field mapping and pass/fail handling before going live. (#41)
- **[Task]** **Faster Survey Engine** — A behind-the-scenes caching layer will speed up surveys by keeping placement, offer, and cap information quickly available. (#42)
- **[Task]** **Run new scheduled jobs in parallel** — New scheduled processes will run alongside the existing ones in production and be monitored daily before any handover. (#43)
- **[Task]** **Switch over survey stats jobs** — Retiring the older hourly survey-stats process once its replacement proves stable. (#44)
- **[Task]** **Switch over secondary stats jobs** — Retiring a group of older statistics and caching processes after their replacements run cleanly for a week. (#45)
- **[Task]** **Switch over critical lead and cap jobs** — Carefully retiring the most important lead-processing and offer-cap-reset processes, with close monitoring and an immediate fallback if needed. (#46)
- **[Task]** **Document rollback steps** — Written, tested recovery procedures for each production system so the team can quickly undo a change if anything goes wrong. (#48)
- **[Task]** **Troubleshooting guides** — Step-by-step guides for handling common issues like lead-processing or offer-cap problems, helping the team resolve incidents faster. (#49)

## Offers
- **[Feature]** **Set all offer fields at creation** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting will be available when you first create an offer, so you no longer have to save and then re-edit to add them. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — A pending decision on blocking leads that are missing required pre-ping fields, so incomplete leads aren't passed through to advertisers. (#218)
- **[Bug]** **Advertiser info missing on the Offers report** — A data fix so every offer shows its advertiser in the Offers report, even after a recent attempt to correct this. (#242)
- **[Feature]** **Easier advertiser and state entry on offers** — Adds type-to-search to the Advertiser selector and lets you type or paste a comma-separated list of states (e.g., CA, TX, FL) for targeting. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in a group to the Conflicting Offers list in one step, saving significant time. (#250)
- **[Task]** **Quick action links on offer rows** — Restores legacy row actions (Edit, Quick Edit, Trash, View, Preview, Trends, Details) beneath each offer, with Trends opening a performance page showing leads, revenue, and daily breakdowns. (#252)
- **[Bug]** **HTML and Linkout issues in offer previews** — Fixes fields like "More Info" and TCPA content showing raw code instead of formatted text and links, and makes Linkout offers work correctly from the preview. (#259)

## Surveys
- **[Bug]** **Let visitors decline CPA offers** — Fixes a flow that traps visitors by forcing a "Yes" click; they'll be able to decline an offer or move past it instead of getting stuck. (#233)
- **[Feature]** **Skip the extra "Claim your offers" page** — New flows will take visitors straight to the form fields instead of showing an intro page first. (#228)
- **[Feature]** **Better TCPA consent checkbox** — The consent checkbox on the lander will be larger, rounded, and properly aligned with its text for a cleaner, clearer look. (#229)
- **[Feature]** **Footer copyright and site name** — The lander footer will include the copyright line and site name pulled from your General Information settings. (#232)

## Placements
- **[Bug]** **Tidy up the placement create/edit form** — Unfamiliar new fields will be reviewed (removed, relabeled, or explained) and missing links like Preview and Details will be restored to match what you're used to. (#234)
- **[Feature]** **Manually order assigned offers** — The offer assignment list will default to manual order with drag-and-drop reordering, an "X" to remove offers, and the ability to filter by taxonomy. (#235)
- **[Feature]** **Drag-and-drop offer assignment (UAT follow-up)** — The same improvement tracked from testing: manual-order default, drag-to-reorder, an "X" remove button, and taxonomy filtering on the offer transfer list. (#255)

## Flows
- **[Task]** **Fix the Flow form's appearance** — Resolves styling problems across the Flow form so textareas, color pickers, checkboxes, and paired side-by-side fields display correctly and consistently. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — You'll be able to add every available form field in one click instead of adding them one at a time. (#224)
- **[Feature]** **Clearer "Step order" setting** — The step-order control will get labels and help text so it's obvious what it does and what the values mean. (#226)

## General / Across the App
- **[Feature]** **Campaigns module** — Brings back the ability to create, edit, and manage campaigns and offer groups, matching the legacy system; this core feature is currently missing from the new platform. (#200)
- **[Task]** **Users management review** — A behind-the-scenes comparison of the old and new Users screens to identify missing capabilities (like bulk actions and last-login info) to guide upcoming work. (#80)
- **[Feature]** **Adopt brand guidelines for AI output** — A canonical brand-guidelines document will be established and used as the primary input to improve the quality of AI-generated content. (#264)

## Link Testing
- **[Feature]** **Pre-select the placement you came from** — Opening Link Testing from a placement will automatically choose that placement, so you don't have to pick it from the list each time. (#238)
- **[Bug]** **Show an error for invalid links** — Testing an invalid link will return a clear failure message instead of dumping you back on the dashboard. (#239)

## Properties
- **[Feature]** **Search the publisher list** — Adds type-to-search to the publisher selector on the property form so you can find a publisher without scrolling. (#237)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 687487fb5892cb0959b36f8b6c4eb3ec174c16bbb22d3dcbdd9d3df606803281 -->
