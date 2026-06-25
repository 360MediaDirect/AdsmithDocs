# Open Issues — Plain-Language Overview

_Last updated 2026-06-25 11:55:10 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a proper start- and end-date picker, so you can view dashboard data for any range you choose instead of only the preset options like Today or This Month. (#58)
- **[Bug]** **Restore missing Dashboard sections** — The campaign stats, top offers, and watch lists sections will be back on the Dashboard, and the date-range selector will update them as expected, rather than only showing the system overview. (#240)
- **[Feature]** **Buttons on detail pages will actually work** — Edit, Preview, and Pull Leads buttons on Placement, Modal, Offer, and Advertiser detail pages will respond when clicked instead of doing nothing. (#154)
- **[Feature]** **Dark and Light mode toggle** — You'll be able to switch the Admin between dark and light themes from your account menu, and your choice will be remembered next time you log in. (#59)
- **[Feature]** **Sub-ID Stats moving to the Dashboard** — The Sub-ID Stats view will move out of the placement form and into the Dashboard's reporting area, where it's easier to find and review. (#236)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer timespan chart will show activity in 15-minute increments again, making it easier to spot errors and monitor offer and partner performance in near real time. (#243)
- **[Feature]** **New monitoring views and an activity log** — A new "Other Dashboard" area will add views for long-running offers and low-converting CLP offers, plus a searchable log that records changes like pausing an offer or adjusting daily caps, with who made them and when. (#256)
- **[Feature]** **Consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for cleaner, more readable visuals. (#263)

## Offers
- **[Feature]** **Set all offer details when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting will be available right when you create an offer, so you no longer have to save it first and then edit it to add these. (#142)
- **[Feature]** **Search and faster state targeting on the offer form** — The Advertiser selector will get a type-to-search box, and state targeting will accept a typed or pasted comma-separated list (like CA, TX, FL) in addition to picking states manually. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in an offer group to the Conflicting Offers list in one step, saving a lot of manual effort. (#250)
- **[Feature]** **Enforce required pre-ping fields before sending** — When a pre-ping runs before a data push, missing required fields will stop the lead right away instead of being passed along, helping keep incomplete or malformed leads from slipping through. (#218)

## Flows
- **[Task]** **Fix unstyled areas of the Flow form** — Textareas, color pickers, checkboxes, and paired fields on the Flow form will look polished and lay out side-by-side like the Placement and Modal forms, instead of appearing plain or stacked. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — When building a flow, you'll be able to add every available form field at once instead of adding them one at a time. (#224)
- **[Feature]** **Clearer "Step order" setting** — The step-order control on the flow form will get labels and help text so it's obvious what it controls and what the values mean. (#226)
- **[Feature]** **Better-looking TCPA consent checkbox** — On the published lander, the TCPA consent checkbox will be larger, rounded, and properly aligned with its text. (#229)

## Link Testing
- **[Feature]** **Link Testing remembers where you opened it** — When you start Link Testing from a placement, that placement will already be selected, so you don't have to pick it each time. (#238)
- **[Bug]** **Clear errors for invalid links** — Testing a bad link will show a clear failure message in Link Testing instead of unexpectedly sending you to the Dashboard. (#239)

## General / Across the App
- **[Feature]** **Campaigns module coming to the new platform** — The Campaigns area from the legacy admin will be rebuilt here, letting you view, create, edit, and configure campaigns and manage offer groups, all in one place. This is a high-priority, core feature. (#200)
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, one will see a "locked by" notice, and saving over someone else's recent change will be blocked with a prompt to reload, preventing lost updates. (#267)
- **[Feature]** **Stronger brand guidelines for AI-generated content** — A comprehensive brand-guidelines document will become the primary reference for AI-generated output, improving consistency and quality. (#264)

## Placements
- **[Feature]** **Easier offer ordering on placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer (so clicking is reserved for dragging), and the ability to filter the offer list by taxonomy. (#235)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8a5ffa5558be3c2ea09af2a6c1cf14599c4f7d3a480af89a537b4cc4b0bd651a -->
