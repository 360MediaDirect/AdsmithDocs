# Open Issues — Plain-Language Overview

_Last updated 2026-06-23 00:36:24 UTC · 52 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **Restore the missing dashboard sections** — Campaign stats, top offers, and watch lists will be back on the dashboard, and choosing a date range will update them. Right now only the system overview loads. (#240)
- **A consistent, easy-to-read color scheme** — The dashboard will use a defined set of colors so information is clearer and easier to scan at a glance. (#263)
- **Distinct status colors for offers** — Paused offers will show in red, Capped in yellow/orange, and Active in green, so you can tell them apart instantly instead of Paused and Capped sharing a color. (#246)
- **Cleaner publisher and property names** — When a name contains colons, only the meaningful part after the last colon will be shown (so "Foo: Bar: Acme Publishing" simply reads "Acme Publishing"). (#262)
- **More room on screen** — The ID/number column will be removed from dashboard tables to free up space for the details that matter. (#261)
- **Full names, no cut-off text** — Advertiser and placement names will display in full instead of being clipped with an ellipsis. (#260)
- **New monitoring views and an activity log** — A new "Other Dashboard" area will help you watch long-running offers and spot low-converting CLP offers (under 30%), plus a searchable record of every change like pausing an offer or adjusting a daily cap. (#256)
- **Custom date range on the dashboard filter** — Selecting "Custom" will open a start/end date picker so you can view data for any range you choose, not just the preset options. (#58)
- **Working Edit, Preview, and Pull Leads buttons** — These buttons on placement, modal, offer, and advertiser detail pages will actually take you where they should, instead of doing nothing when clicked. (#154)
- **Sub-ID Stats moved to the Dashboard** — Sub-ID Stats will live in the dashboard reporting area rather than buried inside the placement form. (#236)
- **Light mode option** — A new toggle will let you switch between dark and light themes to suit your environment and preferences; your choice will be remembered. (#59)

## Offers

- **HTML and link-out fixes in the offer preview** — Headlines, More Info, and TCPA content will display properly formatted text and working links instead of raw code, and link-out offers will work correctly from the preview. A bug fix. (#259)
- **Quick action links under each offer** — Familiar shortcuts like Edit, Quick Edit, Trash, View, Preview, Trends, and Details will appear under each offer, with Trends opening an offer activity and performance page. (#252)
- **Offer images will display** — Images on the offer form that currently fail to load will render correctly. A bug fix. (#247)
- **Add a whole offer group to Conflicting Offers at once** — On the Delivery & Settings tab you'll be able to add every offer in a group to the Conflicting Offers list in one step, saving significant time. A new feature. (#250)
- **Easier advertiser and state entry on the offer form** — You'll be able to type to search for an advertiser, and enter state targeting as a typed or pasted comma-separated list (e.g. CA, TX, FL). (#249)
- **More fields available when creating an offer** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting will be settable while creating an offer, instead of having to save it first and then edit. (#142)
- **Stricter pre-ping checks before pushing a lead** — When required fields are missing, a "Before Data Push" pre-ping will stop the lead right away rather than sending it on. A decision is pending before this is finalized. (#218)

## Flows & Surveys

- **Visitors can move past a CPA offer** — Consumers will be able to decline or continue instead of being forced to click "yes," which currently traps them mid-flow. A high-priority bug fix. (#233)
- **Flows start right at the form** — The extra "Claim your offers" intro page will be removed so visitors land directly on the form fields. (#228)
- **Option to turn header and footer on or off** — The flow form will let you disable the header, footer, and other sections. A bug fix. (#225)
- **Add all form fields in one click** — A new button will add every available field to the Form tab at once, instead of adding them one at a time. (#224)
- **Clearer "step order" setting** — The step-order control on the flow form will get labels and help text so it's obvious what it does. (#226)
- **Footer with copyright and site name** — The lander footer will show the copyright line and site name pulled from General Information. (#232)
- **Better-looking TCPA consent checkbox** — The consent checkbox will be larger, rounded, and properly aligned with its text. (#229)
- **Consistent styling across the flow form** — Text boxes, color pickers, checkboxes, and paired fields will be properly styled and laid out instead of appearing unstyled or stacked. (#152)

## Placements

- **Drag-and-drop offer ordering** — You'll be able to set offers to manual order, drag them into the sequence you want, remove them with an "x," and filter the list by taxonomy. (#235, #255)
- **Placement create form cleanup** — Unfamiliar fields will be reviewed and clarified, and missing links like Preview and Details will be restored. A bug fix. (#234)

## Reports

- **Advertiser info on the Offers report** — Every offer will show its advertiser in the Offers report; the gap that remained after the recent data update will be resolved. A bug fix. (#242)
- **15-minute detail on offer timespan stats** — The offer timespan chart will return to 15-minute increments, restoring a key tool for catching offer and partner-server issues early. (#243)

## Link Testing

- **Clear error for invalid links** — Testing a bad link will show a proper error message instead of dropping you back on the dashboard. A bug fix. (#239)
- **Remembers the placement you came from** — Opening Link Testing from a placement will pre-select that placement so you don't have to find it again. (#238)

## Properties

- **Search box for the publisher selector** — You'll be able to type to find a publisher on the property form instead of scrolling through a long list. (#237)

## General / Across the App

- **Campaigns module added** — The Campaigns area from the legacy system will return, letting you create, edit, and manage campaigns and their offer groups. A high-priority new feature. (#200)
- **Stronger brand guidelines for AI output** — A comprehensive brand-guidelines document will guide AI-generated content so results are more consistent and on-brand. (#264)
- **Users area improvements under review** — A review of the Users screens is identifying missing options (such as bulk actions and additional columns) to bring them in line with the previous system. (#80)

## Behind the Scenes

- **Accurate, complete reporting data** — Work is underway to fix a data-sync problem that left yesterday's stats blank, made property counts disagree, and caused some offer data to come through missing. A critical, high-priority fix that will make the numbers you see trustworthy. (#241)
- **Keeping the test environment in sync with live data** so the team can verify changes against realistic information. (#217)
- **Faster survey performance** through added caching of placement, offer, and targeting data. (#42)
- **Validating the new lead-checking and stats systems** before they fully take over, by running them alongside the existing ones and comparing results. (#40, #41, #43)
- **A carefully staged switchover** of scheduled background jobs, monitored at each step with the ability to roll back if anything looks off. (#44, #45, #46)
- **Reliable, up-to-date stats** through new behind-the-scenes processes that record and roll up performance data, including today's figures. (#34, #35, #33)
- **Operational guides for the support team** covering common issues and safe rollback procedures, so problems can be resolved quickly. (#48, #49)
- **An internal test ticket** with no user-facing impact. (#205)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 905b944c449ab732e67e60b5c8026f192146069e39349711713ee642909df73e -->
