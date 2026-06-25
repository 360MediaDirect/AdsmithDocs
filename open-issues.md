# Open Issues — Plain-Language Overview

_Last updated 2026-06-25 15:56:24 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will finally open a start- and end-date picker so you can view dashboard data for any specific range, with the chosen dates shown right on the filter button. (#58)
- **[Feature]** **Make Edit, Preview, and Pull Leads buttons work** — On the Placement, Modal, Offer, and Advertiser detail pages these buttons currently do nothing when clicked. They'll be wired up so they take you where you expect instead of leaving you stuck. (#154)
- **[Feature]** **Sub-ID Stats move to the Dashboard** — Sub-ID Stats will be relocated out of the placement form and into the Dashboard reporting area, where this kind of information belongs. (#236)
- **[Bug]** **Bring back missing Dashboard sections** — Right now only the system overview loads. We're restoring the campaign stats, top offers, and watch list sections, and making the date range update them. A high-priority fix. (#240)
- **[Feature]** **New "Other Dashboard" monitoring views and an activity log** — Adds an "Offer with Legs" view and a CLP offers performance view that highlights offers converting under 30%, plus a searchable log that records changes like pausing an offer or adjusting daily caps, so you can spot issues and trace what changed. (#256)
- **[Feature]** **Consistent Dashboard color scheme** — A defined color palette will be applied across the Dashboard to make it easier to read at a glance. (#263)

## General / Across the App

- **[Feature]** **Campaigns module** — The Campaigns area from the legacy admin isn't in New Adsmith Frontend yet. This high-priority work adds it back so you can view, create, edit, and configure campaigns and offer groups as before. (#200)
- **[Feature]** **Protection against two people overwriting each other's edits** — When you open a record someone else is already editing, you'll see a clear "locked by" notice, and if a record changes while you have it open, you'll be prompted to reload instead of silently wiping out the other person's work. Applies to offers, flows, placements, advertisers, and more. (#267)
- **[Feature]** **Dark and Light mode toggle** — You'll be able to switch the admin between dark and light themes from your user menu, with your choice remembered between sessions and applied instantly. (#59)
- **[Feature]** **Clearer, on-brand AI output** — A comprehensive brand-guidelines document will be used as the main reference for AI-generated content, leading to more consistent, on-brand results. (#264)

## Flows

- **[Task]** **Fix the look of the Flow form** — Several parts of the Flow form currently appear unstyled or stacked awkwardly. This tidies up textareas, color pickers, checkboxes, and paired fields so the form looks clean and matches the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field in a single click. (#224)
- **[Feature]** **Make the "Step order" setting understandable** — Clearer labels and help text will explain what step order controls and what its values mean, so it's no longer a guessing game. (#226)
- **[Feature]** **Better TCPA consent checkbox styling** — On the published lander, the consent checkbox will be larger, rounded, and properly aligned with its text. (#229)

## Offers

- **[Feature]** **Set all offer details during creation** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting can currently only be added after an offer exists. You'll be able to set them right when you first create the offer. A high-priority improvement. (#142)
- **[Feature]** **Enforce required fields before a pre-ping pushes** — When a pre-ping runs before a data push, missing required fields will stop the lead up front rather than letting incomplete data slip through. (Pending confirmation that this is the desired behavior.) (#218)
- **[Feature]** **Easier advertiser and state entry on the offer form** — Adds a type-to-search box for picking an advertiser and lets you type or paste a comma-separated list of states (e.g. CA, TX, FL) for targeting. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers at once** — On the Delivery & Settings tab, you'll be able to add every offer in an offer group to the Conflicting Offers list in one step, saving a lot of manual work. (#250)

## Link Testing

- **[Feature]** **Default to the placement you opened it from** — When you open Link Testing from a placement, that placement will already be selected so you don't have to pick it each time. (#238)
- **[Bug]** **Show an error for invalid links** — Testing an invalid link currently dumps you on the dashboard. Instead you'll get a clear failure message right in Link Testing. (#239)

## Reports

- **[Feature]** **15-minute detail on the offer timespan chart** — The offer detail timespan stats will show data in 15-minute increments again, so you can closely monitor offers and partner servers and catch issues quickly. (#243)

## Placements

- **[Feature]** **Better control over selected offers** — The offer selection list will default to manual order, let you drag and drop to reorder, give each selected offer an X to remove it (so clicking is reserved for dragging), and let you filter the offer list by taxonomy. (#235)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8a5ffa5558be3c2ea09af2a6c1cf14599c4f7d3a480af89a537b4cc4b0bd651a -->
