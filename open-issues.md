# Open Issues — Plain-Language Overview

_Last updated 2026-06-25 01:41:26 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will finally open a start/end date picker so you can view dashboard data for any range you like, with the chosen dates shown right on the filter button. (#58)
- **[Bug]** **Missing dashboard sections restored** — Campaign stats, top offers, and watch lists will reappear on the Dashboard, and changing the date range will update them. Right now only the system overview loads. This is a high-priority fix. (#240)
- **[Feature]** **Dark and light mode** — You'll be able to switch the Admin between dark and light themes from your user menu, and your choice will be remembered next time you sign in. (#59)
- **[Feature]** **Working Edit, Preview, and Pull Leads buttons** — On the Placement, Modal, Offer, and Advertiser detail pages, these buttons currently do nothing when clicked. They'll be wired up so they take you where you expect. (#154)
- **[Feature]** **Sub-ID Stats moved to the Dashboard** — Sub-ID Stats will move out of the placement form and into the Dashboard reporting area, where this kind of information belongs. (#236)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer timespan chart will show activity in 15-minute increments again, making it much easier to spot errors and issues with offers or partner servers as they happen. (#243)
- **[Feature]** **New monitoring views and an activity log** — A new "Other Dashboard" area will add views for long-running offers and low-converting CLP offers (flagging those under 30%), plus a searchable log that records every change—like pausing an offer or adjusting daily caps—with a timestamp and who made it. (#256)
- **[Feature]** **Consistent dashboard colors** — The Dashboard will adopt a defined color palette to make it cleaner and easier to read at a glance. (#263)

## Offers
- **[Feature]** **Set all offer details at creation time** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting will be available when you first create an offer, so you no longer have to save it and then go back in to edit. A high-priority improvement. (#142)
- **[Feature]** **Stricter pre-ping checks before pushing leads** — When a pre-ping runs before a data push, required fields will be enforced up front, so leads missing required information are stopped rather than passed through. (Pending a final go-ahead on the change.) (#218)
- **[Feature]** **Easier advertiser and state entry on the offer form** — The Advertiser field will gain a type-to-search box, and state targeting will accept a typed or pasted comma-separated list (like CA, TX, FL) in addition to picking from the list. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in an offer group to the Conflicting Offers list in one step, saving a lot of repetitive clicking. (#250)

## Flows
- **[Task]** **Cleaner, properly styled Flow form** — The Flow form's text boxes, color pickers, checkboxes, and section layouts will be tidied up so paired fields sit side by side and everything matches the look of the other forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field at once with a single click. (#224)
- **[Feature]** **Clearer "Step order" setting** — The step-order control will get labels and help text so it's obvious what it controls and what the choices mean. (#226)
- **[Feature]** **Better TCPA consent checkbox** — On the published lander, the TCPA checkbox will be larger, rounded, and properly aligned with its consent text. (#229)

## Link Testing
- **[Feature]** **Link Testing remembers where you started** — When you open Link Testing from a specific placement, that placement will be pre-selected for you instead of making you pick it again. (#238)
- **[Bug]** **Clear error for invalid links** — Testing an invalid link will show a clear failure message in Link Testing rather than dropping you onto the dashboard. (#239)

## Campaigns
- **[Feature]** **Campaigns module added** — The Campaigns area from the previous admin will be rebuilt here, letting you view, create, edit, and configure campaigns and their offer groups. This is a critical, high-priority gap. (#200)

## Placements
- **[Feature]** **Smarter offer selection on placements** — Selected offers will default to manual order, support drag-and-drop reordering, include an "X" to remove an offer (so clicking is reserved for dragging), and let you filter the offer list by taxonomy. (#235)

## General / Across the App
- **[Feature]** **Protection against overwriting each other's edits** — If two people open the same record, the app will warn that someone else is editing it and prevent one person's save from silently wiping out the other's changes, across all the main forms. (#267)
- **[Feature]** **Brand guidelines drive AI output** — A comprehensive brand-guidelines document will become the primary reference for AI-generated content, improving the quality and consistency of the results. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8a5ffa5558be3c2ea09af2a6c1cf14599c4f7d3a480af89a537b4cc4b0bd651a -->
