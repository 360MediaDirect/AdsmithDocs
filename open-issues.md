# Open Issues — Plain-Language Overview

_Last updated 2026-06-23 12:55:30 UTC · 50 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Set every offer detail at creation time** — You'll be able to configure piggyback offers, HD pixel placements, and ZIP-code targeting right when you create an offer, instead of having to save it first and then come back to edit it. (#142)
- **[Bug]** **Advertiser names showing on the Offers report** — A fix so every offer displays its advertiser in the Offers report; right now some are blank even after a data cleanup. (#242)
- **[Bug]** **Status filter on the Offers report** — You'll be able to narrow the Offers report to a status (Active, Paused, or Capped) instead of seeing every offer at once. (#244)
- **[Bug]** **Offer images will display in the offer form** — Fixes images that currently fail to appear when viewing or editing an offer. (#247)
- **[Bug]** **Offer preview shows formatted content and working links** — Fixes preview tabs that display raw HTML text and "Linkout" offers that don't redirect, so the More Info and TCPA content render properly. (#259)
- **[Feature]** **Faster offer setup with search and typed state lists** — Adds a type-to-search box to the Advertiser picker and lets you enter state targeting as a typed or pasted comma-separated list (e.g. CA, TX, FL). (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers at once** — On the Delivery & Settings tab you'll be able to add every offer in a group to the Conflicting Offers list in one step, saving a lot of manual work. (#250)
- **[Feature]** **15-minute detail in offer timespan stats** — Restores 15-minute increments on the offer detail chart so you can spot offer or partner-server issues quickly. (#243)
- **[Feature]** **Distinct colors for offer statuses** — Paused will show red, Capped yellow/orange, and Active green, so the two are no longer easy to confuse in lists and dashboard indicators. (#246)
- **[Feature]** **Required pre-ping fields enforced before a lead is sent** — A high-priority change so a lead missing required fields is stopped up front rather than relying on the advertiser's response. (Decision needed before building.) (#218)
- **[Task]** **Quick action links under each offer** — Brings back the familiar row actions (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an offer activity page showing lead, revenue, and daily performance. (#252)

## Dashboard

- **[Bug]** **Restore missing dashboard sections** — A high-priority fix so campaign stats, top offers, and watch lists load again (today only the system overview appears), with the date range updating them. (#240)
- **[Bug]** **Custom date range on the Dashboard** — Choosing "Custom" will open a start/end date picker with Apply and Cancel, so you can view dashboard data for any range you choose. (#58)
- **[Feature]** **Working Edit, Preview, and Pull Leads buttons** — These buttons on Placement, Modal, Offer, and Advertiser detail pages will actually do something when clicked instead of nothing. (#154)
- **[Feature]** **Sub-ID stats moving to the Dashboard** — Sub-ID Stats will live in the Dashboard reporting area rather than buried in the placement form. (#236)
- **[Feature]** **New monitoring views and an activity log** — Adds "Offer with Legs" and CLP performance views (highlighting offers converting under 30%) plus a searchable log of changes like pausing an offer or adjusting daily caps. (#256)
- **[Feature]** **Full advertiser and placement names** — Names will no longer be cut off with "…", so you can read them in full. (#260)
- **[Feature]** **More room in dashboard tables** — Removes the ID/number column to free up screen space. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon (e.g. "Foo: Bar: Acme Publishing" shows as "Acme Publishing"). (#262)
- **[Feature]** **A consistent dashboard color scheme** — A defined palette will be applied across the dashboard for better readability. (#263)

## Flows & Surveys

- **[Bug]** **Visitors can decline or move past CPA offers** — A high-priority fix so consumers are no longer forced to click "Yes" with no way to decline or continue, which currently traps them mid-flow. (#233)
- **[Task]** **Tidy up the Flow form's appearance** — Fixes unstyled text boxes, color pickers, and checkboxes, and restores side-by-side fields so the Flow form looks consistent with the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Add every available form field to a flow in one click instead of one at a time. (#224)
- **[Feature]** **Clearer "step order" setting** — Adds labels and help text so it's obvious what the step-order control does and what its values mean. (#226)
- **[Feature]** **Flows start directly on the form** — Removes the extra "Claim your offers" page so visitors land straight on the form fields. (#228)
- **[Feature]** **Better TCPA consent checkbox** — Makes the consent checkbox larger, rounded, and properly aligned with its text on the published lander. (#229)
- **[Feature]** **Footer with copyright and site name** — The lander footer will include the copyright line and site name pulled from General Information. (#232)

## Placements

- **[Bug]** **Clean up the placement create/edit form** — Reviews unfamiliar new fields (to remove, relabel, or explain) and restores missing links like Preview and Details. (#234)
- **[Feature]** **Reorder assigned offers by hand** — Defaults offer sorting to Manual Order, lets you drag selected offers into the order you want, adds an "X" to remove an offer, and adds a filter by taxonomy. (#235)
- **[Feature]** **Drag-and-drop offer assignment (UAT follow-up)** — The same offer transfer-list improvements, tracked from formal testing: manual order, drag-and-drop, remove button, and taxonomy filtering. (#255)

## General / Across the App

- **[Feature]** **Campaigns module** — A critical, high-priority addition that brings back campaign management—creating, editing, and configuring campaigns and offer groups—which is currently missing from New Adsmith Frontend. (#200)
- **[Feature]** **Dark and Light mode** — A theme switcher so you can choose a light or dark appearance (currently dark only), with your choice remembered between visits. (#59)
- **[Task]** **Users area review** — A documentation review comparing the new Users screens to the old system to confirm which features still need to be added (e.g. bulk actions, last-login info). (#80)

## Link Testing

- **[Bug]** **Clear error for invalid links** — Testing a bad link will show a failure message in Link Testing instead of dropping you back on the dashboard. (#239)
- **[Feature]** **Link Testing remembers the placement** — When opened from a placement, that placement is pre-selected so you don't have to pick it each time. (#238)

## Properties

- **[Feature]** **Search the publisher list** — Adds type-to-search to the publisher picker on the property form so you don't have to scroll to find one. (#237)

## Behind the Scenes

- **[Task]** **Real-time "today" stats** — Behind-the-scenes work so the dashboard's "today" numbers come from up-to-the-hour data in the correct (Eastern) time zone. (#34)
- **[Task]** **Faster historical reporting** — Automated rollups that summarize stats for quicker access to past performance. (#35)
- **[Task]** **Review an older stats job** — Maintenance to decide whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Speed improvements for the survey system** — Adds caching of placement, offer, and cap data to keep things responsive at high volume. High priority. (#42)
- **[Task]** **Side-by-side pre-ping testing** — Runs the new pre-ping process alongside the old one to confirm results match before switching over. (#40)
- **[Task]** **Per-advertiser pre-ping checks** — Verifies each advertiser's pre-ping works correctly before the switchover. (#41)
- **[Task]** **Parallel run of scheduled jobs** — Runs new and old background jobs together in production while monitoring for differences. (#43)
- **[Task]** **Phased switchover of background jobs (Tier 3)** — Retires the first group of older scheduled jobs once their replacements prove stable. (#44)
- **[Task]** **Phased switchover of background jobs (Tier 2)** — Retires the next group of stats-related scheduled jobs after a week of monitoring. (#45)
- **[Task]** **Phased switchover of background jobs (Tier 1)** — Retires the most critical scheduled jobs last, with close monitoring and instant rollback ready. (#46)
- **[Task]** **Documented rollback steps** — Written procedures to quickly revert each production system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides** — Step-by-step guides for handling common operational issues like lead-processing or stats hiccups. (#49)
- **[Bug]** **Fix data-sync that wipes good records** — A critical, high-priority fix to the process that copies production data to the test environment, which is currently overwriting records and causing missing stats and offer data. (#241)
- **[Feature]** **Stronger brand guidelines for AI output** — Establishing a single, detailed brand-guidelines document to improve the quality of AI-generated results. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: e5b525ea5deaae522eb5c0b96bdc06719dcba9b7faa6fb95d679ecf984c97411 -->
