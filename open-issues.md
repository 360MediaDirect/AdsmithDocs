# Open Issues — Plain-Language Overview

_Last updated 2026-06-23 05:20:53 UTC · 50 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Bug]** **Custom date range on the Dashboard** — Picking "Custom" in the date filter will open a real start/end date picker, so you can view dashboard data for any range you choose instead of only the preset options. (#58)
- **[Feature]** **Light mode option** — You'll be able to switch the Admin between the current dark theme and a new light theme, and your choice will stick between visits. (#59)
- **[Feature]** **Working Edit, Preview, and Pull Leads buttons** — On Placement, Modal, Offer, and Advertiser detail pages these buttons currently do nothing; they'll be wired up so they take you where you expect. (#154)
- **[Feature]** **Sub-ID Stats move to the Dashboard** — Sub-ID performance stats will live in the Dashboard reporting area instead of being buried inside the placement form. (#236)
- **[Bug]** **Missing dashboard sections restored** — Campaign stats, top offers, and watch lists will load again alongside the system overview, and the date-range selector will update them. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds views to spot durable offers and low-converting CLP offers, plus a searchable record of changes like pausing offers or editing caps. (#256)
- **[Feature]** **Full advertiser and placement names** — Long names will no longer be cut off with "…", so you can read them in full. (#260)
- **[Feature]** **Remove the ID column** — The ID/number column will be dropped from dashboard tables to free up screen space for the information you actually use. (#261)
- **[Feature]** **Cleaner publisher and property names** — Display names will show only the part after the last colon (e.g. "Acme Publishing"), making lists easier to scan. (#262)
- **[Feature]** **Standardized dashboard colors** — A defined color palette will be applied consistently across dashboard views for better readability. (#263)

## Offers
- **[Feature]** **Set more fields when creating an offer** — Piggyback offers, HD pixel placements, and ZIP-code targeting will be available right when you create an offer, instead of having to save first and then edit. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — When a pre-ping runs before pushing a lead, missing required fields will stop the lead immediately rather than relying on the partner's response. (Decision needed before building.) (#218)
- **[Feature]** **Distinct status colors** — Paused will be red, Capped yellow/orange, and Active green, so the three are easy to tell apart at a glance. (#246)
- **[Bug]** **Offer images not showing** — Offer images that currently fail to appear in the offer form will display correctly. (#247)
- **[Feature]** **Easier advertiser and state entry on the offer form** — Adds type-to-search for the Advertiser field and lets you paste a comma-separated list of states for targeting. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — You'll be able to add every offer in a group to the Conflicting Offers list in one step, saving repetitive clicks. (#250)
- **[Task]** **Quick action links under each offer** — Brings back legacy row actions (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an offer performance page. (#252)
- **[Bug]** **Formatted content and linkouts in offer preview** — Headline, More Info, and TCPA fields will show proper links and styling instead of raw code, and linkout offers will work from the preview. (#259)

## Flows
- **[Task]** **Fix Flow form styling** — Textareas, color pickers, checkboxes, and paired fields will be properly styled and laid out side-by-side, matching the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Add every available form field at once instead of one at a time. (#224)
- **[Feature]** **Clearer step-order setting** — The step-order control will get labels and help text so it's obvious what it controls and what the values mean. (#226)
- **[Feature]** **Skip the extra "Claim your offers" page** — Visitors will land directly on the form fields instead of an intro page. (#228)
- **[Feature]** **Better TCPA checkbox styling** — The consent checkbox will be larger, rounded, and properly aligned with its text. (#229)
- **[Feature]** **Footer copyright and site name** — The lander footer will show the copyright line and site name pulled from General Information. (#232)

## Placements
- **[Bug]** **Tidy up the placement form** — Unfamiliar fields will be reviewed (removed, relabeled, or explained) and missing links like Preview and Details will be restored. (#234)
- **[Feature]** **Reorder assigned offers by drag-and-drop** — Selected offers will default to Manual Order, support drag-and-drop reordering, get an "X" to remove, and allow filtering by taxonomy. (#235)
- **[Feature]** **Manual ordering for the offer transfer list** — Confirms the same improvement from testing: manual order by default, drag-and-drop, remove buttons, and taxonomy filtering when assigning offers. (#255)

## Reports
- **[Bug]** **Advertiser info on the Offers report** — Offers that still show no advertiser will be corrected so advertiser details appear for every offer. (#242)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail chart will return to 15-minute increments, making it easier to catch issues with offers or partner servers quickly. (#243)
- **[Feature]** **Status filter on the Offers report** — You'll be able to narrow the report to Active, Paused, or Capped offers instead of seeing everything at once. (#244)

## General / Across the App
- **[Task]** **Users area review** — A comparison of the new Users screens against the legacy version to plan which missing pieces (bulk actions, last-login, and more) to bring over. (#80)
- **[Feature]** **Campaigns module** — Adds the missing Campaigns area so you can create, edit, and manage campaigns and offer groups, matching the legacy system. (#200)
- **[Feature]** **Brand guidelines for AI output** — A comprehensive brand-guidelines document will be created and used to improve the quality of AI-generated content. (#264)

## Link Testing
- **[Feature]** **Default to the placement you opened it from** — When you start Link Testing from a placement, that placement will already be selected so you don't have to pick it. (#238)
- **[Bug]** **Clear error for invalid links** — Testing a bad link will show a proper failure message instead of bouncing you back to the dashboard. (#239)

## Properties
- **[Feature]** **Searchable publisher selector** — Type to find a publisher on the property form instead of scrolling through the full list. (#237)

## Surveys
- **[Bug]** **Let visitors move past CPA offers** — Right now visitors are forced to click "Yes" with no way to decline or continue; they'll be able to decline an offer and proceed through the flow. (#233)

## Behind the Scenes
- **[Bug]** **Missing stats and data mismatches** — Investigating why some stats (like yesterday's totals) and offer data come through empty, and reconciling property counts so the numbers you see are accurate. (#241)
- **[Task]** **"Today" stats** — Behind-the-scenes work so dashboards can show up-to-the-day numbers. (#34)
- **[Task]** **Historical stats roll-up** — Maintenance so daily and historical reporting totals stay accurate over time. (#35)
- **[Task]** **Review of an old stats job** — Checking whether a legacy scheduled stats job is still needed. (#33)
- **[Task]** **Faster surveys** — Performance improvements so survey landers and offer data load more quickly. (#42, high priority)
- **[Task]** **Pre-ping safety testing** — Running the new pre-ping process alongside the old one to confirm results match before switching over. (#40)
- **[Task]** **Per-advertiser pre-ping checks** — Verifying each advertiser's pre-ping works correctly ahead of the switchover. (#41)
- **[Task]** **Deploying updated scheduled jobs** — Bringing the new background jobs online to run in parallel with the existing ones while they're monitored. (#43)
- **[Task]** **Gradual switchover, lower-risk jobs** — Retiring the least critical legacy background jobs once their replacements prove stable. (#44)
- **[Task]** **Gradual switchover, mid-tier jobs** — Retiring the next set of legacy stats jobs after a monitoring period. (#45)
- **[Task]** **Gradual switchover, critical jobs** — Carefully retiring the most important lead-processing and offer-cap jobs, with the ability to roll back instantly. (#46, critical)
- **[Task]** **Rollback procedures** — Documenting and testing how to quickly revert each system if something goes wrong. (#48)
- **[Task]** **Troubleshooting runbooks** — Creating step-by-step guides for handling common issues like lead-processing or pre-ping failures. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: e5b525ea5deaae522eb5c0b96bdc06719dcba9b7faa6fb95d679ecf984c97411 -->
