# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 22:28:45 UTC · 27 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter currently does nothing. Once fixed, picking "Custom" will open a start- and end-date picker so you can view dashboard data for any specific period. (#58)
- **[Bug]** **Restore the missing dashboard sections** — Right now only the system overview loads. This high-priority fix brings back campaign stats, top offers, and watch lists, and makes them respond to the date range you choose. (#240)
- **[Feature]** **Make the Edit, Preview, and Pull Leads buttons work** — On several detail pages these buttons appear but don't respond when clicked. They'll be wired up so they actually open the editor, show a preview, or pull leads. (#154)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer timespan chart will show activity in 15-minute increments again, helping you spot offer or partner-server issues quickly. (#243)
- **[Feature]** **New monitoring views and an activity log** — Adds "Offer with Legs" and CLP performance views (flagging low-converting offers), plus a searchable record of changes like pausing an offer or adjusting daily caps. (#256)
- **[Feature]** **Move Sub-ID Stats to the Dashboard** — Sub-ID Stats will move out of the placement form and into the dashboard reporting area where they're easier to find. (#236)
- **[Feature]** **Show full advertiser and placement names** — Long names will no longer be cut off with an ellipsis, so you can read them in full. (#260)
- **[Feature]** **Remove the ID/number column** — Dropping this column frees up screen space for the information you actually use. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon (for example, "Foo: Bar: Acme Publishing" shows as "Acme Publishing"). (#262)
- **[Feature]** **A consistent dashboard color scheme** — A defined palette will be applied across the dashboard for better, more consistent readability. (#263)

## Offers

- **[Feature]** **Set all offer details when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP-code targeting can currently only be added after saving. This high-priority change lets you set them right when you first create the offer. (#142)
- **[Feature]** **Advertiser search and typed state targeting** — Adds a type-to-search box to the Advertiser selector and lets you type or paste a comma-separated list of states (e.g. CA, TX, FL) for targeting. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in a group to the Conflicting Offers list in one step, saving considerable time. (#250)
- **[Feature]** **Distinct status colors** — Paused and Capped currently look the same. Paused will become red, Capped yellow/orange, and Active green, applied consistently across offers and the dashboard. (#246)
- **[Feature]** **Enforce required pre-ping fields before pushing** — When a pre-ping runs before a data push, missing required fields will block the lead instead of being passed along. (Awaiting a decision before this is built.) (#218)

## Flows

- **[Task]** **Fix the Flow form styling** — Several parts of the Flow form currently look unstyled or stack awkwardly. This cleans up text boxes, color pickers, checkboxes, and side-by-side fields to match the rest of the app. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field in a single click. (#224)
- **[Feature]** **Clearer "Step order" setting** — The step-order control will get labels and help text so it's obvious what it controls and what the values mean. (#226)
- **[Feature]** **Better TCPA consent checkbox** — On the published lander, the TCPA checkbox will be larger, rounded, and properly aligned with its consent text. (#229)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other** — When you open a record to edit, others will see it's locked and won't be able to save over your changes; you'll also be warned if a record changed while you had it open. Works across all entity screens. (#267)
- **[Feature]** **Dark and Light mode toggle** — The Admin currently only offers dark mode. A toggle will let you switch to a light theme, with your choice remembered between sessions. (#59)
- **[Feature]** **Brand guidelines as the basis for AI output** — A comprehensive brand-guidelines document will be used as the main input for AI-generated content, improving the quality and consistency of results. (#264)

## Link Testing

- **[Bug]** **Show an error for invalid links** — Testing an invalid link currently dumps you back on the dashboard. Instead, you'll see a clear failure message in the Link Testing screen. (#239)
- **[Feature]** **Default to the placement you started from** — When you open Link Testing from a placement, that placement will be pre-selected so you don't have to pick it manually. (#238)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — This core feature from the legacy admin is missing in New Adsmith Frontend. It will be added so you can view, create, edit, and configure campaigns and their offer groups. High priority. (#200)

## Placements

- **[Feature]** **Better control over selected offers** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove each one, and the ability to filter the offer list by taxonomy. (#235)

## Properties

- **[Feature]** **Search box for the Publisher selector** — Adds type-to-search to the publisher dropdown on the property form, so you no longer have to scroll to find one. (#237)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f244b4acd5b088f4278b2406294799cfd49054c53b2cfebc502b1942f7f06662 -->
