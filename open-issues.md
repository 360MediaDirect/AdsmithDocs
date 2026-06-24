# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 18:35:19 UTC · 32 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Bug]** **Custom date range on the Dashboard** — When you pick "Custom" on the Dashboard date filter, you'll now get start and end date pickers so you can view data for any specific stretch of time instead of only the preset options. (#58)
- **[Feature]** **Light mode option** — You'll be able to switch the admin between the current dark theme and a new light theme, with your choice remembered next time you log in. (#59)
- **[Feature]** **Working buttons on detail pages** — The Edit, Preview, and Pull Leads buttons on placement, modal, offer, and advertiser detail pages will actually do something when clicked instead of being unresponsive. (#154)
- **[Feature]** **Sub-ID Stats moved to the Dashboard** — Sub-ID Stats will be relocated out of the placement form and into the Dashboard reporting area, where they belong. (#236)
- **[Bug]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will load again on the Dashboard, and the date range selector will update them. A high-priority fix. (#240)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer timespan chart will show activity in 15-minute increments, making it much easier to spot offer or partner issues as they happen. (#243)
- **[Feature]** **Clearer offer status colors** — Paused offers will show in red, Capped in yellow/orange, and Active in green, so you can tell statuses apart at a glance. (#246)
- **[Feature]** **New monitoring views and activity log** — Adds "Offer with Legs" and "CLP Performance" views to highlight low-converting offers, plus a searchable record of changes like pausing offers or adjusting caps. (#256)
- **[Feature]** **Full advertiser and placement names** — Long advertiser and placement names will no longer be cut off with "…" on the Dashboard, so you can read them in full. (#260)
- **[Feature]** **More room on Dashboard tables** — The ID/number column will be removed from Dashboard tables to free up screen space. (#261)
- **[Feature]** **Cleaner publisher and property names** — Publisher and property names will display only the meaningful part after the last colon (e.g. "Acme Publishing" instead of "Foo: Bar: Acme Publishing"). (#262)
- **[Feature]** **Consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for better, more consistent readability. (#263)

## Offers
- **[Feature]** **More options when first creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting will be available right when you create an offer, so you won't have to save it and then edit it to add them. A high-priority improvement. (#142)
- **[Feature]** **Stricter pre-ping checks** — When a pre-ping requires certain fields, a lead missing those fields will be stopped before the request is sent, preventing incomplete leads from slipping through. (#218)
- **[Feature]** **Easier offer form entry** — The Advertiser field will get a type-to-search box, and state targeting will accept a typed or pasted comma-separated list (like CA, TX, FL) in addition to picking. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in an offer group to the Conflicting Offers list in one step, saving a lot of manual work. (#250)
- **[Task]** **Quick action links under each offer** — Each offer will show familiar links like Edit, Quick Edit, Trash, View, Preview, Trends, and Details, with Trends opening an offer performance page. (#252)

## Placements
- **[Bug]** **Review the placement create/edit form** — Unfamiliar new fields on the placement form will be cleaned up or clarified, and missing links such as Preview and Details will be restored. (#234)
- **[Feature]** **Reorder assigned offers by dragging** — Selected offers will default to manual order with drag-and-drop reordering, an "x" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)
- **[Feature]** **Manual offer ordering on the transfer list** — Tracked from UAT, this covers the same improvements as above: a Manual Order default, drag-and-drop, a remove button, and taxonomy filtering on the offer assignment list. (#255)

## Surveys
- **[Bug]** **Visitors can move past CPA offers** — Fixes a trap where visitors had to click "Yes" to continue with no way to decline or exit a CPA offer. A high-priority fix. (#233)
- **[Bug]** **No accidental duplicate submissions** — Fixes a problem where switching Yes → No → Yes on an offer could open a second tab or submit a duplicate lead; the action will now fire only once. A high-priority fix. (#266)
- **[Feature]** **Better TCPA consent checkbox** — The consent checkbox on the lander will be made larger, rounded, and properly aligned with its consent text. (#229)

## Flows
- **[Task]** **Polished Flow form styling** — Fixes unstyled text boxes, color pickers, and checkboxes on the Flow form and restores side-by-side fields so it matches the look of the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button** — When building a flow, you'll be able to add every available form field at once instead of adding them one by one. (#224)
- **[Feature]** **Clearer step order control** — The step-order setting will get labels and help text so it's obvious what it controls and what the values mean. (#226)

## Link Testing
- **[Feature]** **Pre-selected placement** — When you open Link Testing from a placement, that placement will already be selected, saving you from picking it each time. (#238)
- **[Bug]** **Clear error for invalid links** — Testing an invalid link will show a clear failure message instead of dumping you back on the dashboard. (#239)

## Modals
- **[Bug]** **Visitors can close modal offers** — Fixes a dead Close button that could trap visitors on a single linkout/CPA offer with no way to dismiss or decline it. (#265)

## Properties
- **[Feature]** **Searchable publisher selector** — The publisher dropdown on the property form will let you type to search instead of scrolling to find the one you want. (#237)

## General / Across the App
- **[Feature]** **Campaigns module** — Brings the legacy Campaigns feature into New Adsmith Frontend so you can view, create, edit, and configure campaigns and offer groups. A critical, high-priority addition. (#200)

## Behind the Scenes
- **[Feature]** **Brand guidelines for AI output** — A comprehensive brand-guidelines document will be established and used as the main reference for AI-generated content, improving the quality and consistency of results. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 9de43829593399b79cce2cce58f007e1e79ca8e38db3ea17ad6154a6f8b9c16d -->
