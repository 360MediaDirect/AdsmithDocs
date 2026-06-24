# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 20:34:32 UTC · 33 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard** — Choosing "Custom" in the date filter will open a proper start- and end-date picker so you can view dashboard data for any range you like, instead of being limited to presets like Today or This Month. (#58)
- **[Feature]** **Make the Edit and Preview buttons work on detail pages** — On Placement, Modal, Offer, and Advertiser detail screens, the Edit, Preview, and Pull Leads buttons will actually do something when clicked instead of sitting there unresponsive. (#154)
- **[Feature]** **Move Sub-ID Stats to the Dashboard** — Sub-ID statistics will be relocated out of the placement form and into the Dashboard's reporting area, where this kind of information belongs. (#236)
- **[Bug]** **Bring back the missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date-range selector will update them — right now only the system overview loads. This is high priority. (#240)
- **[Feature]** **15-minute detail on the offer timespan chart** — The offer detail timespan stats will show 15-minute increments again, giving you a fine-grained view to spot errors and issues with offers or partner servers as they happen. (#243)
- **[Feature]** **New "Other Dashboard" views and an activity log** — You'll get dedicated views for long-running ("Offers with Legs") and CLP offers, with low-converting offers highlighted, plus a searchable log of changes like pausing offers or adjusting daily caps. (#256)
- **[Feature]** **Show full advertiser and placement names** — Long advertiser and placement names will no longer be cut off with "…" in dashboard views, so you can always read the whole name. (#260)
- **[Feature]** **Remove the ID/number column** — The ID column will be dropped from dashboard tables to free up screen space for the information you actually use. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon (for example, "Foo: Bar: Acme Publishing" becomes "Acme Publishing"), making lists easier to scan. (#262)
- **[Feature]** **A consistent dashboard color scheme** — A defined set of colors will be applied across the Dashboard for better, more consistent readability. (#263)

## Offers

- **[Feature]** **Set all offer details at creation time** — You'll be able to configure piggyback offers, HD pixel placements, and ZIP code targeting right when you create an offer, instead of having to save it first and come back to edit. This is high priority. (#142)
- **[Feature]** **Enforce required fields before a pre-ping sends** — When a pre-ping runs before pushing data, leads missing required fields will be stopped up front rather than relying on the advertiser's system to catch them. (A decision is still needed on whether to adopt this behavior.) (#218)
- **[Feature]** **Distinct status colors for offers** — Paused offers will show red, Active green, and Capped yellow/orange, so you can tell at a glance which is which in offer lists and dashboard indicators. (#246)
- **[Feature]** **Easier advertiser and state targeting on the offer form** — You'll be able to type to search for an advertiser instead of scrolling, and enter state targeting as a typed or pasted comma-separated list (e.g. CA, TX, FL). (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in a group to the Conflicting Offers list in one step, saving significant time. (#250)
- **[Task]** **Offer row action links and a Trends page** — Each offer will gain quick action links (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an offer activity page showing lead and revenue trends and a daily performance breakdown. (#252)

## General / Across the App

- **[Feature]** **Dark and Light mode** — You'll be able to switch the whole admin between dark and light themes from your user menu, with your choice remembered between visits — helpful for different lighting and personal preference. (#59)
- **[Feature]** **Bring back the Campaigns module** — Campaign management from the legacy system will be added so you can create, edit, and configure campaigns and offer groups directly in New Adsmith Frontend. This is a high-priority core feature. (#200)
- **[Feature]** **Brand guidelines to improve AI output** — A comprehensive brand-guidelines document will be established and used as the main input for AI-generated content, raising the quality and consistency of results. (#264)
- **[Feature]** **Prevent two people overwriting each other's edits** — When you open a record to edit, others will see it's being worked on, and the app will warn you if a record changed since you opened it — so changes are no longer silently lost when two people edit the same item. (#267)

## Flows

- **[Task]** **Fix the look of the Flow form** — The Flow form's text boxes, color pickers, checkboxes, and paired fields will be properly styled and laid out side-by-side, matching the polish of the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — When building a flow, you'll be able to add every available form field at once instead of adding them one at a time. (#224)
- **[Feature]** **Clearer "Step order" setting** — The step-order control on the flow form will get clearer labels or help text so it's obvious what it controls and what the values mean. (#226)

## Surveys

- **[Feature]** **Better TCPA consent checkbox** — The TCPA consent checkbox on the lander will be larger, rounded, and properly aligned with its text for a cleaner, more readable look. (#229)
- **[Bug]** **Let visitors decline a CPA offer** — Visitors will be able to decline, skip past, or exit a CPA offer instead of being forced to click "Yes," which currently traps them mid-flow. This is high priority. (#233)
- **[Bug]** **Stop duplicate offer actions when changing your mind** — Toggling Yes → No → Yes on a survey offer will no longer fire the offer twice (opening a second tab or submitting a duplicate lead). This high-priority fix protects against double billing and compliance issues. (#266)

## Placements

- **[Bug]** **Clean up the placement create/edit form** — Unfamiliar new fields on the placement form will be reviewed and removed or relabeled, and missing links like Preview and Details will be restored to match what you expect. (#234)
- **[Feature]** **Reorder assigned offers by hand** — On placements, selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)
- **[Feature]** **Drag-and-drop offer assignment (UAT follow-up)** — Confirms the same improvement: assigned offers keep a manual order you set by dragging, with an "X" to remove and taxonomy filtering, addressing the failed offer-assignment test. (#255)

## Link Testing

- **[Feature]** **Default to the placement you came from** — When you open Link Testing from a placement, that placement will already be selected, so you don't have to pick it each time. (#238)
- **[Bug]** **Show a clear error for invalid links** — Testing an invalid link will display a proper failure message in Link Testing instead of dumping you back on the dashboard with no explanation. (#239)

## Modals

- **[Bug]** **Let visitors close or decline a modal offer** — The Close button on offer modals will work, and single-offer modals will offer a way to dismiss or skip — so visitors are no longer stuck with no way out. (#265)

## Properties

- **[Feature]** **Search box for the publisher selector** — On the property form, you'll be able to type to find a publisher instead of scrolling through the whole list. (#237)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 5fd3825deeedaffec43ce35ec69041d36954e26c6d8d81fe302043b883f8876e -->
