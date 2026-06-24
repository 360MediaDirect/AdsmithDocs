# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 16:43:32 UTC · 33 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard filter** — When you pick "Custom" in the Dashboard date filter, a proper date range picker will appear with start and end dates, so you can view data for any period you choose instead of just the preset options. (#58)
- **[Feature]** **Light mode for the Admin** — You'll be able to switch between the current dark theme and a new light theme, with your choice remembered next time you log in. Helpful for bright rooms or personal preference. (#59)
- **[Feature]** **Working Edit, Preview, and Pull Leads buttons on detail pages** — These buttons currently do nothing on the Placement, Modal, Offer, and Advertiser detail pages. They'll be wired up so clicking them takes you where you expect. (#154)
- **[Bug]** **Restore missing Dashboard sections** — Right now only the system overview loads. Campaign stats, top offers, and watch lists will be brought back, and the date range will properly update them. (#240)
- **[Feature]** **Move Sub-ID Stats to the Dashboard** — Sub-ID statistics will move out of the placement form and into the Dashboard reporting area, where they belong for monitoring. (#236)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer timespan chart will show data in 15-minute increments again, making it much easier to spot offer or partner-server issues quickly. (#243)
- **[Feature]** **New monitoring views and an activity log** — Adds "Offer with Legs" and "CLP Performance" views (highlighting offers converting under 30%) plus a searchable log that records changes like pausing offers or cap edits, with who made them and when. (#256)
- **[Feature]** **Show full advertiser and placement names** — Long advertiser and placement names will no longer be cut off with an ellipsis, so you can always read them in full. (#260)
- **[Feature]** **Remove the ID column to save space** — The ID/number column will be dropped from Dashboard tables to free up room for more useful information. (#261)
- **[Feature]** **Cleaner publisher and property names** — Publisher and property names will display only the part after the last colon (for example, "Foo: Bar: Acme Publishing" shows as "Acme Publishing") for easier reading. (#262)
- **[Feature]** **Standardized Dashboard colors** — A defined color palette will be applied consistently across the Dashboard to improve readability. (#263)

## Offers

- **[Feature]** **Set all offer fields when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting can be set right when you create an offer, instead of having to save it first and then edit it. High priority. (#142)
- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping runs before a data push, required fields will be checked first so incomplete leads are stopped instead of slipping through. (Pending a decision to confirm this is the wanted behavior.) (#218)
- **[Feature]** **Distinct status colors for offers** — Paused and Capped offers currently look the same. Paused will become red, Capped yellow/orange, and Active stays green, used consistently across offer lists and Dashboard indicators. (#246)
- **[Feature]** **Easier advertiser and state entry on the offer form** — You'll be able to type to search for an advertiser instead of scrolling, and enter state targeting as a typed or pasted comma-separated list (e.g. CA, TX, FL). (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in an offer group to the Conflicting Offers list in one step, saving significant time. (#250)
- **[Task]** **Offer row action links** — Each offer will get quick action links beneath its title (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an offer activity page showing lead and revenue performance over time. (#252)
- **[Bug]** **Fix HTML display and linkout in offer previews** — Fields like More Info Headline, More Info Content, and TCPA Content currently show raw code instead of formatted links and styling, and linkout offers don't work in preview. Both will be corrected. (#259)

## Flows

- **[Task]** **Fix the Flow form's styling and layout** — The Flow form has unstyled text boxes, color pickers, and checkboxes, and paired fields stack awkwardly. It will be cleaned up to match the polished look of the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field with a single click. (#224)
- **[Feature]** **Clearer "Step order" control** — The step-order setting is confusing today. It will get clear labels and help text (or a redesign) so you understand what it controls. (#226)
- **[Feature]** **Better TCPA consent checkbox** — On the published lander, the TCPA consent checkbox will be made larger, rounded, and properly aligned with its text. (#229)

## General / Across the App

- **[Feature]** **Bring back the Campaigns module** — Campaign management from the legacy admin isn't available yet in New Adsmith Frontend. It will be rebuilt so you can view, create, edit, and configure campaigns and offer groups as before. Critical, high priority. (#200)
- **[Feature]** **Link Testing remembers your placement** — When you open Link Testing from a placement, that placement will be pre-selected automatically instead of making you choose it. (#238)
- **[Bug]** **Clear error for invalid test links** — Testing an invalid link will show a clear failure message in Link Testing, rather than dumping you back on the Dashboard. (#239)
- **[Feature]** **Brand guidelines as the basis for AI output** — A comprehensive brand-guidelines document will become the primary input for AI-generated content, improving the quality and consistency of results. (#264)

## Placements

- **[Bug]** **Review the placement form's fields and links** — The create/edit form has unfamiliar new fields and is missing links like Preview and Details. The fields will be checked against the legacy version and the missing links restored. (#234)
- **[Feature]** **Reorderable offer assignment** — Selected offers will default to Manual Order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)
- **[Feature]** **Manual reordering on the offer transfer list** — The same improvements as above, captured from UAT: manual ordering, drag-and-drop, a remove button, and taxonomy filtering when assigning offers to a placement. (#255)

## Surveys

- **[Bug]** **Let visitors decline a CPA offer** — Visitors are currently forced to click "Yes" to continue, with no way to decline or move past a CPA offer. This trap will be fixed so visitors can decline and proceed. High priority. (#233)
- **[Bug]** **Stop duplicate offer firing on Yes/No/Yes** — Switching a survey offer from Yes to No and back to Yes can fire the offer twice, opening a second tab or submitting a duplicate lead. Each offer will fire only once per visit. High priority. (#266)

## Modals

- **[Bug]** **Let visitors close or decline a modal offer** — A single linkout/CPA offer in a modal can trap visitors because the Close button does nothing and there's no decline option. The Close button will work and visitors will be able to dismiss the offer. (#265)

## Properties

- **[Feature]** **Search box for the publisher selector** — On the property form, you'll be able to type to find a publisher instead of scrolling through the whole list. (#237)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: c70529953b1157da0415945098e365c0f79a226dba59aaaf2f20fa8c10257570 -->
