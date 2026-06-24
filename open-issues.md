# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 23:25:11 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will now open a proper start- and end-date picker, so you can view dashboard data for any time period you like instead of only the preset options. (#58)
- **[Feature]** **Light mode option for the Admin** — A new theme switch lets you toggle between the current dark look and a lighter one, with your choice remembered next time you sign in. Easier on the eyes in any lighting. (#59)
- **[Feature]** **Working Edit, Preview, and Pull Leads buttons** — Several detail pages (Placement, Modal, Offer, Advertiser) have buttons that currently do nothing when clicked. They'll be wired up so they take you where you expect. (#154)
- **[Feature]** **Sub-ID Stats moving to the Dashboard** — The Sub-ID Stats view will move out of the placement form and into the Dashboard reporting area, where it fits more naturally. (#236)
- **[Bug]** **Restore missing Dashboard sections** — Right now only the system overview loads. Campaign stats, top offers, and watch lists will return, and the date-range selector will update them. (#240)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer timespan chart will show data in 15-minute increments again, giving you the fine-grained view needed to spot offer or partner issues quickly. (#243)
- **[Feature]** **New monitoring views and an activity log** — Adds "Offer with Legs" and CLP performance views (flagging offers converting under 30%) plus a searchable record of changes like pausing offers or adjusting daily caps, so you can track and troubleshoot what happened and when. (#256)
- **[Feature]** **Consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for cleaner, more readable visuals. (#263)

## Offers

- **[Feature]** **Set all offer details when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting can be set right when you create an offer, instead of having to save it first and then go back to edit. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — When a pre-ping runs before a data push, the system will check required fields first and stop a lead that's missing them, rather than letting incomplete leads through. (Pending a decision to confirm this is the intended behavior.) (#218)
- **[Feature]** **Faster advertiser and state entry on the offer form** — Adds a type-to-search box for picking an advertiser and lets you paste or type a comma-separated list of states (e.g. CA, TX, FL) for targeting. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add all offers in a group to the Conflicting Offers list in one step, saving a lot of manual effort. (#250)

## Flows

- **[Task]** **Fix Flow form styling** — Cleans up the Flow form so textareas, color pickers, checkboxes, and paired fields display correctly and side-by-side, matching the polished look of the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, a single button will add every available field at once. (#224)
- **[Feature]** **Clearer "Step order" setting** — The step-order control will get labels and help text (or a redesign) so it's obvious what it controls and what the values mean. (#226)
- **[Feature]** **Better TCPA consent checkbox** — On the published lander, the TCPA checkbox will be larger, rounded, and properly aligned with its consent text for a cleaner look. (#229)

## Link Testing

- **[Feature]** **Pre-select the placement you came from** — Opening Link Testing from a placement will automatically choose that placement, so you don't have to find it in the list. (#238)
- **[Bug]** **Clear error for invalid links** — Testing a bad link will show a clear failure message in Link Testing instead of dumping you on the dashboard. (#239)

## Placements

- **[Feature]** **Easier offer ordering on placements** — The selected-offers list will default to Manual Order with drag-and-drop reordering, a clear X to remove an offer, and the ability to filter the offer list by taxonomy. (#235)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — The Campaigns area from the legacy admin will be added to New Adsmith Frontend, so you can view, create, edit, and configure campaigns and offer groups in one place. This is a high-priority gap. (#200)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit, others will see it's being edited and you'll be warned if it changed since you opened it, so one person's save can no longer silently wipe out another's changes. (#267)
- **[Feature]** **Brand guidelines to guide AI output** — A thorough, documented brand-guidelines reference will be used as the main input for AI-generated content, improving the quality and consistency of what it produces. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8a5ffa5558be3c2ea09af2a6c1cf14599c4f7d3a480af89a537b4cc4b0bd651a -->
