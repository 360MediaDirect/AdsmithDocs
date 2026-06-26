# Open Issues — Plain-Language Overview

_Last updated 2026-06-26 03:05:15 UTC · 15 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Picking "Custom" in the date filter will open a proper start- and end-date picker so you can view dashboard data for any specific stretch of time, with the chosen range shown right on the filter button. (#58)
- **[Feature]** **Sub-ID Stats move to the Dashboard** — The Sub-ID Stats section is being relocated out of the placement form and into the Dashboard's reporting area, where this kind of performance data belongs. (#236)
- **[Task]** **Bring back missing Dashboard sections** — Campaign stats, top offers, and watch lists will reappear on the Dashboard, and changing the date range will properly refresh them. A high-priority fix so the Dashboard shows the full picture again. (#240)
- **[Feature]** **New "Other Dashboard" monitoring views and an activity log** — You'll get dedicated views for long-running ("Offers with Legs") and CLP offers, with under-30% converters flagged for quick action, plus a searchable record of every change (pauses, cap edits, status updates) for easy auditing. (#256)
- **[Task]** **Consistent Dashboard color scheme** — A defined set of colors will be applied across the Dashboard so charts and sections are easier to read at a glance. (#263)

## General / Across the App

- **[Feature]** **Dark and Light mode for the Admin** — You'll be able to switch the whole Admin between dark and light themes from your user menu, with your choice remembered next time you sign in. Helpful for bright rooms, low light, and personal comfort. (#59)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper failure message in Link Testing instead of unexpectedly dropping you onto the Dashboard. (#239)
- **[Feature]** **Protection against two people overwriting the same record** — When you open a record someone else is already editing, you'll see who has it and when, and the app will warn you before anyone's changes can be accidentally wiped out. This applies across all the main entity screens. (#267)
- **[Task]** **Stronger brand guidelines for AI output** — The team will maintain a comprehensive brand-guidelines document and use it as the main reference for AI-generated content, leading to more on-brand, higher-quality results. (#264)

## Offers

- **[Feature]** **Bring back the Campaigns module** — Campaign management is being rebuilt in New Adsmith Frontend so you can create, edit, and configure campaigns and their offer groups just like in the legacy system. A high-priority feature, since this is core to day-to-day work. (#200)
- **[Bug]** **Required fields enforced before a lead is pushed** — When a pre-ping runs before pushing data, missing required fields will stop the lead right away rather than relying on the advertiser's response, closing a gap where incomplete leads could slip through. (Pending confirmation that this is the desired behavior.) (#218)

## Flows

- **[Task]** **Polish the Flow form's appearance** — The Flow form will get proper styling so textareas, color pickers, and checkboxes look right and paired fields sit side by side instead of stacking, matching the cleaner look of other forms. (#152)
- **[Feature]** **Make the "Step order" setting easier to understand** — Clearer labels and help text will explain what step order controls and what its values mean, so it's no longer a guessing game when building a flow. (#226)

## Reports

- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will return to 15-minute increments, giving you the fine-grained view needed to spot errors and partner-server issues quickly. (#243)

## Placements

- **[Feature]** **Easier offer selection and ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer (so clicking is reserved for dragging), and the ability to filter the offer list by taxonomy. (#235)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 2a56fd67f9291cb8ae4aad8782237f68a408d23759c09f54732863f026266184 -->
