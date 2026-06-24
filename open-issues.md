# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 00:30:50 UTC · 47 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a proper start/end date picker so you can view dashboard data for any range you like, with the chosen dates shown right on the filter button. (#58)
- **[Feature]** **Light mode option for the Admin UI** — You'll be able to switch between the current dark theme and a new light theme, with your choice remembered next time you log in. (#59)
- **[Feature]** **Make Edit, Preview, and Pull Leads buttons work on detail pages** — Buttons on the Placement, Modal, Offer, and Advertiser detail pages that currently do nothing will take you to the right screen when clicked. (#154)
- **[Feature]** **Move Sub-ID Stats to the Dashboard** — Sub-ID statistics will move out of the placement form into the Dashboard reporting area, where they're easier to find and monitor. (#236)
- **[Bug]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will be brought back so the Dashboard shows full reporting again and updates when you change the date range. (#240)
- **[Feature]** **New monitoring views and an activity log** — Adds "Offer with Legs" and CLP performance views (highlighting offers converting under 30%) plus a searchable record of every change, such as pausing an offer or adjusting a daily cap. (#256)
- **[Feature]** **Show full advertiser and placement names** — Names will no longer be cut off with an ellipsis, so you can read them in full across Dashboard views. (#260)
- **[Feature]** **Remove the ID/number column** — Dropping the ID column from Dashboard tables frees up screen space for the information you actually use. (#261)
- **[Feature]** **Cleaner publisher and property names** — Publisher and property names will display only the part after the last colon (e.g. "Foo: Bar: Acme Publishing" shows as "Acme Publishing"). (#262)
- **[Feature]** **Standardized Dashboard colors** — A defined color palette will be applied consistently across the Dashboard for better readability. (#263)

## Offers

- **[Feature]** **Set more fields when first creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting will be available on the create screen, so you no longer have to save an offer first and then edit it to add them. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — When a lead is missing a field marked required, the pre-ping will stop it immediately instead of passing it along, helping keep incomplete leads from slipping through. (Decision needed before this is built.) (#218)
- **[Bug]** **Show advertiser info on the Offers report** — A data issue leaving the Advertiser column blank for some offers will be resolved so advertiser details appear for every offer. (#242)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will return to 15-minute increments, making it easier to spot errors and partner-server issues quickly. (#243)
- **[Feature]** **Clearer offer status colors** — Paused will be red, Active green, and Capped yellow/orange, so Paused and Capped are no longer confused for one another in the offer list and Dashboard. (#246)
- **[Feature]** **Easier offer form entry** — Adds a type-to-search box to the Advertiser selector and lets you type or paste a comma-separated list of states (e.g. CA, TX, FL) for targeting. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab you'll be able to add every offer in a group to the Conflicting Offers list in one step, saving significant time. (#250)
- **[Task]** **Quick action links under each offer** — Adds legacy-style links (Edit, Quick Edit, Trash, View, Preview, Trends, Details) beneath offer titles, with Trends opening an offer activity page showing lead and revenue trends. (#252)
- **[Bug]** **Fix HTML display and Linkout in offer previews** — Headline, more-info, and TCPA fields will show formatted links and styling instead of raw code, and Linkout offers will work correctly from the preview. (#259)

## Flows

- **[Task]** **Fix Flow form styling** — The Flow form will get proper styling so text areas, color pickers, checkboxes, and paired fields display correctly side-by-side, matching the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field with a single click. (#224)
- **[Feature]** **Explain the "Step order" setting** — Clearer labels and help text will make it obvious what the step-order control does and what its values mean. (#226)
- **[Feature]** **Drop the extra "Claim your offers" page** — New flows will start visitors directly on the form fields instead of an introductory button page. (#228)
- **[Feature]** **Improved TCPA consent checkbox** — The consent checkbox on the lander will be larger, rounded, and properly aligned with its text. (#229)
- **[Feature]** **Add a footer to the lander** — The lander footer will include the copyright line and site name pulled from General Information. (#232)
- **[Bug]** **Let visitors decline CPA offers** — Visitors will be able to move past or decline a CPA offer instead of being forced to click "yes," preventing them from getting stuck mid-flow. (#233)

## General / Across the App

- **[Feature]** **Bring back the Campaigns module** — The Campaigns area from the legacy admin will be added so you can create, edit, and manage campaigns and offer groups in New Adsmith Frontend. (#200)
- **[Task]** **Users area review** — A documentation review comparing the legacy and new Users screens to identify gaps and plan improvements. (#80)
- **[Feature]** **Brand guidelines for AI output** — A comprehensive brand-guidelines document will be created and used as the main reference to improve the quality of AI-generated output. (#264)
- **[Feature]** **Smarter Link Testing default** — When you open Link Testing from a placement, that placement will be pre-selected for you instead of making you choose. (#238)
- **[Bug]** **Clear error for invalid test links** — Testing an invalid link will show a clear failure message in Link Testing rather than dropping you on the Dashboard. (#239)

## Placements

- **[Bug]** **Clean up the placement create/edit form** — Unfamiliar new fields will be reviewed (removed, relabeled, or explained) and missing links like Preview and Details will be restored. (#234)
- **[Feature]** **Better offer assignment list** — The selected-offers list will default to Manual Order with drag-and-drop reordering, an X to remove an offer, and the ability to filter offers by taxonomy. (#235)
- **[Feature]** **Manual reordering for assigned offers** — Companion to the above: offers will keep the order you arrange them in, using drag-and-drop, with quick removal and taxonomy filtering. (#255)

## Properties

- **[Feature]** **Search box on the Publisher selector** — The property form's publisher dropdown will let you type to find a publisher instead of scrolling through the whole list. (#237)

## Behind the Scenes

- **[Task]** **Today's stats from the live data source** — Groundwork so the Dashboard's "today" view shows accurate, up-to-date impressions, clicks, leads, and revenue. (#34)
- **[Task]** **Daily stats roll-up** — Behind-the-scenes work to summarize live stats into daily totals for faster historical reporting. (#35)
- **[Task]** **Faster Survey performance with caching** — High-priority groundwork to speed up survey delivery by caching placement, offer, and cap data. (#42)
- **[Task]** **Review an old stats job** — Maintenance to decide whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Validate the new pre-ping system in parallel** — The new pre-ping process will run alongside the existing one to confirm it produces matching results before switching over. (#40)
- **[Task]** **Per-advertiser pre-ping checks** — Each advertiser's pre-ping will be verified for correct field mapping and success handling before the switch. (#41)
- **[Task]** **Run new scheduled jobs alongside the old ones** — New background jobs will run in parallel with the existing ones in production, monitored daily for any differences. (#43)
- **[Task]** **Retire legacy scheduled jobs — group 3** — Lower-risk legacy survey-stats jobs will be switched off once their replacements prove stable. (#44)
- **[Task]** **Retire legacy scheduled jobs — group 2** — Several stats-related legacy jobs will be switched off and monitored for a week. (#45)
- **[Task]** **Retire legacy scheduled jobs — group 1 (critical)** — The most critical legacy jobs, including lead processing and offer-cap resets, will be switched off last, with close monitoring and instant rollback ready. (#46)
- **[Task]** **Document rollback steps** — Clear recovery procedures will be written and tested for each production system in case anything needs to be reverted. (#48)
- **[Task]** **Troubleshooting runbooks** — Step-by-step guides for common issues (lead processing, stats, offer caps, pre-ping, and connections) will be created for support staff. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 687487fb5892cb0959b36f8b6c4eb3ec174c16bbb22d3dcbdd9d3df606803281 -->
