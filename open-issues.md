# Open Issues — Plain-Language Overview

_Last updated 2026-06-25 13:42:47 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard** — Picking "Custom" in the Dashboard's date filter will finally open a start- and end-date picker, so you can view results for any range you choose instead of only the preset options. (#58)
- **[Bug]** **Missing Dashboard sections will return** — Right now only the system overview loads. This restores the campaign stats, top offers, and watch-list sections, and makes them update when you change the date range. A high-priority fix. (#240)
- **[Feature]** **Working Edit and Preview buttons on detail pages** — The Edit, Preview, and Pull Leads buttons on Placement, Modal, Offer, and Advertiser detail pages currently do nothing when clicked. They'll be wired up so each one takes you where you expect. (#154)
- **[Feature]** **Dark/Light mode for the Admin area** — You'll be able to switch between the current dark theme and a new light theme to suit your environment, and your choice will be remembered next time you log in. (#59)
- **[Feature]** **Sub-ID Stats moving to the Dashboard** — The Sub-ID Stats section will move out of the placement form and into the Dashboard reporting area, where it's easier to find and review. (#236)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer timespan chart will show activity in 15-minute increments again, giving you the fine-grained view needed to spot offer or partner issues quickly. (#243)
- **[Feature]** **New monitoring views and an activity log** — Adds "Offer with Legs" and "CLP Performance" views (flagging offers converting under 30%) plus a searchable record of key actions like pausing offers and changing daily caps, so changes are easy to trace. (#256)
- **[Feature]** **Consistent Dashboard color scheme** — A defined set of brand colors will be applied across the Dashboard for clearer, more readable visuals. (#263)

## Offers

- **[Feature]** **Set all offer details when first creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting can currently only be added after saving. You'll be able to set them right away during creation, saving a round trip. A high-priority feature. (#142)
- **[Feature]** **Easier advertiser search and state targeting on the offer form** — Adds a type-to-search box for choosing an advertiser and lets you type or paste a comma-separated list of states (e.g. CA, TX, FL) instead of selecting them one by one. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers at once** — On the Delivery & Settings tab, you'll be able to add every offer in an offer group to the Conflicting Offers list in a single step, saving considerable time. (#250)
- **[Feature]** **Stricter checks on pre-ping required fields** — When a pre-ping runs before a data push, missing required fields will stop the lead before it's sent, rather than relying on the advertiser's response. (Confirmation needed before this change is made.) (#218)

## Flows

- **[Task]** **Polished, consistent Flow form styling** — The Flow form will get the same clean look as the Placement and Modal forms: properly styled text boxes, color pickers, and checkboxes, with paired fields sitting side by side instead of stacked. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field with a single click. (#224)
- **[Feature]** **Clearer "Step order" setting** — The step-order control will get labels and help text (or a redesign) so it's obvious what it controls and what each value means. (#226)
- **[Feature]** **Better-looking TCPA consent checkbox** — On the published lander, the TCPA checkbox will be larger, rounded, and properly aligned with its consent text. (#229)

## General / Across the App

- **[Feature]** **Campaigns module coming to the new platform** — The Campaigns feature from the legacy admin isn't available yet. It will be rebuilt so you can view, create, edit, and configure campaigns and offer groups just as before. A critical, high-priority addition. (#200)
- **[Feature]** **Protection against two people overwriting each other** — When you open a record to edit, it will be locked so a second person sees a "Locked by…" notice, and if a record changes while you have it open you'll be prompted to reload — preventing accidental loss of someone's work. (#267)
- **[Feature]** **Clear brand guidelines to improve AI-generated content** — The team will create a single, comprehensive brand-guidelines document and use it as the main reference for AI output, improving consistency and quality. (#264)

## Link Testing

- **[Bug]** **Clear error for invalid links** — Testing an invalid link will now show a proper failure message in Link Testing instead of dropping you back on the dashboard. (#239)
- **[Feature]** **Link Testing remembers where you opened it** — When you start Link Testing from a specific placement, that placement will be pre-selected for you, so you don't have to pick it manually. (#238)

## Placements

- **[Feature]** **Easier reordering of selected offers** — The offer list will default to Manual Order, let you drag and drop to reorder, add an X to remove an offer (so a click is only for dragging), and let you filter offers by taxonomy. (#235)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8a5ffa5558be3c2ea09af2a6c1cf14599c4f7d3a480af89a537b4cc4b0bd651a -->
