# Open Issues — Plain-Language Overview

_Last updated 2026-06-25 09:04:09 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the Dashboard date filter will open a start/end date picker so you can view data for any range you like, instead of being limited to preset options like Today or This Month. (#58)
- **[Bug]** **Bring back missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date-range selector will properly update them so you see complete, current data again. (#240)
- **[Feature]** **Make Edit, Preview, and Pull Leads buttons work** — On the Placement, Modal, Offer, and Advertiser detail pages, these buttons will actually open the right screen when clicked, instead of doing nothing. (#154)
- **[Feature]** **New monitoring views and a full activity log** — Adds "Offer with Legs" and "CLP Offers Performance" views (flagging offers converting under 30%), plus a searchable record of every change—like pausing an offer or adjusting daily caps—so you can audit and troubleshoot quickly. (#256)
- **[Feature]** **Move Sub-ID Stats to the Dashboard** — Sub-ID Stats will live in the Dashboard reporting area rather than buried inside the placement form, making them easier to find. (#236)
- **[Feature]** **15-minute detail on the offer timespan chart** — The offer detail timespan stats will show data in 15-minute increments, helping you spot offer or partner-server issues as they happen. (#243)
- **[Feature]** **Consistent Dashboard color scheme** — A defined color palette will be applied across the Dashboard for cleaner, more readable visuals. (#263)

## Offers

- **[Feature]** **Set all offer fields when first creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting can be entered right when you create an offer, instead of having to save first and then edit. This is high priority. (#142)
- **[Feature]** **Quicker advertiser search and state targeting on the offer form** — You'll be able to type to search for an advertiser, and enter state targeting as a typed or pasted comma-separated list (e.g. CA, TX, FL) in addition to picking from a menu. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers at once** — On the Delivery & Settings tab, you can add every offer in an offer group to the Conflicting Offers list in one step, saving considerable time. (#250)
- **[Feature]** **Enforce required Pre-Ping fields before pushing** — When a pre-ping runs before a data push, missing required fields will stop the lead instead of letting it slip through, matching how the "Before Offer Displays" trigger already works. (Pending confirmation that this is the intended behavior.) (#218)

## Flows

- **[Feature]** **Add all form fields in one click** — When building a flow, a new button lets you add every available field to the Form tab at once, instead of adding them one at a time. (#224)
- **[Feature]** **Clearer "Step order" setting** — Helpful labels and guidance will explain what the step-order control does and what its values mean, so it's no longer confusing. (#226)
- **[Feature]** **Better-looking consent checkbox on landers** — The TCPA consent checkbox will be larger, rounded, and properly lined up with its text for a cleaner appearance. (#229)
- **[Task]** **Fix the Flow form's appearance** — The Flow form will display correctly, with properly styled text boxes, color pickers, and checkboxes, and paired fields shown side-by-side instead of stacked—matching the polish of the Placement and Modal forms. (#152)

## General / Across the App

- **[Feature]** **Protection against overwriting each other's edits** — If two people open the same record, the app will warn you that someone else is editing or has already saved changes, preventing one person from silently wiping out the other's work. Rolling out to offers first, then all other editable screens. (#267)
- **[Feature]** **Dark and Light mode toggle** — You'll be able to switch the entire Admin between dark and light themes from your user menu, and your choice will be remembered next time you sign in. (#59)
- **[Feature]** **Adopt comprehensive brand guidelines** — A documented set of brand guidelines will be established and used as the primary input for AI-generated content, improving the quality and consistency of results. (#264)

## Link Testing

- **[Feature]** **Pre-select the placement you came from** — When you open Link Testing from a placement, that placement will already be selected, so you don't have to choose it manually. (#238)
- **[Bug]** **Show a clear error for invalid links** — Testing an invalid link will display a proper failure message in Link Testing, instead of unexpectedly sending you to the Dashboard. (#239)

## Placements

- **[Feature]** **Easier offer ordering on placements** — Selected offers will default to Manual Order with drag-and-drop reordering, an "X" to remove an offer (so clicking is reserved for dragging), and the ability to filter the offer list by taxonomy. (#235)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — A Campaigns area will let you view, create, edit, and configure campaigns—including offer groups, CTA text, offer handling and order, and marketing partners—matching the legacy admin. This is a critical, high-priority gap. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8a5ffa5558be3c2ea09af2a6c1cf14599c4f7d3a480af89a537b4cc4b0bd651a -->
