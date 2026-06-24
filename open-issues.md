# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 19:32:42 UTC · 32 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Bug]** **Custom date range on the Dashboard date filter** — Choosing "Custom" will open a proper start- and end-date picker so you can view Dashboard data for any range you like, instead of only the preset options. (#58)
- **[Feature]** **Make the Edit, Preview, and Pull Leads buttons work** — On Placement, Modal, Offer, and Advertiser detail pages, these buttons currently do nothing when clicked. They'll be wired up so they take you where you expect. (#154)
- **[Feature]** **Move Sub-ID Stats into the Dashboard** — Sub-ID statistics will be relocated out of the placement form and into the Dashboard reporting area, where they belong. (#236)
- **[Bug]** **Restore the missing Dashboard sections** — Campaign stats, top offers, and watch lists will load again, and changing the date range will update them. Today only the system overview appears. (#240)
- **[Feature]** **New monitoring views and an activity log** — Adds an "Other Dashboard" area with views for long-running offers and low-converting CLP offers, plus a searchable record of changes like pausing offers or adjusting caps. (#256)
- **[Feature]** **Show full advertiser and placement names** — Names will no longer be cut off with "…" so you can read them in full. (#260)
- **[Feature]** **Remove the ID/number column** — Dropping this column frees up screen space for the information you actually use. (#261)
- **[Feature]** **Cleaner publisher and property names** — When a name contains colons, only the part after the last colon will be shown (e.g. "Foo: Bar: Acme Publishing" becomes "Acme Publishing"). (#262)
- **[Feature]** **Standardized Dashboard colors** — A defined color palette will be applied consistently across the Dashboard for better readability. (#263)

## Offers
- **[Feature]** **Set all offer details when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting can be filled in right away, instead of having to save the offer first and then edit it. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — When a pre-ping is set to run before pushing data, a lead missing required fields will be stopped immediately rather than being sent out and relying on the partner to reject it. (#218)
- **[Feature]** **Clearer offer status colors** — Paused will show red, Active green, and Capped yellow/orange, so Paused and Capped are no longer easy to confuse. (#246)
- **[Feature]** **Easier offer form entry** — The Advertiser field gets a type-to-search box, and state targeting will accept a typed or pasted comma-separated list (like CA, TX, FL). (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in a group to the conflicting list in one step, saving considerable time. (#250)
- **[Task]** **Quick action links under each offer** — Brings back the familiar row actions (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an Offer Activity page showing lead and revenue trends. (#252)

## Placements
- **[Bug]** **Tidy up the placement create/edit form** — Unfamiliar fields will be reviewed and removed, relabeled, or explained, and missing links such as Preview and Details will be restored. (#234)
- **[Feature]** **Manually order and manage assigned offers** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)
- **[Feature]** **Reorder offers in the assignment list** — A companion request to support manual ordering, drag-and-drop, an "X" to remove, and taxonomy filtering when assigning offers to a placement. (#255)

## Surveys
- **[Feature]** **Better-looking TCPA consent checkbox** — The consent checkbox will be made larger, rounded, and properly aligned with its text on the live lander. (#229)
- **[Bug]** **Let visitors decline or move past a CPA offer** — Today visitors are forced to click "Yes" with no way to decline or exit, trapping them mid-flow. They'll be able to continue without being forced into the offer. (#233)
- **[Bug]** **Prevent duplicate offer firing on a survey** — If a visitor clicks Yes, then No, then Yes again, the offer currently fires a second time (opening another tab or submitting a duplicate lead). It will fire only once. (#266)

## Flows
- **[Task]** **Fix the Flow form's appearance** — Textareas, color pickers, checkboxes, and paired fields will be styled and laid out correctly to match the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Add every available form field in one click instead of adding them one at a time. (#224)
- **[Feature]** **Make the "Step order" setting understandable** — Clearer labels and help text (or a reworked control) so it's obvious what the step order controls and what the values mean. (#226)

## Link Testing
- **[Feature]** **Default to the placement you opened it from** — When you start Link Testing from a placement, that placement will already be selected so you don't have to pick it manually. (#238)
- **[Bug]** **Show an error for invalid links** — Testing a bad link will return a clear failure message instead of dumping you back on the dashboard. (#239)

## Reports
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will support 15-minute increments, restoring the close monitoring needed to catch offer or partner-server issues quickly. (#243)

## Properties
- **[Feature]** **Search box for the Publisher selector** — Type to find a publisher on the property form instead of scrolling through a long list. (#237)

## Modals
- **[Bug]** **Let visitors close or decline a modal offer** — A modal showing a single linkout/CPA offer currently has a Close button that does nothing, trapping the visitor. The Close button will work and visitors will be able to dismiss the offer. (#265)

## Campaigns
- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — Recreates the campaign management from the legacy admin, letting you view, create, edit, and configure campaigns and their offer groups. This is a high-priority gap. (#200)

## General / Across the App
- **[Feature]** **Dark/Light mode toggle** — A theme switcher will let you choose between the current dark look and a new light option, with your choice remembered between visits. (#59)

## Behind the Scenes
- **[Feature]** **Brand guidelines as the basis for AI-generated content** — A comprehensive brand-guidelines document will be established and used as the primary input to improve the quality of AI-generated output. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f8e70aaf676e6166eef6b3707647ee12ef886cf5f4291fa5acdc80957f95f545 -->
