# Open Issues — Plain-Language Overview

_Last updated 2026-06-25 20:39:45 UTC · 17 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Picking "Custom" in the date filter will finally open a start- and end-date picker, so you can view dashboard data for any specific stretch of time instead of just preset ranges like Today or This Month. (#58)
- **[Feature]** **Light mode option for the Admin** — A new theme switch lets you flip between the current dark look and a brighter light mode, with your choice remembered next time you sign in. Easier on the eyes in any lighting. (#59)
- **[Bug]** **Edit, Preview, and Pull Leads buttons that do nothing** — On several detail pages (placements, modals, offers, advertisers) these buttons currently don't respond when clicked. This fix wires them up so they actually take you where you expect. (#154)
- **[Task]** **Restore missing dashboard sections** — Campaign stats, top offers, and watch lists will return to the dashboard, and the date-range selector will properly update them. Right now only the system overview loads. High priority. (#240)
- **[Feature]** **Sub-ID Stats moving to the Dashboard** — The Sub-ID Stats section will move out of the placement form and into the Dashboard reporting area, where it's easier to find and review. (#236)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will show activity in 15-minute increments again, giving you the close-up view needed to spot offer or partner-server issues quickly. (#243)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds dedicated views for long-running ("Offer with Legs") and CLP offers, highlighting underperformers, plus a searchable record of every change—like pausing an offer or adjusting daily caps—for easy auditing and troubleshooting. (#256)
- **[Task]** **Consistent dashboard colors** — A defined color palette will be applied across the dashboard so everything looks cleaner and is easier to read at a glance. (#263)

## General / Across the App

- **[Feature]** **Campaigns module brought into the new platform** — The Campaigns area from the older admin isn't here yet. This adds the ability to view, create, edit, and configure campaigns and offer groups, restoring a core part of day-to-day work. Critical, high priority. (#200)
- **[Feature]** **Protection against two people overwriting each other** — When you open a record to edit it, others will see it's in use, and you'll be warned if someone changed it since you opened it—so edits no longer get silently lost. This applies across all the main edit screens. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently bounces you to the dashboard with no explanation. Instead, you'll get a clear failure message right where you ran the test. (#239)
- **[Task]** **Brand guidelines for better AI output** — A comprehensive brand-guidelines document will be created and used as the main reference for AI-generated content, improving quality and consistency. A documentation update. (#264)

## Offers

- **[Bug]** **Set all offer details when first creating an offer** — Today, certain fields (piggyback offers, HD pixel placement IDs, and ZIP code targeting) can only be added after the offer is created. This fix lets you fill them in during initial creation, saving a round trip. High priority. (#142)
- **[Bug]** **Enforce required pre-ping fields before sending** — When a pre-ping runs before a data push, missing required fields currently slip through. This change will stop a lead with missing required information before it's sent. (Awaiting confirmation that this is the desired behavior.) (#218)

## Flows

- **[Task]** **Fix the Flow form's broken styling** — Parts of the Flow form currently look unstyled or misaligned, with paired fields stacking awkwardly. This tidies up the layout so it matches the polished look of the Placement and Modal forms. (#152)
- **[Feature]** **Make the "Step order" setting understandable** — Testers found this control confusing. Clear labels and help text (or a reworked control) will explain what it orders and what each option means. (#226)

## Placements

- **[Feature]** **Better offer selection on placements** — Selected offers will default to manual order with drag-and-drop reordering, an X button to remove an offer (so clicking is reserved for dragging), and the ability to filter the offer list by taxonomy—making it much easier to build and arrange your offer lineup. (#235)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 573b3b1348850b83ce9adbfd70bff61915aebb52583bf841764d1ec76ba30dc9 -->
