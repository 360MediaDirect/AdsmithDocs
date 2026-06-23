# Open Issues — Plain-Language Overview

_Last updated 2026-06-23 09:06:25 UTC · 50 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a start/end date picker so you can view dashboard data for any range you want, not just the preset options. (#58)
- **[Feature]** **Make detail-page buttons work** — The Edit, Preview, and Pull Leads buttons on Placement, Modal, Offer, and Advertiser detail pages will actually do something when clicked instead of sitting there unresponsive. (#154)
- **[Feature]** **Sub-ID Stats moved to the Dashboard** — Sub-ID statistics will live in the Dashboard reporting area instead of being buried inside the placement form, making them easier to find. (#236)
- **[Bug]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will load again, and the date-range selector will update them. Right now only the system overview appears. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds views for long-running ("offers with legs") and underperforming CLP offers, plus a searchable record of changes like pausing offers or cap edits, with timestamps. (#256)
- **[Feature]** **Show full advertiser and placement names** — Long advertiser and placement names will no longer be cut off with "…", so you can read them in full. (#260)
- **[Feature]** **Remove the ID column** — The ID/number column will be dropped from dashboard tables to free up screen space for the information that matters. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon (e.g. "Foo: Bar: Acme Publishing" shows as "Acme Publishing") for easier reading. (#262)
- **[Feature]** **Standardized dashboard colors** — A defined color palette will be applied consistently across the dashboard to improve readability. (#263)

## Offers
- **[Feature]** **Set all offer fields when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting will be available during initial creation, so you no longer have to save first and then edit to add them. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — When a pre-ping runs before pushing data, leads missing required fields will be stopped up front rather than relying on the advertiser's endpoint to catch them. (Needs a decision before building.) (#218)
- **[Feature]** **Distinct offer status colors** — Paused will be red, Capped yellow/orange, and Active green, so you can tell them apart at a glance in offer lists and dashboard indicators. (#246)
- **[Bug]** **Offer images not showing** — Images on the offer form will render correctly instead of appearing blank. (#247)
- **[Feature]** **Faster offer form entry** — Adds a type-to-search box on the Advertiser selector and lets you type or paste a comma-separated list of states for targeting. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab you'll be able to add every offer in an offer group to the conflicting list in one step, saving a lot of manual work. (#250)
- **[Task]** **Quick action links on offer rows** — Brings back per-offer actions like Edit, Quick Edit, View, Preview, Trends, and Details beneath each offer title, with Trends opening an offer activity/performance view. (#252)
- **[Bug]** **HTML and linkout fixes in offer tabs** — Headline, More Info, and TCPA fields will display formatted text and working links instead of raw code, and linkout offers will work from the preview. (#259)

## Flows
- **[Task]** **Fix Flow form styling** — Textareas, color pickers, checkboxes, and paired fields will display properly and sit side-by-side as in the Placement and Modal forms, instead of looking unstyled or stacked. (#152)
- **[Feature]** **"Add all fields" button** — When building a flow you'll be able to add every available form field at once instead of adding them one at a time. (#224)
- **[Feature]** **Clearer step-order control** — The step-order setting will get labels and help text so it's obvious what it controls and what the values mean. (#226)
- **[Feature]** **Start flows on the form** — The extra "Claim your offers" intro page will be removed so visitors land directly on the form fields. (#228)
- **[Feature]** **Better TCPA checkbox styling** — The consent checkbox will be larger, rounded, and properly aligned with the consent text on the rendered lander. (#229)
- **[Feature]** **Footer copyright and site name** — The lander footer will show the copyright line and the site name pulled from General Information. (#232)
- **[Bug]** **Let visitors move past CPA offers** — Visitors will be able to decline or proceed past a CPA offer instead of being forced to click "Yes," which currently traps them mid-flow. (#233)

## Placements & Properties
- **[Bug]** **Clean up the placement create/edit form** — Unfamiliar new fields will be reviewed and relabeled or removed, and missing links like Preview and Details will be restored. (#234)
- **[Feature]** **Better offer assignment on placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove, and the ability to filter the offer list by taxonomy. (#235)
- **[Feature]** **Drag-and-drop offer ordering (UAT follow-up)** — Same improvement tracked from testing: manual ordering, drag-and-drop, remove buttons, and taxonomy filtering on the placement offer transfer list. (#255)
- **[Feature]** **Search box for the publisher selector** — On the property form you'll be able to type to find a publisher instead of scrolling the whole list. (#237)

## Reports
- **[Bug]** **Show advertiser info on the Offers report** — Advertiser details will appear for all offers; some are still missing after an earlier data fix. (#242)
- **[Bug]** **Status filter on the Offers report** — You'll be able to narrow the Offers report to Active, Paused, or Capped offers instead of seeing everything at once. (#244)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will show 15-minute increments again, helping you spot offer or partner-server issues quickly. (#243)

## General / Across the App
- **[Feature]** **Dark/Light mode toggle** — You'll be able to switch the Admin between dark and light themes, with your choice remembered between sessions. (#59)
- **[Feature]** **Bring back the Campaigns module** — Restores the ability to view, create, edit, and configure campaigns and offer groups, matching the legacy admin. This is currently missing entirely. (#200)
- **[Task]** **Users management review** — A documentation review comparing the old and new Users screens to identify missing pieces (like bulk actions and extra columns) and plan what to add next. (#80)

## Link Testing
- **[Feature]** **Default to the current placement** — When you open Link Testing from a placement, that placement will already be selected so you don't have to pick it each time. (#238)
- **[Bug]** **Clear error for invalid links** — Testing an invalid link will show a proper failure message instead of bouncing you back to the dashboard. (#239)

## Behind the Scenes
- **[Task]** **Real-time "today" stats** — Behind-the-scenes work so the dashboard's "today" figures (impressions, clicks, leads, revenue) update from live data with correct Eastern Time handling. (#34)
- **[Task]** **Historical stats roll-up** — Maintenance to summarize live stats into daily totals so historical reports stay accurate and fast. (#35)
- **[Task]** **Review an old stats job** — Checking whether a legacy sub-ID stats process is still needed or can be retired. (#33)
- **[Task]** **Pre-ping safety testing** — Running the new pre-ping system alongside the old one to confirm results match before switching over. (#40)
- **[Task]** **Per-advertiser pre-ping checks** — Verifying each active advertiser's pre-ping works correctly before the switchover. (#41)
- **[Task]** **Faster survey performance** — Adding a caching layer so surveys load and check offer caps more quickly. High priority. (#42)
- **[Task]** **Deploy updated scheduled jobs** — Rolling out new background jobs to run in parallel with the old ones while we monitor for differences. (#43)
- **[Task]** **Retire old scheduled jobs (low risk)** — Turning off the lowest-risk legacy survey-stats job once its replacement proves stable. (#44)
- **[Task]** **Retire old scheduled jobs (medium risk)** — Turning off additional legacy stats jobs after the first batch is confirmed stable. (#45)
- **[Task]** **Retire old scheduled jobs (critical, last)** — Turning off the most critical legacy jobs, including lead processing and offer-cap resets, with close monitoring and quick rollback ready. (#46)
- **[Task]** **Rollback procedures** — Documenting and testing how to safely revert each system if something goes wrong. (#48)
- **[Task]** **Troubleshooting runbooks** — Step-by-step guides for resolving common issues like lead processing or stats problems. (#49)
- **[Feature]** **Brand guidelines for AI output** — Establishing a single comprehensive brand-guidelines document to guide and improve AI-generated content. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: e5b525ea5deaae522eb5c0b96bdc06719dcba9b7faa6fb95d679ecf984c97411 -->
