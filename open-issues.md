# Open Issues — Plain-Language Overview

_Last updated 2026-06-25 05:20:39 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard filter** — Picking "Custom" in the Dashboard date filter will open a proper start- and end-date picker so you can view results for any specific range, not just the preset options. (#58)
- **[Feature]** **Light mode for the Admin area** — A new theme switch lets you flip between the current dark look and a new light look, with your choice remembered next time you sign in. (#59)
- **[Feature]** **Working buttons on detail pages** — The Edit, Preview, and Pull Leads buttons on Placement, Modal, Offer, and Advertiser detail pages will actually do something when clicked instead of sitting there unresponsive. (#154)
- **[Bug]** **Missing Dashboard sections restored** — Familiar sections like campaign stats, top offers, and watch lists will return to the Dashboard, and the date-range picker will update them as expected. (#240)
- **[Feature]** **Sub-ID Stats moving to the Dashboard** — The Sub-ID Stats view is being relocated out of the placement form into the Dashboard reporting area, where it fits better. (#236)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will show results in 15-minute increments again, making it easier to spot and react to offer or partner issues quickly. (#243)
- **[Feature]** **New monitoring views and an activity log** — New "Offer with Legs" and CLP performance views (flagging offers converting under 30%) plus a searchable log of changes like pausing offers or cap adjustments will give you better visibility for troubleshooting. (#256)
- **[Feature]** **Consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for cleaner, more readable visuals. (#263)

## Offers

- **[Feature]** **Set all offer details at creation time** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting will be available right when you create an offer, so you no longer have to save first and then go back to add them. High priority. (#142)
- **[Feature]** **Campaigns module added** — The Campaigns area from the legacy system is coming to New Adsmith Frontend, letting you view, create, and edit campaigns and manage offer groups all in one place. Critical, high priority. (#200)
- **[Feature]** **Stricter checks before sending leads** — When a pre-ping runs before a data push, required fields will be checked first, so leads missing key information are stopped rather than passed along. (Pending confirmation that this is the desired behavior.) (#218)
- **[Feature]** **Easier advertiser and state targeting on the offer form** — You'll be able to type to search for an advertiser, and enter state targeting as a simple comma-separated list (e.g. CA, TX, FL) instead of only picking one at a time. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the offer's Delivery & Settings tab, you'll be able to add every offer in a group to the Conflicting Offers list at once, saving a lot of manual clicking. (#250)

## Flows

- **[Task]** **Polished, consistent Flow form** — The Flow form's appearance is being cleaned up so text boxes, color pickers, checkboxes, and paired fields look right and line up side-by-side, matching the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button** — A single button will add every available form field to a flow at once, instead of adding them one by one. (#224)
- **[Feature]** **Clearer "Step order" setting** — The step-order control on the flow form will get labels and help text so it's obvious what it controls and what each option means. (#226)
- **[Feature]** **Better TCPA consent checkbox** — On the published lander, the TCPA consent checkbox will be larger, rounded, and properly aligned with its text for a cleaner look. (#229)

## General / Across the App

- **[Feature]** **Protection against overwriting each other's work** — When two people open the same record, the app will warn that someone else is editing it and prevent accidental overwrites, keeping changes from being silently lost across offers, flows, placements, advertisers, and more. (#267)
- **[Feature]** **Brand guidelines as the foundation for AI output** — A comprehensive brand-guidelines document will become the main reference for AI-generated content, improving the quality and consistency of results. (#264)

## Link Testing

- **[Feature]** **Link Testing remembers where you came from** — Opening Link Testing from a placement will pre-select that placement automatically, so you don't have to pick it yourself each time. (#238)
- **[Bug]** **Clear errors for invalid links** — Testing an invalid link will show a proper error message in the Link Testing screen instead of unexpectedly sending you back to the Dashboard. (#239)

## Placements

- **[Feature]** **Easier offer ordering on placements** — Selected offers will default to manual order with drag-and-drop reordering, a clear X to remove an offer, and the ability to filter the offer list by taxonomy. (#235)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8a5ffa5558be3c2ea09af2a6c1cf14599c4f7d3a480af89a537b4cc4b0bd651a -->
