# Open Issues — Plain-Language Overview

_Last updated 2026-06-25 17:54:35 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Picking "Custom" in the date filter will open a proper start- and end-date picker so you can view dashboard data for any period you choose, with the selected range shown right on the filter button. (#58)
- **[Feature]** **Dark and Light mode toggle** — You'll be able to switch the Admin between the current dark theme and a new light theme, with your choice remembered next time you sign in — easier on the eyes in any lighting. (#59)
- **[Bug]** **Edit, Preview, and Pull Leads buttons that do nothing** — On the Placement, Modal, Offer, and Advertiser detail pages, these buttons currently don't respond when clicked. This fix wires them up so they take you where you expect. (#154)
- **[Feature]** **Sub-ID Stats moving to the Dashboard** — Sub-ID Stats will move out of the placement form and into the Dashboard's reporting area, where this kind of information belongs. (#236)
- **[Task]** **Restore missing Dashboard sections** — The Dashboard will once again show campaign stats, top offers, and watch lists (today only the system overview loads), and the date-range selector will update them. High priority. (#240)
- **[Feature]** **New "Other Dashboard" monitoring views and an activity log** — Adds views to track long-running ("offers with legs") and under-performing CLP offers, plus a searchable log that records changes like pausing an offer or adjusting daily caps — making it easy to spot issues and see who changed what. (#256)
- **[Task]** **Consistent Dashboard color scheme** — A defined set of colors will be applied across Dashboard views for better, more consistent readability. (#263)

## Offers

- **[Bug]** **Set all offer fields when first creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting can currently only be added after an offer exists. This fix lets you set them right away during creation, saving an extra editing step. High priority. (#142)
- **[Bug]** **Enforce required fields on pre-pings before data is pushed** — When a pre-ping runs before a data push, required fields aren't currently checked on our side, so incomplete leads can slip through. This will block a lead that's missing required information. (Pending a decision to confirm the change.) (#218)
- **[Feature]** **Add a whole offer group to Conflicting Offers at once** — On the offer's Delivery & Settings tab, you'll be able to add every offer in a group to the Conflicting Offers list in one action instead of adding them one by one. (#250)

## General / Across the App

- **[Feature]** **Protection against two people overwriting the same record** — When you open a record to edit, others will see it's being edited by you, and if a record changed since you opened it you'll be prompted to reload — preventing accidental overwrites of each other's work. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you on the dashboard with no explanation. Instead, you'll see a clear failure message in Link Testing. (#239)
- **[Task]** **Comprehensive brand guidelines for AI output** — A single, thorough brand-guidelines document will be created and used as the main input for AI-generated content, improving the quality and consistency of results. (#264)

## Flows

- **[Task]** **Fix the Flow form's appearance** — The Flow form has several styling problems — plain-looking text boxes, unstyled color pickers and checkboxes, and paired fields stacking vertically. This brings it in line with the polished look of the Placement and Modal forms. (#152)
- **[Feature]** **Clearer "Step order" setting** — The step-order control on the Flow form isn't easy to understand today. Adding labels and help text (or reworking the control) will make it clear what it orders and what the values mean. (#226)

## Placements

- **[Feature]** **Better control over the offer list on placements** — Selected offers will default to manual order with drag-and-drop reordering, a clear "X" to remove an offer (so clicking is reserved for dragging), and the ability to filter the offer list by taxonomy. (#235)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — The new platform is missing the Campaigns area from the legacy system. This adds it back so you can view, create, edit, and configure campaigns and their offer groups. Critical, high priority. (#200)

## Reports

- **[Feature]** **15-minute detail on the offer timespan chart** — The offer detail timespan stats will show data in 15-minute increments again, giving you the fine-grained view needed to catch issues with offers or partner servers quickly. (#243)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 81c0bed32c04b090e96440de4175d8dd117b8c0e44c263fba23750cf656d0276 -->
