# Open Issues — Plain-Language Overview

_Last updated 2026-06-24 11:01:57 UTC · 47 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date range on the Dashboard** — Choosing "Custom" in the date filter will finally open start and end date pickers, so you can view Dashboard data for any range you like instead of just the preset options. (#58)
- **[Feature]** **Light mode option** — A new theme switch will let you flip the Admin between the current dark look and a lighter one, with your choice remembered next time you sign in. (#59)
- **[Feature]** **Working buttons on detail pages** — Edit, Preview, and Pull Leads buttons on Placement, Modal, Offer, and Advertiser detail pages will actually do something when clicked instead of sitting idle. (#154)
- **[Feature]** **Sub-ID Stats moved to the Dashboard** — Sub-ID performance stats will live in the Dashboard reporting area rather than tucked inside the placement form, where they're easier to find. (#236)
- **[Bug]** **Missing Dashboard sections restored** — Campaign stats, top offers, and watch lists will return to the Dashboard and respond to your date-range selection, instead of only the system overview loading. (#240)
- **[Feature]** **New monitoring views and activity log** — A new "Other Dashboard" area will add views for long-running and low-converting offers, plus a searchable record of changes like pausing offers or adjusting caps. (#256)
- **[Feature]** **Full names shown on the Dashboard** — Advertiser and placement names will no longer be cut off with an ellipsis, so you can read them in full. (#260)
- **[Feature]** **ID column removed** — The ID/number column will be dropped from Dashboard tables to free up screen space for the information you actually use. (#261)
- **[Feature]** **Tidier publisher and property names** — Names will display only the part after the last colon (e.g. "Acme Publishing"), removing the noisy prefixes. (#262)
- **[Feature]** **Consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for better, more consistent readability. (#263)

## Offers

- **[Feature]** **Set more fields when creating an offer** — Piggyback offers, HD pixel placements, and ZIP code targeting will be available right when you create an offer, so you no longer have to save first and then edit. A high-priority improvement. (#142)
- **[Feature]** **Enforce required pre-ping fields** — When a pre-ping is set to run before a data push, leads missing required fields will be stopped up front rather than slipping through. (Needs a quick confirmation before it's built.) (#218)
- **[Feature]** **Clearer offer status colors** — Paused will be red, Active green, and Capped yellow/orange, so statuses are easy to tell apart at a glance in the offer list and on the Dashboard. (#246)
- **[Feature]** **Easier advertiser and state targeting on the offer form** — You'll be able to type to search for an advertiser, and paste or type a comma-separated list of states for targeting. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in a group to the Conflicting Offers list in one step, saving lots of manual work. (#250)
- **[Task]** **Offer row action links** — Quick links (Edit, Quick Edit, Trash, View, Preview, Trends, Details) will appear under each offer title, with Trends opening an offer performance page like the legacy system. (#252)
- **[Bug]** **Offer preview rendering and linkouts** — Formatted text in the More Info and TCPA fields will display properly instead of showing raw code, and linkout offers will work correctly from the preview. (#259)

## Flows

- **[Task]** **Flow form styling fixes** — Text boxes, color pickers, checkboxes, and side-by-side fields on the Flow form will display correctly instead of looking unstyled or stacked. (#152)
- **[Feature]** **"Add all fields" button** — When building a flow's form, one click will add every available field at once instead of adding them one at a time. (#224)
- **[Feature]** **Clearer step-order setting** — The step-order control on the flow form will get labels or help text so it's obvious what it controls. (#226)
- **[Feature]** **Skip the "Claim your offers" intro** — Visitors will land directly on the form fields, removing the extra opening page. (#228)
- **[Feature]** **Better TCPA consent checkbox** — On the published lander, the consent checkbox will be larger, rounded, and properly aligned with its text. (#229)
- **[Feature]** **Footer copyright and site name** — The lander footer will show the copyright line and site name, which are currently missing. (#232)
- **[Bug]** **CPA offers no longer trap visitors** — Visitors will be able to decline or move past a CPA offer instead of being forced to click "Yes" to continue. A high-priority fix. (#233)

## General / Across the App

- **[Feature]** **Campaigns module** — The Campaigns area from the legacy system will be rebuilt so you can view, create, edit, and configure campaigns and offer groups. A critical, high-priority gap. (#200)
- **[Feature]** **Searchable publisher selector** — On the property form, you'll be able to type to find a publisher instead of scrolling a long list. (#237)
- **[Feature]** **Smarter Link Testing default** — Opening Link Testing from a placement will pre-select that placement for you. (#238)
- **[Bug]** **Link Testing shows real errors** — Testing an invalid link will return a clear error in the Link Testing screen instead of bouncing you to the Dashboard. (#239)
- **[Task]** **Users management review** — A comparison of the old and new Users screens to confirm which features still need to be brought over. (#80)

## Placements

- **[Bug]** **Clean up the Placement create/edit form** — Unfamiliar new fields will be reviewed and either removed, relabeled, or explained, and missing links like Preview and Details will be restored. (#234)
- **[Feature]** **Reorder assigned offers** — The offer assignment list will default to manual order, support drag-and-drop reordering, an "X" to remove an offer, and filtering by taxonomy. (#235)
- **[Feature]** **Drag-and-drop offer assignment** — Selected offers will keep the order you set, with drag-and-drop reordering and a remove button, addressing the offer assignment test. (#255)

## Reports

- **[Bug]** **Advertiser shown for every offer** — The Offers report will display advertiser information for all offers, resolving the remaining gap left after the earlier data fix. (#242)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will return to 15-minute increments, giving you the fine-grained view needed to spot offer and partner issues quickly. (#243)

## Behind the Scenes

- **[Task]** **Faster survey loading** — Adding a caching layer so survey pages and offer rules load more quickly. A high-priority improvement. (#42)
- **[Task]** **Real-time "today" stats** — Work to make today's impressions, clicks, leads, and revenue available in near real time. (#34)
- **[Task]** **Historical stats roll-up** — Automatically summarizing daily stats so historical reporting stays accurate. (#35)
- **[Task]** **Pre-ping safety testing** — Running the new pre-ping process alongside the existing one to confirm it behaves identically before switching over. (#40)
- **[Task]** **Per-advertiser pre-ping checks** — Validating pre-ping for each active advertiser before the switch-over. (#41)
- **[Task]** **Scheduled stats job review** — Checking whether an older stats job is still needed or can be retired. (#33)
- **[Task]** **Run new scheduled jobs in parallel** — Running the new background jobs alongside the current ones to compare results before relying on them. (#43)
- **[Task]** **Phased switch-over of background jobs** — Carefully retiring older scheduled jobs in stages, starting with the lowest-risk ones and monitoring each step. (#44)
- **[Task]** **Continued switch-over of stats jobs** — Retiring the next group of older stats jobs once the earlier stage proves stable. (#45)
- **[Task]** **Final switch-over of critical jobs** — Retiring the most critical background jobs last, with close monitoring and the ability to revert. (#46)
- **[Task]** **Rollback procedures documented** — Writing clear steps to safely revert each system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides** — Creating step-by-step guides for handling common operational issues. (#49)
- **[Feature]** **Brand guidelines as the AI standard** — Establishing a comprehensive brand-guidelines document to use as the primary input for AI-generated output quality. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 687487fb5892cb0959b36f8b6c4eb3ec174c16bbb22d3dcbdd9d3df606803281 -->
