# Open Issues — Plain-Language Overview

_Last updated 2026-06-27 08:54:58 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Dark and light mode** — You'll be able to switch New Adsmith Frontend between the current dark look and a new light theme from your user menu, and your choice will stick the next time you sign in. (#59)
- **[Feature]** **Protection against overwriting each other's work** — When two people open the same record (an offer, flow, placement, advertiser, and so on), New Adsmith Frontend will warn you if someone else is already editing it and stop a save from quietly wiping out their changes. (#267)
- **[Bug]** **Clearer result when testing a bad link** — Testing an invalid link will show a proper error message instead of bouncing you back to the Dashboard with no explanation. (#239)
- **[Task]** **Review of the Users area against the old system** — A documentation review comparing the current Users screens to the legacy version, so any missing capabilities (like bulk actions and extra columns) can be planned and added. (#80)
- **[Task]** **Brand guidelines to steer AI output** — A single, thorough set of brand guidelines will become the main reference the AI uses, leading to more on-brand, consistent generated content. (#264)

## Dashboard

- **[Task]** **Custom date range on the Dashboard** — Choosing "Custom" in the date filter will open a start- and end-date picker so you can view Dashboard data for exactly the period you want, with your chosen range shown on the filter button. (#58)
- **[Task]** **Bring back missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and changing the date range will update them as expected. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — You'll get dedicated views for offers with staying power and for CLP offer performance (with low-converting offers highlighted), plus a searchable record of changes like pausing offers or adjusting caps, showing who changed what and when. (#256)
- **[Task]** **A consistent Dashboard color scheme** — The Dashboard will adopt a defined color palette applied across all its views for cleaner, easier-to-read screens. (#263)

## Offers & Campaigns

- **[Feature]** **Campaigns are coming to New Adsmith Frontend** — A full Campaigns area, matching the legacy system, where you can view, create, and edit campaigns and manage offer groups, settings, and assigned offers. This is a high-priority, core capability that's currently missing. (#200)
- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, a clear "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)
- **[Feature]** **Required fields checked before a lead is sent** — For pre-pings that run before data is pushed, leads missing required fields will be stopped up front rather than relying on the advertiser's system to catch them, helping keep incomplete leads from slipping through. (#218)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Remaining styling gaps on the Flow form (such as plain-looking text boxes, color pickers, and side-by-side fields) will be cleaned up so it looks consistent with the Placement and Modal forms. (#152)
- **[Feature]** **Make "Step order" understandable** — The "Step order" setting will get a clearer label and inline help explaining what it controls and what its values do, so you don't have to guess. (#226)

## Behind the Scenes

- **[Feature]** **Up-to-date "today" numbers** — Maintenance to ensure today's impressions, clicks, leads, and revenue are read live and shown correctly (in Eastern Time) on the Dashboard. (#34)
- **[Feature]** **Faster historical reporting** — Behind-the-scenes work to roll up daily totals so longer-term stats load reliably for reports. (#35)
- **[Task]** **Speed improvements for surveys** — Adding a caching layer so survey placements, offers, and caps respond more quickly. This is high priority. (#42)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each active advertiser's pre-ping setup works correctly before the new system goes live. (#41)
- **[Task]** **Side-by-side pre-ping testing** — Running the new pre-ping process alongside the existing one to confirm it behaves identically before switching over. (#40)
- **[Task]** **Reviewing an old stats job** — Checking whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Running new and old scheduled tasks together** — Operating the new and existing automated jobs in parallel and watching for any differences before relying on the new ones. (#43)
- **[Task]** **Careful switchover of routine jobs (lower risk)** — Retiring the first batch of older automated jobs once their replacements prove stable, with the ability to revert. (#44)
- **[Task]** **Careful switchover of routine jobs (mid risk)** — Retiring the next batch of older stats jobs after a week of monitoring. (#45)
- **[Task]** **Careful switchover of critical jobs (highest risk)** — Retiring the most important automated jobs (lead processing and offer-cap resets) last, with close monitoring and instant rollback ready. (#46)
- **[Task]** **Documented recovery steps** — Writing and testing clear rollback procedures for each system so issues can be reversed quickly if needed. (#48)
- **[Task]** **Troubleshooting guides** — Creating step-by-step guides for handling common problems like lead processing or stats hiccups, so issues get resolved faster. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
