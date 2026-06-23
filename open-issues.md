# Open Issues — Plain-Language Overview

_Last updated 2026-06-23 22:27:09 UTC · 47 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range picker on the Dashboard** — Choosing "Custom" in the date filter will finally open a start/end date picker, so you can view dashboard data for any range you like instead of just preset options. (#58)
- **[Feature]** **Light/Dark mode toggle** — You'll be able to switch the whole admin between the current dark theme and a new light theme, with your choice remembered next time you log in. (#59)
- **[Feature]** **Working Edit/Preview/Pull Leads buttons on detail pages** — Buttons on the Placement, Modal, Offer, and Advertiser detail pages that currently do nothing will take you where you expect, removing a confusing dead end. (#154)
- **[Feature]** **Sub-ID Stats moved to the Dashboard** — The Sub-ID Stats view will move out of the placement form and into the Dashboard reporting area, where it belongs. (#236)
- **[Bug]** **Restore missing dashboard sections** — Campaign stats, top offers, and watch lists will return to the dashboard, and the date-range selector will update them as expected. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds an "Offers with Legs" view, a CLP performance view that flags offers converting under 30%, and a searchable record of changes like pausing offers or adjusting caps. (#256)
- **[Feature]** **Show full advertiser and placement names** — Long advertiser and placement names will no longer be cut off, so you can read them in full. (#260)
- **[Feature]** **Remove the ID/number column** — The ID column will be removed from dashboard tables to free up screen space for the information you actually use. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon (for example, "Acme Publishing" instead of "Foo: Bar: Acme Publishing"). (#262)
- **[Feature]** **Standardized dashboard colors** — A defined color palette will be applied consistently across the dashboard for easier reading at a glance. (#263)

## Offers

- **[Feature]** **Set all offer fields during creation** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting will be available when first creating an offer, so you won't have to create it and then edit it to finish the setup. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — A lead missing required fields will be stopped up front rather than relying on the partner's response, preventing incomplete leads from slipping through. (Decision needed before this change.) (#218)
- **[Bug]** **Advertiser info missing on the Offers report** — A data fix so every offer correctly shows its advertiser in the Offers report. (#242)
- **[Feature]** **15-minute granularity on offer timespan stats** — The offer detail timespan chart will show 15-minute increments again, making it a useful tool for spotting issues with offers or partner servers quickly. (#243)
- **[Feature]** **Distinct offer status colors** — Paused will be red, Active green, and Capped yellow/orange, so you can tell them apart instantly across the offer list and dashboard. (#246)
- **[Feature]** **Easier advertiser selection and state targeting on the offer form** — Adds type-to-search for the Advertiser field and lets you type or paste a comma-separated list of states (e.g. CA, TX, FL). (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in an offer group to the Conflicting Offers list in one step, saving significant time. (#250)
- **[Task]** **Offer row action links** — Adds legacy quick links (Edit, Quick Edit, Trash, View, Preview, Trends, Details) under each offer title, with Trends opening an offer activity/performance page. (#252)
- **[Bug]** **HTML and linkout issues in Offer preview tabs** — More Info Headline, More Info Content, and TCPA Content will display formatted text and working links instead of raw code, and Linkout offers will work from the preview. (#259)

## Surveys

- **[Bug]** **CPA offers trap the visitor** — Visitors will be able to decline or move past a CPA offer instead of being forced to click "Yes," fixing a flow that currently strands real consumers. (#233)
- **[Feature]** **Start flows directly on the form** — The extra "Claim your offers" page before the form will be removed so visitors land straight on the form fields. (#228)
- **[Feature]** **Better TCPA checkbox styling** — The consent checkbox will be larger, rounded, and properly aligned with its text for a cleaner, clearer lander. (#229)
- **[Feature]** **Footer with copyright and site name** — The lander footer will include the copyright line and site name, which are currently missing. (#232)

## Placements

- **[Bug]** **Clean up the placement create/edit form** — Unexpected new fields will be reviewed and removed or relabeled, and missing links like Preview and Details will be restored to match what you're used to. (#234)
- **[Feature]** **Reorder assigned offers by hand** — The offer transfer list will default to manual order with drag-and-drop reordering, an "X" to remove offers, and the ability to filter by taxonomy. (#235)
- **[Feature]** **Manual offer ordering and drag-and-drop (UAT follow-up)** — Confirms the offer assignment list keeps the order you set, supports drag-and-drop, an "X" to remove, and taxonomy filtering. (#255)

## Flows

- **[Task]** **Fix Flow form styling** — The Flow form's textareas, color pickers, checkboxes, and paired side-by-side fields will look consistent and properly styled like the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Add every available form field in one click instead of adding them one at a time. (#224)
- **[Feature]** **Clearer "Step order" setting** — Labels and help text (or a reworked control) will make it obvious what the step-order setting controls and what its values mean. (#226)

## General / Across the App

- **[Feature]** **Bring back the Campaigns module** — A high-priority addition so you can view, create, edit, and configure campaigns and offer groups in New Adsmith Frontend, matching the legacy system. (#200)
- **[Task]** **Users management review** — A comparison of the current Users area against the legacy system to identify missing pieces (like bulk actions and additional columns) and plan improvements. (#80)
- **[Feature]** **Adopt brand guidelines for AI-assisted output** — Establishes a comprehensive brand-guidelines document to be used as the main reference, improving the consistency and quality of generated output. (#264)

## Link Testing

- **[Feature]** **Default to the placement you came from** — Opening Link Testing from a placement will pre-select that placement, so you don't have to find it manually each time. (#238)
- **[Bug]** **Show an error for invalid links** — Testing an invalid link will return a clear failure message instead of dropping you back on the dashboard. (#239)

## Properties

- **[Feature]** **Searchable publisher selector** — Adds type-to-search to the publisher dropdown on the property form so you can find a publisher without scrolling. (#237)

## Behind the Scenes

- **[Task]** **Review legacy sub-ID stats job** — Confirming whether an older background stats process is still needed or can be retired. (#33)
- **[Task]** **Real-time "today" stats** — Behind-the-scenes work so the dashboard's "today" view shows up-to-the-hour impressions, clicks, leads, and revenue in the correct time zone. (#34)
- **[Task]** **Roll up stats for historical reporting** — Automatically summarizing recent activity into daily totals so historical reports stay fast and accurate. (#35)
- **[Task]** **Test the new pre-ping system safely** — Running the new pre-ping process alongside the old one to confirm results match before switching over. (#40)
- **[Feature]** **Verify pre-ping per advertiser** — Checking each active advertiser's pre-ping setup so leads are handled correctly after the switch. (#41)
- **[Task]** **Faster survey performance** — Adding a caching layer to speed up survey-related lookups; high priority. (#42)
- **[Task]** **Run new scheduled jobs in parallel** — Running new and old background jobs side by side and monitoring them before fully switching over. (#43)
- **[Task]** **Gradual job switchover — Tier 3** — Retiring the least-critical legacy background jobs after their replacements prove stable. (#44)
- **[Task]** **Gradual job switchover — Tier 2** — Retiring the next set of legacy stats jobs after a week of stable monitoring. (#45)
- **[Task]** **Gradual job switchover — Tier 1 (critical)** — Carefully retiring the most critical legacy jobs (lead processing and offer cap resets) last, with the ability to roll back instantly. (#46)
- **[Task]** **Document rollback steps** — Writing and testing recovery procedures for each major system in case anything needs to be reversed. (#48)
- **[Task]** **Create troubleshooting guides** — Step-by-step guides for resolving common operational issues like lead-processing or stats problems. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 687487fb5892cb0959b36f8b6c4eb3ec174c16bbb22d3dcbdd9d3df606803281 -->
