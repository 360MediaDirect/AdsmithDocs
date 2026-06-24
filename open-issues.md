# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 07:09:56 UTC · 47 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard filter** — The date filter offers a "Custom" choice, but nothing happens when you pick it. Once fixed, choosing "Custom" will open a start/end date picker so you can view Dashboard data for any range you like. (#58)
- **[Feature]** **Make the Edit, Preview, and Pull Leads buttons work** — On several detail pages (Placement, Modal, Offer, Advertiser) these buttons currently do nothing. They'll be wired up so clicking them takes you where you expect. (#154)
- **[Feature]** **Move Sub-ID Stats into the Dashboard** — Sub-ID performance stats will move out of the Placement form and into the Dashboard reporting area, where this kind of information belongs. (#236)
- **[Bug]** **Restore missing Dashboard sections** — Right now only the system overview loads. The campaign stats, top offers, and watch list sections will be brought back, and the date-range selector will update them. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds views for monitoring long-running offers and low-converting CLP offers, plus a searchable log that records every change (pausing offers, cap changes, status updates) for easy auditing. (#256)
- **[Feature]** **Show full advertiser and placement names** — Long names will no longer be cut off with "…" so you can read them in full. (#260)
- **[Feature]** **Remove the ID/number column** — Dropping this column frees up screen space for the information you actually use. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon (e.g. "Foo: Bar: Acme Publishing" shows as "Acme Publishing") for easier reading. (#262)
- **[Feature]** **A consistent Dashboard color scheme** — A defined set of colors will be applied across the Dashboard for better visual clarity and readability. (#263)

## Offers

- **[Feature]** **Set all Offer fields during creation** — Piggyback offers, HD pixel placement IDs, and ZIP-code targeting can currently only be added after an offer is created. You'll be able to set them right away when creating a new offer. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — When a pre-ping runs before pushing data, missing required fields aren't blocked today. The change will stop a lead with missing required information before it's sent, instead of relying on the partner to catch it. (#218)
- **[Bug]** **Advertiser info missing on the Offers report** — Some offers still don't show their advertiser. This fixes the underlying data so every offer displays its advertiser correctly. (#242)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail chart will show activity in 15-minute increments again, so you can spot errors and partner-server issues quickly. (#243)
- **[Feature]** **Clearer offer status colors** — Paused and Capped currently look the same. Paused will be red, Capped yellow/orange, and Active green—everywhere these indicators appear. (#246)
- **[Feature]** **Easier advertiser and state entry on the Offer form** — Adds type-to-search for picking an advertiser and lets you type or paste a comma-separated list of states (e.g. CA, TX, FL) for targeting. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in an offer group to the Conflicting Offers list in one step. (#250)
- **[Task]** **Quick action links under each offer** — Adds the familiar row actions (Edit, Quick Edit, Trash, View, Preview, Trends, Details) beneath each offer title, with Trends opening an offer performance page. (#252)
- **[Bug]** **Offer preview shows raw code and broken link-outs** — Formatted fields (More Info Headline, More Info Content, TCPA Content) show raw HTML instead of styled text and links, and Linkout offers don't redirect from the preview. Both will display and work correctly. (#259)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or stacked awkwardly (plain textareas, unstyled color pickers and checkboxes, fields that should sit side by side). It will be tidied up to match the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field with a single click. (#224)
- **[Feature]** **Clearer "step order" setting** — The step-order control is confusing today. It will get labels and help text (or a redesign) so it's clear what it controls. (#226)
- **[Feature]** **Start flows directly on the form** — The extra "Claim your offers" intro page will be removed so visitors land straight on the form fields. (#228)
- **[Feature]** **Better TCPA consent checkbox** — On the published lander, the consent checkbox will be larger, rounded, and properly aligned with its text. (#229)
- **[Feature]** **Footer with copyright and site name** — The lander footer will include the copyright line and site name (pulled from General Information). (#232)
- **[Bug]** **Visitors stuck on CPA offers** — On CPA offers, visitors are forced to click "Yes" with no way to decline or move on, trapping them mid-flow. This will be fixed so they can proceed or opt out. (#233)

## Placements

- **[Bug]** **Unfamiliar fields and missing links on the Placement form** — The create/edit form shows unexpected new fields and is missing links like Preview and Details. The form will be reviewed against the legacy version and the missing links restored. (#234)
- **[Feature]** **Reorder assigned offers by drag-and-drop** — Selected offers will default to manual order and let you drag to reorder, with an "X" to remove each one and the ability to filter the offer list by taxonomy. (#235)
- **[Feature]** **Manual ordering for offer assignment (UAT follow-up)** — Confirms the same improvement: manual ordering, drag-and-drop, an "X" to remove offers, and taxonomy filtering on the placement offer transfer list. (#255)

## Link Testing

- **[Feature]** **Pre-select the placement you came from** — When you open Link Testing from a specific placement, that placement will already be selected instead of asking you to choose. (#238)
- **[Bug]** **Show an error for invalid links** — Testing a bad link currently dumps you on the Dashboard. Instead, you'll see a clear failure message right in Link Testing. (#239)

## Properties

- **[Feature]** **Search box for the publisher selector** — Adds type-to-search to the publisher dropdown on the Property form so you don't have to scroll to find one. (#237)

## General / Across the App

- **[Feature]** **Light and Dark mode toggle** — The Admin is dark-only today. You'll be able to switch between light and dark themes, with your choice remembered between visits. (#59)
- **[Task]** **Users management review** — A side-by-side look at the legacy and new Users areas to identify what's missing (such as bulk actions, last-login and password fields) and prioritize bringing it over. (#80)
- **[Feature]** **Bring back the Campaigns module** — The Campaigns area from the legacy admin isn't in the new product yet. It will be added so you can view, create, edit, and configure campaigns and offer groups as before. (#200)

## Behind the Scenes

- **[Task]** **Review an old stats job** — Checking whether a legacy stats process is still needed or can be retired, with no change to what you see. (#33)
- **[Task]** **Today's live stats** — Groundwork so the Dashboard's "today" view reflects up-to-the-hour impressions, clicks, leads, and revenue in Eastern Time. (#34)
- **[Task]** **Roll up historical stats** — A scheduled process to summarize live stats into daily totals for faster historical reporting. (#35)
- **[Task]** **Safe pre-ping testing** — Running the new pre-ping process alongside the old one to confirm results match before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each active advertiser's pre-ping works correctly ahead of the switch. (#41)
- **[Task]** **Faster surveys** — Adding a caching layer so survey configurations and offer data load more quickly. High priority. (#42)
- **[Task]** **Run new scheduled jobs in parallel** — Operating the new background jobs alongside the old ones to confirm they behave identically before relying on them. (#43)
- **[Task]** **Retire old scheduled jobs — group 3** — Switching off the first set of legacy background jobs after the replacements prove stable. (#44)
- **[Task]** **Retire old scheduled jobs — group 2** — Switching off the next set of legacy stats jobs once group 3 is stable. (#45)
- **[Task]** **Retire old scheduled jobs — group 1 (critical)** — Switching off the most critical legacy jobs last, with close monitoring and quick rollback ready. (#46)
- **[Task]** **Rollback plans** — Documenting and testing how to revert each system quickly if a problem arises. (#48)
- **[Task]** **Troubleshooting guides** — Creating step-by-step guides for resolving common operational issues. (#49)
- **[Feature]** **Brand guidelines for AI output** — Establishing a thorough brand-guidelines document to use as the main input for AI-generated content, improving quality and consistency. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 687487fb5892cb0959b36f8b6c4eb3ec174c16bbb22d3dcbdd9d3df606803281 -->
