# Open Issues — Plain-Language Overview

_Last updated 2026-06-29 03:06:24 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Light mode option for the Admin** — A new theme switch lets you choose between the current dark look and a brighter light theme, with your choice remembered next time you sign in. Helpful for different lighting or personal preference. (#59)
- **[Feature]** **Protection against two people overwriting the same record** — When someone else is already editing an offer, flow, placement, advertiser, or other record, you'll see a clear "locked by" notice, and saves are checked so one person's changes can't silently wipe out another's. (#267)
- **[Task]** **Users area review against the old system** — A side-by-side check of the old and new Users screens to spot anything still missing (like bulk actions, last-login, and two-factor status) so the new Users area can catch up. (#80)
- **[Task]** **Cleaner, brand-aligned AI results** — Adopting a single, thorough brand guidelines document as the main reference so AI-generated content comes out more consistent and on-brand. (#264)
- **[Bug]** **Invalid link tests now show a clear error** — When you test a bad link, you'll get a proper failure message instead of being unexpectedly bounced back to the Dashboard. (#239)

## Dashboard

- **[Task]** **Restore the missing Dashboard sections** — Brings back the campaign stats, top offers, and watch lists alongside the system overview, and makes the date range actually update them. (#240)
- **[Task]** **Custom date range on the Dashboard** — Choosing "Custom" will open a start/end date picker so you can view Dashboard data for any range you like, not just the preset options. (#58)
- **[Feature]** **New "Other Dashboard" views plus an activity log** — Adds an "Offers with Legs" view and a CLP performance view that flags offers converting under 30%, plus a searchable log of changes like pausing offers or adjusting caps, with who did it and when. (#256)
- **[Task]** **Consistent Dashboard colors** — A defined color palette will be applied across Dashboard views for easier, more readable visuals. (#263)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The Step order field gets a plain-language label and inline help explaining what it controls, so you no longer have to guess what it does. (#226)
- **[Task]** **Tidy up the Flow form's appearance** — Fixes unstyled areas of the Flow form (text boxes, color pickers, checkboxes, and side-by-side fields) so it looks polished and consistent with the Placement and Modal forms. (#152)

## Placements

- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by category. (#235)

## Pre-Pings

- **[Feature]** **Catch missing required fields before sending** — A lead missing a required field will be stopped up front instead of being sent out and relying on the advertiser to reject it, helping keep bad leads from slipping through. (#218)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — Adds the missing Campaigns area so you can view, create, edit, and configure campaigns and offer groups, matching what the old admin system offered. High priority. (#200)

## Behind the Scenes

- **[Task]** **Faster Survey Engine** — Adds a caching layer so survey placements and offer data load more quickly during real-time use. High priority. (#42)
- **[Feature]** **Today's stats for the Dashboard** — Behind-the-scenes work to pull current-day impressions, clicks, leads, and revenue (in Eastern Time) for the Dashboard's "today" view. (#34)
- **[Feature]** **Reliable historical stats** — Sets up automatic rollups of live data into daily totals so longer-term reporting stays accurate. (#35)
- **[Task]** **Pre-ping accuracy checks** — Runs the new pre-ping process alongside the old one to compare results and response times before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping verification** — Confirms each advertiser's pre-ping behaves correctly before the switch, so nothing breaks at go-live. (#41)
- **[Task]** **Review of a legacy stats job** — Checks whether an older statistics process is still needed or can be retired. (#33)
- **[Task]** **Deploy the new scheduled jobs in parallel** — Runs the new automated background jobs alongside the existing ones, monitoring daily for any differences. (#43)
- **[Task]** **Phased switch-over of background jobs (lower-risk batch)** — Retires the first set of older scheduled jobs once their replacements prove stable, with monitoring in place. (#44)
- **[Task]** **Phased switch-over of background jobs (mid-tier batch)** — Retires the next group of older statistics jobs after the previous batch is confirmed stable. (#45)
- **[Task]** **Phased switch-over of background jobs (most critical batch)** — Carefully retires the most important jobs (lead processing and offer-cap resets) last, with close monitoring and the ability to roll back instantly. (#46)
- **[Task]** **Documented recovery steps** — Writes and tests clear rollback procedures for each major system in case something needs to be reversed. (#48)
- **[Task]** **Troubleshooting guides** — Creates step-by-step guides for handling common issues like lead processing or stats problems, so they can be resolved quickly. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
