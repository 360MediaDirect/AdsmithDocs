# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 21:30:51 UTC · 29 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard** — Choosing "Custom" in the Dashboard date filter will open a start- and end-date picker, so you can view results for any time period you like instead of only the preset options. (#58)
- **[Feature]** **Working Edit, Preview, and Pull Leads buttons on detail pages** — The Edit, Preview, and Pull Leads buttons on Placement, Modal, Offer, and Advertiser detail pages will actually do something when clicked, taking you where you expect to go. (#154)
- **[Feature]** **Sub-ID Stats moving to the Dashboard** — The Sub-ID Stats view is being relocated out of the placement form and into the Dashboard reporting area, where it's easier to find. (#236)
- **[Bug]** **Missing dashboard sections restored** — Campaign stats, top offers, and watch lists will be back on the Dashboard, and the date-range selection will update them. (#240)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will show activity in 15-minute increments, making it easier to spot and react to issues with offers or partner servers quickly. (#243)
- **[Feature]** **Clearer offer status colors** — Paused offers will show in red, Active in green, and Capped in yellow/orange, so statuses are easy to tell apart at a glance across the offer list and dashboard. (#246)
- **[Feature]** **New "Other Dashboard" views and activity log** — Adds dedicated views for monitoring offer longevity and CLP offer performance (flagging those converting under 30%), plus a searchable log that records changes like pausing offers or cap adjustments. (#256)
- **[Feature]** **Full advertiser and placement names** — Advertiser and placement names will no longer be cut off with "…", so you can always read the complete name. (#260)
- **[Feature]** **More room on dashboard tables** — The ID/number column is being removed from dashboard tables to free up screen space for the information that matters. (#261)
- **[Feature]** **Cleaner publisher and property names** — Publisher and property names will display only the part after the last colon (for example, "Foo: Bar: Acme Publishing" shows as "Acme Publishing"), keeping lists tidy and readable. (#262)
- **[Feature]** **A consistent dashboard color scheme** — A defined color palette will be applied across the dashboard for better, more consistent readability. (#263)

## General / Across the App

- **[Feature]** **Dark and Light mode** — A theme switcher is coming so you can choose between the current dark look and a new light mode; your choice is remembered and applies instantly across the whole admin area. (#59)
- **[Feature]** **Campaigns module** — The Campaigns area from the legacy admin is being added so you can view, create, edit, and configure campaigns and their offer groups directly in New Adsmith Frontend. This is a high-priority, core feature. (#200)
- **[Feature]** **Search box for the publisher selector** — On the property form, you'll be able to type to find a publisher instead of scrolling through the full list. (#237)
- **[Feature]** **Link Testing remembers your placement** — When you open Link Testing from a placement, that placement will be pre-selected for you instead of making you pick it again. (#238)
- **[Bug]** **Clear error for invalid test links** — Testing an invalid link will show a clear failure message in Link Testing, rather than unexpectedly sending you to the dashboard. (#239)
- **[Feature]** **Protection against overwriting each other's work** — When two people open the same record, New Adsmith Frontend will warn you if someone else has it open or has changed it since you opened it, so edits aren't silently lost. (#267)

## Offers

- **[Feature]** **More fields available when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting can be set right when you create an offer, instead of having to save first and then edit. This is high priority. (#142)
- **[Feature]** **Required pre-ping fields actually enforced** — For pre-pings set to run before a data push, missing required fields will stop the lead from going through, matching how the "before offer displays" option already works. (#218)
- **[Feature]** **Easier advertiser and state targeting on the offer form** — The Advertiser field gets a type-to-search box, and state targeting will accept a typed or pasted comma-separated list (like CA, TX, FL) in addition to picking states. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in an offer group to the Conflicting Offers list in one step, saving a lot of manual effort. (#250)
- **[Task]** **Quick action links on each offer** — Action links (Edit, Quick Edit, Trash, View, Preview, Trends, Details) will appear under each offer, with Trends opening an offer activity page showing lead and revenue trends over time. (#252)

## Flows

- **[Task]** **Polished Flow form styling** — The Flow form is being cleaned up so textareas, color pickers, checkboxes, and paired fields look right and line up side by side, matching the rest of the app. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — When building a flow, you'll be able to add every available form field at once instead of one at a time. (#224)
- **[Feature]** **Clearer step-order setting** — The step-order control on the flow form will get labels and help text so it's obvious what it controls and what the values mean. (#226)
- **[Feature]** **Better TCPA consent checkbox** — On the rendered lander, the TCPA consent checkbox will be larger, rounded, and properly aligned with its consent text. (#229)

## Placements

- **[Feature]** **Reorder assigned offers by drag-and-drop** — Selected offers will default to Manual Order, let you drag to reorder, and include an "X" to remove an offer, plus the ability to filter the offer list by taxonomy. (#235)
- **[Feature]** **Manual offer ordering on placements (UAT follow-up)** — Confirms the same improvements to the offer assignment list: manual ordering by default, drag-and-drop reordering, an "X" to remove, and taxonomy filtering. (#255)

## Behind the Scenes

- **[Feature]** **Stronger brand guidelines for AI output** — The team will use a comprehensive brand-guidelines document as the main input for AI-generated content, improving the quality and consistency of results. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 5b4f68aa07d694e6d0a2e1c780cf3856d4173d5ef95d2b9c004932a578fabb33 -->
