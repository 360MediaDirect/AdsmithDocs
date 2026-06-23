# Open Issues — Plain-Language Overview

_Last updated 2026-06-23 16:48:48 UTC · 49 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Set piggyback offers, HD pixel placements, and ZIP targeting at creation** — Today you have to save a new offer first and then re-open it to add these details. Soon you'll be able to set them all while first creating the offer. (#142)
- **[Feature]** **Enforce required fields before sending a lead (pre-ping)** — When a pre-ping runs before pushing data, missing required information will stop the lead right away instead of letting an incomplete lead slip through. (This one needs a final go-ahead before it's built.) (#218)
- **[Bug]** **Advertiser names missing from the Offers report** — A fix so every offer correctly shows its advertiser, instead of leaving that information blank. (#242)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail chart will break activity into 15-minute increments, making it easier to spot errors or partner-server issues quickly. (#243)
- **[Bug]** **Status filter on the Offers report** — You'll be able to narrow the Offers report to Active, Paused, or Capped offers instead of seeing everything at once. (#244)
- **[Feature]** **Clearer status colors for offers** — Paused will be red, Active green, and Capped yellow/orange, so you can tell statuses apart at a glance across lists and dashboard indicators. (#246)
- **[Bug]** **Offer images not showing on the offer form** — A fix so offer images display correctly instead of appearing blank. (#247)
- **[Feature]** **Easier advertiser search and state targeting on the offer form** — You'll be able to type to find an advertiser and enter state targeting as a typed/pasted comma-separated list (e.g. CA, TX, FL). (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in a group to the conflicting list in one step, saving considerable time. (#250)
- **[Task]** **Bring back offer row action links** — Each offer will show familiar quick links (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an offer activity and performance page. (#252)
- **[Bug]** **HTML and linkouts not working in offer preview** — More Info and TCPA fields will render formatted text and working links, and linkout offers will redirect properly from the preview. (#259)

## Dashboard

- **[Bug]** **Custom date range picker on the Dashboard** — Choosing "Custom" will open start and end date pickers so you can view dashboard data for any range you like, not just the preset options. (#58)
- **[Feature]** **Light/Dark mode toggle** — You'll be able to switch the Admin between dark and light themes to match your preference and lighting, with your choice remembered next time. (#59)
- **[Feature]** **Working Edit, Preview, and Pull Leads buttons on detail pages** — These buttons on Placement, Modal, Offer, and Advertiser detail pages will actually take action when clicked instead of doing nothing. (#154)
- **[Feature]** **Move Sub-ID Stats to the Dashboard** — Sub-ID statistics will live in the Dashboard reporting area rather than buried inside the placement form. (#236)
- **[Bug]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date-range selector will update them. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds dedicated views for long-running offers and low-converting CLP offers, plus a searchable record of every offer change (pauses, cap changes, and more) for easy auditing. (#256)
- **[Feature]** **Show full advertiser and placement names** — Long names will no longer be cut off with "…", so you can read them in full. (#260)
- **[Feature]** **Remove the ID/number column** — Dropping this column frees up screen space for the information that matters. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon (e.g. "Foo: Bar: Acme Publishing" shows as "Acme Publishing"). (#262)
- **[Feature]** **Standardized dashboard colors** — A defined color palette will be applied consistently across the Dashboard for better readability. (#263)

## Flows

- **[Task]** **Fix Flow form styling** — Text boxes, color pickers, checkboxes, and section layouts will look polished and consistent, with paired fields sitting side-by-side like other forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Add every available form field in one click instead of adding them one at a time. (#224)
- **[Feature]** **Make the "Step order" setting understandable** — Clearer labels or help text so you know exactly what this controls and what its values mean. (#226)
- **[Feature]** **Skip the "Claim your offers" intro page** — Visitors will land directly on the form fields instead of an extra opening step. (#228)
- **[Feature]** **Better TCPA consent checkbox styling** — The consent checkbox will be larger, rounded, and properly aligned with its text on the live lander. (#229)
- **[Feature]** **Add footer copyright and site name** — The lander footer will include the copyright line and site name pulled from General Information. (#232)
- **[Bug]** **Visitors stuck on CPA offers** — Fixes a problem where visitors are forced to click "Yes" with no way to decline or move past a CPA offer, which currently traps them mid-flow. (#233)

## General / Across the App

- **[Task]** **Users area review** — A study comparing the new Users screens to the legacy version to identify missing features (like bulk actions and last-login info) and plan improvements. (#80)
- **[Feature]** **Bring back the Campaigns module** — Restores the ability to view, create, edit, and configure campaigns and offer groups, matching the legacy admin. This is a high-priority, core capability that's currently missing. (#200)
- **[Feature]** **Add search to the publisher selector on Properties** — Type to find a publisher instead of scrolling a long list. (#237)
- **[Feature]** **Link Testing defaults to the placement you opened it from** — Opens already pointed at that placement, so you don't have to pick it each time. (#238)
- **[Bug]** **Clear error for invalid links in Link Testing** — Testing a bad link will show a proper failure message instead of dropping you back on the dashboard. (#239)
- **[Feature]** **Brand guidelines as the main input for AI output** — Establishes a comprehensive brand-guidelines document to improve the quality and consistency of AI-generated output. (#264)

## Placements

- **[Bug]** **Tidy up the placement create/edit form** — Unfamiliar fields will be reviewed (removed, relabeled, or explained) and missing links like Preview and Details will be restored. (#234, #255)
- **[Feature]** **Reorder and manage assigned offers more easily** — Offers will default to manual order, with drag-and-drop reordering, an "X" to remove, and the ability to filter the offer list by taxonomy. (#235)

## Behind the Scenes

- **[Task]** **Today's live statistics groundwork** — Behind-the-scenes work to power accurate "today" numbers (impressions, clicks, leads, revenue) on the Dashboard. (#34)
- **[Task]** **Automatic stats roll-up for history** — Maintenance to summarize live stats into daily totals for reliable historical reporting. (#35)
- **[Task]** **Review an old stats job** — Checking whether a legacy statistics process is still needed or can be retired. (#33)
- **[Task]** **Side-by-side pre-ping testing** — Running the new and old pre-ping systems together to confirm they match before switching over. (#40)
- **[Task]** **Per-advertiser pre-ping checks** — Verifying each advertiser's pre-ping works correctly before the switch. (#41)
- **[Task]** **Faster Survey Engine** — High-priority groundwork to speed up surveys by caching frequently used settings and offer data. (#42)
- **[Task]** **Run new scheduled jobs alongside the old ones** — Deploying updated background jobs in parallel with the existing ones and watching for any differences. (#43)
- **[Task]** **Phased switch-over of scheduled jobs (lower risk)** — Retiring less-critical background jobs once their replacements prove stable. (#44)
- **[Task]** **Phased switch-over of scheduled jobs (mid-tier)** — Retiring the next group of background jobs after the first round is confirmed stable. (#45)
- **[Task]** **Phased switch-over of scheduled jobs (most critical)** — Carefully retiring the most important background jobs last, with close monitoring and quick rollback if needed. (#46)
- **[Task]** **Rollback plans** — Documenting how to safely revert each production system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides** — Creating step-by-step guides for resolving common operational issues quickly. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 2193e483427bbca7ef4a993b1881469ca39305841dcaa1ee15d37bf610c688fa -->
