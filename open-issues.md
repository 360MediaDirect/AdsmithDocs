# Open Issues — Plain-Language Overview

_Last updated 2026-06-25 19:35:18 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard** — The "Custom" option in the date filter will finally open a real date picker, so you can choose your own start and end dates and see Dashboard data for exactly the period you care about. (#58)
- **[Task]** **Restore missing Dashboard sections** — Sections that aren't loading today — campaign stats, top offers, and watch lists — will be brought back, and the date range selector will properly update them. A high-priority fix. (#240)
- **[Bug]** **Edit and Preview buttons that actually work** — On the Placement, Modal, Offer, and Advertiser detail pages, the Edit, Preview, and Pull Leads buttons currently do nothing. They'll be wired up so clicking them takes you where you expect. (#154)
- **[Feature]** **New monitoring views and a full activity log** — Two new "Other Dashboard" views will help you watch long-running offers and flag CLP offers converting under 30%, plus a searchable history that records every change (pausing offers, cap changes, status updates) with who did it and when. (#256)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will show data in 15-minute increments again, making it much easier to spot errors and issues with offers or partner servers as they happen. (#243)
- **[Feature]** **Move Sub-ID Stats to the Dashboard** — Sub-ID Stats will move out of the placement form and into the Dashboard's reporting area, where this kind of reporting belongs. (#236)
- **[Feature]** **Dark/Light mode toggle** — You'll be able to switch the entire Admin between dark and light themes from your user menu, and your choice will stick between sessions — easier on the eyes in any environment. (#59)
- **[Task]** **Consistent Dashboard colors** — The Dashboard will adopt a defined, documented color palette applied consistently across views for cleaner, more readable screens. (#263)

## Offers

- **[Bug]** **Set all offer details when first creating an offer** — Today, piggyback offers, HD pixel placement IDs, and ZIP code targeting can only be added after an offer exists, forcing you to create then edit. This high-priority fix lets you fill them in during initial creation. (#142)
- **[Feature]** **Add a whole offer group to Conflicting Offers at once** — On the offer's Delivery & Settings tab, you'll be able to pick an offer group and add all of its offers to the Conflicting Offers list in one step, saving hours of manual work. (#250)
- **[Bug]** **Enforce required fields before pushing a lead** — When a pre-ping runs before a data push, missing required fields will block the lead right away instead of relying on the advertiser's endpoint to catch it — closing a gap that could let incomplete leads through. (Pending confirmation that this is the intended behavior.) (#218)

## Flows

- **[Task]** **Polished, consistent Flow form** — The Flow form has several visual problems today — plain white text boxes, unstyled color pickers and checkboxes, and paired fields stacking vertically instead of side by side. This cleanup brings it in line with the Placement and Modal forms. (#152)
- **[Feature]** **Clearer "Step order" setting** — The step-order control on the Flow form confuses users who can't tell what it does. We'll add labels and help text (or rework it) so its purpose and values are obvious. (#226)

## Placements

- **[Feature]** **Easier offer ordering on placements** — Selected offers will default to manual order with drag-and-drop reordering, a dedicated "X" to remove an offer (so clicking is reserved for dragging), and the ability to filter the offer list by taxonomy. (#235)

## General / Across the App

- **[Feature]** **Campaigns module** — The Campaigns module from the legacy admin is being rebuilt in New Adsmith Frontend so you can view, create, edit, and configure campaigns and offer groups — a core capability that's currently missing. A critical, high-priority addition. (#200)
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, the app will warn you if someone else changed it and show a "locked by" banner while another user is editing — so one person's save can no longer quietly wipe out another's work. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you back on the Dashboard with no explanation. It will instead show a clear failure message in the Link Testing screen. (#239)

## Behind the Scenes

- **[Task]** **Stronger brand guidelines for AI-generated output** — We'll establish one comprehensive brand-guidelines document and use it as the primary input for AI-assisted content, improving the consistency and quality of generated results. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 81c0bed32c04b090e96440de4175d8dd117b8c0e44c263fba23750cf656d0276 -->
