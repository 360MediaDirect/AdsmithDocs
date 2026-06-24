# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 15:48:01 UTC · 32 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a proper start/end date picker, so you can view dashboard data for any range you like instead of only the preset options. (#58)
- **[Feature]** **Light mode option** — A theme switch will let you flip between the current dark look and a new light look, with your choice remembered the next time you sign in. (#59)
- **[Feature]** **Make detail-page buttons work** — Edit, Preview, and Pull Leads buttons on Placement, Modal, Offer, and Advertiser detail pages will actually do something when clicked instead of sitting there unresponsive. (#154)
- **[Feature]** **Sub-ID Stats moving to the Dashboard** — Sub-ID Stats will be relocated out of the placement form and into the Dashboard's reporting area, where this kind of information belongs. (#236)
- **[Bug]** **Restore the missing dashboard sections** — Campaign stats, top offers, and watch lists will load again alongside the system overview, and the date-range selector will update them. (#240)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer timespan chart will show activity in 15-minute increments so you can spot offer or partner-server issues quickly. (#243)
- **[Feature]** **Clearer offer status colors** — Paused will show red, Active green, and Capped yellow/orange, so you can tell them apart at a glance across the offer list and dashboard. (#246)
- **[Feature]** **New monitoring views and an activity log** — Adds "Offer with Legs" and "CLP Performance" views (flagging low-converting CLP offers) plus a searchable record of changes like pausing offers or adjusting daily caps. (#256)
- **[Feature]** **Show full advertiser and placement names** — Long advertiser and placement names will no longer be cut off with "…", so you can always read the whole name. (#260)
- **[Feature]** **Remove the ID/number column** — Dropping the ID column from dashboard tables frees up screen space for the information that matters. (#261)
- **[Feature]** **Cleaner publisher and property names** — Publisher and property names will display only the part after the last colon (e.g. "Acme Publishing"), making them easier to read. (#262)
- **[Feature]** **Consistent dashboard colors** — A defined color palette will be applied across the dashboard for better, more consistent readability. (#263)

## Offers

- **[Feature]** **Set all offer details when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting will be available right when you create an offer, instead of forcing you to save first and then edit. (#142)
- **[Feature]** **Enforce required fields before a lead is pushed** — When a pre-ping runs before data is pushed, missing required fields will stop the lead immediately rather than letting incomplete data slip through. (#218)
- **[Bug]** **Advertiser info missing on the Offers report** — Fixes the lingering gap where some offers show no advertiser, so advertiser details appear for every offer in the report. (#242)
- **[Feature]** **Faster advertiser and state entry on the offer form** — You'll be able to type to search for an advertiser, and enter state targeting as a typed or pasted comma-separated list (e.g. CA, TX, FL). (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in a group to the Conflicting Offers list in one step, saving a lot of manual clicking. (#250)
- **[Task]** **Quick action links under each offer** — Brings back the familiar row actions (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an offer performance page showing leads, revenue, and daily breakdowns. (#252)
- **[Bug]** **Offer preview shows raw code and broken linkouts** — More Info and TCPA content will display as proper formatted text and working links, and Linkout offers will link out correctly from the preview. (#259)

## Flows

- **[Task]** **Fix the look of the Flow form** — Textareas, color pickers, checkboxes, and paired fields will be styled correctly and laid out side by side, matching the polished look of the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field with a single click. (#224)
- **[Feature]** **Clearer "Step order" setting** — The step-order control will get labels and help text so it's obvious what it controls and what each value means. (#226)

## Placements

- **[Bug]** **Tidy up the placement create/edit form** — Unfamiliar new fields will be reviewed (removed, relabeled, or explained) and missing links like Preview and Details will be restored to match what you expect. (#234)
- **[Feature]** **Reorder and manage assigned offers easily** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and a taxonomy filter to find offers faster. (#235)
- **[Feature]** **Drag-and-drop offer ordering (follow-up)** — Covers the same improvement to the placement offer transfer list: manual ordering, drag-and-drop, remove buttons, and taxonomy filtering. (#255)

## Surveys

- **[Bug]** **Visitors can move past a CPA offer** — Fixes a trap where visitors were forced to click "Yes" with no way to decline or continue, so people can properly proceed through the flow. (#233)
- **[Feature]** **Better TCPA consent checkbox** — The consent checkbox on the lander will be larger, rounded, and properly aligned with its text for a cleaner, clearer look. (#229)

## Link Testing

- **[Feature]** **Default to the placement you came from** — When you open Link Testing from a placement, that placement will already be selected so you don't have to pick it yourself. (#238)
- **[Bug]** **Clear error for invalid links** — Testing an invalid link will show a proper failure message instead of unexpectedly sending you to the dashboard. (#239)

## Properties

- **[Feature]** **Search box for the publisher selector** — You'll be able to type to find a publisher on the property form instead of scrolling through a long list. (#237)

## General / Across the App

- **[Feature]** **Stronger brand guidelines for AI output** — A comprehensive brand-guidelines document will become the main reference for AI-generated content, improving the quality and consistency of results. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f0408a319ce43448b86d34c13f452118c887526461a9d389ca678a7974fd8090 -->
