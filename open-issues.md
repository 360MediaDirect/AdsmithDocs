# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 14:57:10 UTC · 47 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a proper start- and end-date picker, so you can view dashboard data for any range you choose instead of only preset options like Today or This Month. (#58)
- **[Feature]** **Light mode option for the Admin** — You'll be able to switch between the current dark theme and a new light theme, with your choice remembered next time you sign in. (#59)
- **[Feature]** **Working Edit, Preview, and Pull Leads buttons on detail pages** — These buttons on Placement, Modal, Offer, and Advertiser detail pages will actually do something when clicked instead of sitting there unresponsive. (#154)
- **[Feature]** **Sub-ID Stats move to the Dashboard** — Sub-ID stats will live in the Dashboard reporting area rather than buried inside the placement form, making them easier to find and review. (#236)
- **[Bug]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will load again alongside the system overview, and the date range selector will update them. (#240)
- **[Feature]** **New monitoring views and an activity log** — Adds "Offer with Legs" and CLP performance views (highlighting offers converting under 30%) plus a searchable record of changes like pausing offers or adjusting caps. (#256)
- **[Feature]** **Show full advertiser and placement names** — Long names will no longer be cut off with "…", so you can read them in full. (#260)
- **[Feature]** **Remove the ID column** — Dropping the ID/number column frees up screen space for the information that matters. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon (e.g. "Acme Publishing" instead of "Foo: Bar: Acme Publishing") for easier reading. (#262)
- **[Feature]** **Consistent dashboard colors** — A defined color palette will be applied across the Dashboard for better, more consistent readability. (#263)

## Flows

- **[Task]** **Fix the Flow form's appearance** — Textareas, color pickers, checkboxes, and paired fields will be properly styled and laid out side by side, matching the polished look of the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field in a single click. (#224)
- **[Feature]** **Clearer "Step order" setting** — Labels and help text will explain what the step-order control does and what its values mean, so it's no longer a mystery. (#226)
- **[Feature]** **Remove the extra "Claim your offers" page** — Visitors will land directly on the form instead of clicking through an extra intro screen first. (#228)
- **[Feature]** **Better TCPA checkbox styling** — On the published lander, the consent checkbox will be larger, rounded, and properly aligned with its text. (#229)
- **[Feature]** **Footer copyright and site name** — The lander footer will show the copyright line and site name pulled from General Information. (#232)
- **[Bug]** **Let visitors decline or move past a CPA offer** — Visitors are currently forced to click "Yes" to continue, with no way to decline or exit; this fix lets them proceed through the flow normally. (#233)

## Offers

- **[Feature]** **Set more fields when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting will be available right when you create an offer, instead of forcing you to save first and then edit. (#142)
- **[Feature]** **Enforce required fields on pre-ping** — When a pre-ping runs before pushing data, missing required fields will stop the lead immediately rather than relying on the advertiser's endpoint to catch it. (Pending a decision to confirm this is the desired behavior.) (#218)
- **[Feature]** **Distinct status colors** — Paused will be red, Capped yellow/orange, and Active green, so you can tell them apart at a glance in offer lists and dashboard indicators. (#246)
- **[Feature]** **Easier advertiser and state targeting on the offer form** — You'll be able to type to search for an advertiser and enter state targeting as a comma-separated list (e.g. CA, TX, FL) instead of only picking from a long list. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add all offers in a group to the Conflicting Offers list at once, saving considerable time. (#250)
- **[Task]** **Quick action links under each offer** — Adds familiar row actions (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an offer activity page showing lead and revenue performance over time. (#252)
- **[Bug]** **Fix HTML display and link-outs in offer preview** — Headline, More Info, and TCPA fields will show formatted text and working links rather than raw code, and linkout offers will redirect correctly from the preview. (#259)

## Flows / Placements

- **[Bug]** **Tidy up the Placement create/edit form** — Unfamiliar new fields will be reviewed (removed, relabeled, or explained) and missing links like Preview and Details will be restored. (#234)
- **[Feature]** **Better offer assignment list** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove, and filtering by taxonomy. (#235)
- **[Feature]** **Drag-and-drop offer ordering on Placements** — Lets you manually arrange assigned offers and keep that order, with an "X" to remove and taxonomy filtering (addresses the same need as #235). (#255)

## General / Across the App

- **[Feature]** **Bring back the Campaigns module** — A full Campaigns area will let you view, create, edit, and configure campaigns and offer groups, matching what the legacy admin offers today. This is a high-priority gap. (#200)
- **[Task]** **Users area review** — A comparison of the old and new Users screens to identify missing items (like bulk actions, last login, and 2FA status) and plan how to close the gaps. (#80)
- **[Feature]** **Stronger brand guidelines for AI output** — Establishing a comprehensive brand-guidelines document to drive higher-quality, more on-brand AI-generated content. (#264)

## Reports

- **[Bug]** **Show advertiser info on the Offers report** — Some offers still appear without their advertiser; this resolves the remaining data issue so advertiser details show for every offer. (#242)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will return to 15-minute increments, helping you spot errors and partner-server issues quickly. (#243)

## Link Testing

- **[Feature]** **Pre-select the placement you started from** — When you open Link Testing from a placement, that placement will already be selected so you don't have to find it again. (#238)
- **[Bug]** **Show an error for invalid links** — Testing an invalid link will return a clear failure message instead of bouncing you to the dashboard. (#239)

## Properties

- **[Feature]** **Search box for the publisher selector** — You'll be able to type to find a publisher on the property form instead of scrolling through the full list. (#237)

## Behind the Scenes

- **[Task]** **Review an older stats job** — Checking whether a legacy stats process is still needed or can be retired, with the decision documented. (#33)
- **[Task]** **Faster "today" stats** — Work to pull up-to-the-hour numbers for today's view, correctly handling Eastern Time. (#34)
- **[Task]** **Reliable historical stats** — Rolling up daily totals so longer-term reporting stays accurate. (#35)
- **[Task]** **Safe testing of the new pre-ping system** — Running the new and old systems side by side to confirm results match before switching over. (#40)
- **[Task]** **Per-advertiser pre-ping checks** — Verifying each active advertiser's pre-ping works correctly ahead of the switchover. (#41)
- **[Task]** **Speed improvements for the survey engine** — Adding a caching layer so surveys and offers load faster. A high-priority improvement. (#42)
- **[Task]** **Run new and old scheduled jobs in parallel** — Operating both systems together and monitoring daily to catch any differences. (#43)
- **[Task]** **Gradual switchover, step three** — Retiring the lowest-risk legacy scheduled jobs and watching the replacements closely. (#44)
- **[Task]** **Gradual switchover, step two** — Retiring the next group of legacy stats jobs after the prior step proves stable. (#45)
- **[Task]** **Gradual switchover, final step** — Retiring the most critical legacy jobs last, with the ability to roll back immediately if needed. (#46)
- **[Task]** **Document rollback steps** — Writing and testing recovery procedures for each major system so issues can be reversed quickly. (#48)
- **[Task]** **Create troubleshooting guides** — Preparing step-by-step guides for common operational issues to speed up support. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 687487fb5892cb0959b36f8b6c4eb3ec174c16bbb22d3dcbdd9d3df606803281 -->
