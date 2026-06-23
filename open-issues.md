# Open Issues — Plain-Language Overview

_Last updated 2026-06-23 20:43:20 UTC · 49 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Bug]** **Custom date range on the Dashboard** — Today the "Custom" option in the date filter doesn't do anything. Once fixed, choosing it will open a start/end date picker so you can view Dashboard data for any range you like. (#58)
- **[Feature]** **Light mode for the Admin** — You'll be able to switch the whole Admin between the current dark theme and a new light theme, with your choice remembered next time you sign in. (#59)
- **[Feature]** **Make detail-page buttons work** — The Edit, Preview, and Pull Leads buttons on Placement, Modal, Offer, and Advertiser detail pages currently do nothing when clicked. They'll be wired up so they take you where you expect. (#154)
- **[Feature]** **Sub-ID Stats moving to the Dashboard** — Sub-ID Stats will be relocated out of the placement form and into the Dashboard reporting area, where this kind of data belongs. (#236)
- **[Bug]** **Restore missing Dashboard sections** — Right now only the system overview loads. Campaign stats, top offers, and watch lists will be brought back, and they'll respond to the date-range selection. (#240)
- **[Feature]** **Clearer offer status colors** — Paused will become red, Capped yellow/orange, and Active green, so you can tell statuses apart at a glance across the offer list and Dashboard. (#246)
- **[Feature]** **New monitoring views and an activity log** — Adds "Offer with Legs" and "CLP Performance" views (highlighting low-converting CLP offers) plus a searchable record of changes like pausing offers or editing caps. (#256)
- **[Feature]** **Show full advertiser and placement names** — Long names will no longer be cut off with "…" in Dashboard views, so you can read them in full. (#260)
- **[Feature]** **Remove the ID number column** — The ID/number column will be dropped from Dashboard tables to free up screen space for the information you actually use. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon (e.g. "Acme Publishing" instead of "Foo: Bar: Acme Publishing"), making lists easier to scan. (#262)
- **[Feature]** **A consistent Dashboard color scheme** — A defined palette will be applied throughout the Dashboard for better, more consistent readability. (#263)

## Offers
- **[Feature]** **Set more fields when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting can currently only be added after the offer exists. You'll be able to set them right when you create the offer. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — When a pre-ping is set to run before a data push, leads missing required fields will be stopped up front rather than relying on the partner's system to catch them. (Awaiting confirmation this is the desired change.) (#218)
- **[Bug]** **Advertiser info on the Offers report** — Some offers still show no advertiser in the Offers report. This data issue will be resolved so advertiser details appear for every offer. (#242)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will return to 15-minute increments, making it easier to spot errors or partner-server issues quickly. (#243)
- **[Bug]** **Status filter on the Offers report** — You'll be able to narrow the Offers report to a status (Active, Paused, Capped) instead of seeing everything at once. (#244)
- **[Bug]** **Offer images not showing** — Images aren't rendering in the offer form. We'll find out whether it's a data or display problem and fix it so artwork appears. (#247)
- **[Feature]** **Easier advertiser and state entry on offers** — The Advertiser field gets a type-to-search box, and state targeting will accept a typed or pasted comma-separated list (e.g. CA, TX, FL). (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers** — On the Delivery & Settings tab, you'll be able to add every offer in a group to the Conflicting Offers list in one step, saving a lot of manual clicking. (#250)
- **[Task]** **Quick action links under each offer** — Adds the familiar row actions (Edit, Quick Edit, Trash, View, Preview, Trends, Details) beneath offer titles, with Trends opening an offer activity/performance view. (#252)
- **[Bug]** **HTML and linkouts in offer previews** — More Info and TCPA fields currently show raw HTML code, and linkout offers don't work in preview. Content will render properly and linkouts will function. (#259)

## Flows
- **[Task]** **Tidy up the Flow form's appearance** — The Flow form has several styling problems, such as plain-white text boxes and fields stacking instead of sitting side by side. It'll be brought in line with the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field with a single click. (#224)
- **[Feature]** **Explain the "Step order" setting** — Labels and help text will clarify what the step-order control does and what its values mean. (#226)
- **[Feature]** **Skip the "Claim your offers" page** — New flows will land visitors straight on the form fields instead of showing an extra intro page first. (#228)
- **[Feature]** **Better TCPA consent checkbox** — The consent checkbox will be made larger, rounded, and properly aligned with its text on the published lander. (#229)
- **[Feature]** **Footer with copyright and site name** — The lander footer will include the copyright line and site name pulled from General Information. (#232)
- **[Bug]** **Visitors trapped on CPA offers** — In the CPA flow there's no way to decline an offer or move past it, leaving real visitors stuck. We'll add a working way to proceed or decline. (#233)

## Placements
- **[Bug]** **Clean up the placement create/edit form** — The form shows unfamiliar new fields and is missing links like Preview and Details. We'll review the fields against the legacy version and restore the missing links. (#234)
- **[Feature]** **Reorder assigned offers by hand** — The offer transfer list will default to manual order, support drag-and-drop reordering, add an "X" to remove offers, and let you filter the offer list by taxonomy. (#235)
- **[Feature]** **Manual ordering for offer assignment (follow-up)** — Same improvement tracked from UAT: manual default order, drag-and-drop, an "X" to remove, and taxonomy filtering on the placement offer list. (#255)

## General / Across the App
- **[Feature]** **Bring back the Campaigns module** — The Campaigns area from the legacy admin isn't in the new product yet. It'll be rebuilt so you can view, create, edit, and configure campaigns and their offer groups. (#200)
- **[Task]** **Review of the Users area** — A side-by-side comparison of the legacy and new Users management screens, identifying missing capabilities (like bulk actions and 2FA visibility) to guide upcoming work. (#80)
- **[Feature]** **Stronger brand guidelines for AI output** — A comprehensive brand-guidelines document will be created and used as the main input for AI-generated content to improve quality and consistency. (#264)

## Link Testing
- **[Feature]** **Default to the placement you came from** — When you open Link Testing from a placement, that placement will already be selected instead of making you pick it. (#238)
- **[Bug]** **Clear error for invalid links** — Testing an invalid link currently dumps you on the Dashboard. Instead, you'll see a clear failure message in Link Testing. (#239)

## Properties
- **[Feature]** **Search box for the publisher selector** — You'll be able to type to find a publisher on the property form instead of scrolling through the whole list. (#237)

## Behind the Scenes
- **[Task]** **Faster "today" figures** — Work to power the Dashboard's "today" view with up-to-the-hour impressions, clicks, leads, and revenue. (#34)
- **[Task]** **Reliable historical reporting** — Behind-the-scenes work to roll up daily totals so longer-term reports stay accurate and fast. (#35)
- **[Task]** **Quicker surveys** — Adds a caching layer so survey pages, offers, and caps load faster for visitors. High priority. (#42)
- **[Task]** **Review of an old scheduled job** — Maintenance to decide whether a legacy stats job is still needed or can be retired. (#33)
- **[Task]** **Validate the new pre-ping system in parallel** — The new lead-checking system will run alongside the existing one and be compared to confirm it behaves identically before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Each active advertiser's pre-ping will be tested individually to confirm field mapping and pass/fail logic before going live. (#41)
- **[Task]** **Roll out new background jobs alongside the old ones** — The new scheduled jobs will run in parallel with the current ones in production while we monitor for any differences. (#43)
- **[Task]** **Retire low-risk scheduled jobs** — Step-by-step switch-off of the least critical legacy jobs once their replacements prove stable. (#44)
- **[Task]** **Retire mid-tier scheduled jobs** — Continued careful switch-off of stats-related legacy jobs after the first tier is confirmed stable. (#45)
- **[Task]** **Retire the most critical jobs last** — The lead-processing and offer-cap jobs will be switched over last, with close monitoring and an immediate fallback ready. (#46)
- **[Task]** **Document how to roll back** — Clear recovery steps will be written and tested for each production system in case something needs to be reverted. (#48)
- **[Task]** **Troubleshooting guides for the team** — Step-by-step guides for handling common issues like lead-processing or stats problems, so they can be resolved quickly. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 2193e483427bbca7ef4a993b1881469ca39305841dcaa1ee15d37bf610c688fa -->
