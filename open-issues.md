# Open Issues — Plain-Language Overview

_Last updated 2026-06-23 00:52:12 UTC · 50 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Bug]** **Custom date ranges on the Dashboard** — Choosing "Custom" in the date filter will finally open a start and end date picker, so you can view dashboard data for any range you choose. (#58)
- **[Feature]** **Light mode for the Admin** — You'll be able to switch between the current dark theme and a new light theme, and your choice will be remembered next time you log in. (#59)
- **[Feature]** **Working Edit, Preview and Pull Leads buttons** — On the placement, modal, offer and advertiser detail pages these buttons will actually take you where you expect instead of doing nothing. (#154)
- **[Feature]** **Sub-ID Stats moving to the Dashboard** — Sub-ID performance stats will live in the Dashboard reporting area instead of being tucked inside the placement form. (#236)
- **[Bug]** **Missing dashboard sections restored** — Campaign stats, top offers and watch lists will load again, and the date-range selector will properly update them. (#240)
- **[Feature]** **New monitoring views and an activity log** — A new "Other Dashboard" with "Offer with Legs" and CLP performance views, plus a searchable log of changes like pausing offers or editing caps. (#256)
- **[Feature]** **Full advertiser and placement names** — Long names will no longer be cut off with "…" so you can read them in full. (#260)
- **[Feature]** **More room in dashboard tables** — The ID/number column will be removed to free up screen space. (#261)
- **[Feature]** **Cleaner publisher and property names** — Names will display only the part after the last colon, so "Foo: Bar: Acme Publishing" simply reads "Acme Publishing". (#262)
- **[Feature]** **A consistent color scheme** — The dashboard will adopt a defined palette for clearer, more readable screens. (#263)

## Offers

- **[Feature]** **Set every offer option at creation** — Piggyback offers, HD pixel placements and ZIP-code targeting can be set right when you create an offer, instead of having to save it and come back to edit. High priority. (#142)
- **[Feature]** **Stricter pre-ping checks** — A decision is pending on whether leads missing required fields should be blocked before a pre-ping is sent, to help stop incomplete leads slipping through. (#218)
- **[Feature]** **Clearer offer status colors** — Paused will be red, Active green and Capped yellow/orange, so you can tell them apart at a glance. (#246)
- **[Bug]** **Offer images will display** — Offer images that currently fail to appear in the offer form will show correctly. (#247)
- **[Feature]** **Faster offer form entry** — The Advertiser field gets a type-to-search box, and state targeting will accept a typed or pasted comma-separated list (e.g. CA, TX, FL). (#249)
- **[Feature]** **Add a whole offer group as conflicting** — On the Delivery & Settings tab you'll be able to add every offer in a group to Conflicting Offers in one step, saving lots of manual work. (#250)
- **[Task]** **Familiar offer row actions** — Quick links such as Edit, Quick Edit, Trash, View, Preview, Trends and Details return under each offer, with Trends opening an offer activity and performance page. (#252)
- **[Bug]** **Proper formatting and working linkouts in offer previews** — Headline, More Info and TCPA fields will show formatted text and links instead of raw code, and Linkout offers will work from the preview. (#259)

## Flows

- **[Task]** **Polished Flow form layout** — The Flow form's text boxes, color pickers, checkboxes and paired fields will be properly styled and shown side by side, matching the other forms. (#152)
- **[Feature]** **Add all form fields at once** — A single button will add every available field to a flow's Form tab, instead of adding them one at a time. (#224)
- **[Bug]** **Turn header and footer on or off** — You'll get controls to disable the header, footer and other sections of the flow form. (#225)
- **[Feature]** **Clearer "step order" setting** — Labels and help text will explain what the step-order control does and what its values mean. (#226)
- **[Feature]** **Flows start on the form** — The extra "Claim your offers" intro page is being removed so visitors land directly on the form fields. (#228)
- **[Feature]** **Better TCPA checkbox** — The consent checkbox on the lander will be larger, rounded and properly aligned with its text. (#229)
- **[Feature]** **Footer with copyright and site name** — Rendered landers will show the copyright line and the site name in the footer. (#232)
- **[Bug]** **Visitors can decline CPA offers** — A bug that traps visitors by forcing a "Yes" click will be fixed so they can decline or move past the offer. High priority. (#233)

## General / Across the App

- **[Feature]** **Campaigns module coming to the new app** — The Campaigns feature from the old admin—creating and managing campaigns and offer groups—will be rebuilt here so this core workflow is available again. Critical, high priority. (#200)
- **[Bug]** **Clear error for invalid links** — Testing a bad link in Link Testing will show a proper error instead of bouncing you to the dashboard. (#239)
- **[Feature]** **Link Testing remembers your placement** — Opening Link Testing from a placement will pre-select that placement automatically, instead of making you pick. (#238)
- **[Feature]** **Search the publisher list on Properties** — A type-to-search box on the property form's publisher selector saves scrolling to find the one you need. (#237)
- **[Task]** **Users area review** — A review comparing the new Users management screen with the old one, to spot missing items like bulk actions, two-factor status and last-login info. (#80)
- **[Feature]** **Stronger brand guidelines** — A comprehensive brand-guidelines document will be created to guide AI-generated output for more consistent results. (#264)

## Placements

- **[Bug]** **Placement form cleanup** — Unfamiliar new fields will be reviewed and the missing Preview and Details links restored on the placement create/edit form. (#234)
- **[Feature]** **Reorder assigned offers by hand** — Placements gain manual-order sorting, drag-and-drop reordering, an X to remove an offer, and filtering by taxonomy. (#235)
- **[Feature]** **Drag-and-drop offer assignment** — Companion work to the offer transfer list, bringing manual ordering, drag-and-drop, remove buttons and taxonomy filtering to placements. (#255)

## Reports

- **[Bug]** **Advertiser column on the Offers report** — Remaining data issues will be resolved so every offer shows its advertiser information. (#242)
- **[Feature]** **15-minute offer stats** — The offer detail timespan chart returns to 15-minute increments, making it easier to spot offer or partner-server issues quickly. (#243)

## Behind the Scenes

- **[Bug]** **Fixing data accuracy between systems** — Investigating why some stats and offer details come through empty or mismatched, including missing "yesterday" numbers. A high-priority blocker. (#241)
- **[Task]** **Faster surveys** — Adding a caching layer so survey pages, offers and caps load and check more quickly. High priority. (#42)
- **[Feature]** **Faster "today" stats** — Behind-the-scenes work so the dashboard's "today" figures update in near real time. (#34)
- **[Feature]** **Reliable historical stats** — Routine roll-ups of hourly data into daily totals to keep historical reporting accurate. (#35)
- **[Task]** **Review of an older stats job** — Checking whether an older sub-ID stats process is still needed or can be retired. (#33)
- **[Task]** **Pre-ping safety testing** — Running the new pre-ping system alongside the old one to confirm matching results before switching over. (#40)
- **[Task]** **Per-advertiser pre-ping checks** — Validating each advertiser's pre-ping setup before go-live. (#41)
- **[Task]** **Safer move to new scheduled jobs** — Running new and old background jobs side by side to confirm everything matches before relying on the new ones. (#43)
- **[Task]** **Retiring older scheduled jobs (first group)** — Switching off lower-risk legacy background jobs once their replacements prove stable. (#44)
- **[Task]** **Retiring more scheduled jobs** — Turning off the next set of legacy stats jobs after a period of monitoring. (#45)
- **[Task]** **Retiring the most critical jobs last** — Carefully switching off core lead-processing and offer-cap jobs, with the ability to revert immediately if needed. (#46)
- **[Task]** **Documented recovery steps** — Writing clear rollback procedures for each system in case something needs to be reverted. (#48)
- **[Task]** **Troubleshooting guides** — Step-by-step guides for quickly resolving common issues such as stats or lead-processing hiccups. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 56a32f4c7fb7a8cf5da851848990923ce422a0050b61e7812ca5d1ca22f7aaa6 -->
