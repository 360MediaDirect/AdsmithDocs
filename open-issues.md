# Open Issues — Plain-Language Overview

_Last updated 2026-06-27 05:17:49 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Task]** **Restore the missing dashboard sections** — Right now only the system overview loads. This high-priority fix brings back the campaign stats, top offers, and watch list sections from the previous system, and makes the date-range selector update them. (#240)
- **[Task]** **Custom date range on the dashboard filter** — Choosing "Custom" in the date filter will open a proper start/end date picker so you can view dashboard data for any period you like, with the chosen range shown on the filter button. (#58)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds dedicated views for "Offers with Legs" and CLP offer performance (flagging offers converting under 30%), plus a searchable log of changes like pausing offers or adjusting daily caps, with who made them and when. (#256)
- **[Feature]** **Live "today" figures on the dashboard** — The dashboard's "today" view will show up-to-the-hour impressions, clicks, leads, and revenue so you can see current performance without waiting for overnight totals. (#34)
- **[Task]** **A consistent dashboard color scheme** — A defined color palette will be applied across the dashboard for cleaner, easier-to-read screens. (#263)

## Behind the Scenes
- **[Task]** **Faster Surveys** — A new caching layer will speed up survey loading by keeping frequently used placement, offer, and cap information ready to go. High priority. (#42)
- **[Feature]** **Reliable historical stats** — Behind-the-scenes work to roll up live data into daily totals so historical reports stay accurate over time. (#35)
- **[Task]** **Modernizing scheduled background jobs** — The automated routines that keep stats and leads flowing are being moved to a new, more reliable system, run alongside the old one first to confirm everything matches. (#43)
- **[Task]** **Switching over the least-critical background jobs** — The first set of older scheduled tasks (survey stats) is retired once the replacement proves stable. (#44)
- **[Task]** **Switching over the mid-tier background jobs** — A further set of stats-related scheduled tasks is retired after the previous group runs cleanly. (#45)
- **[Task]** **Switching over the most critical background jobs** — The most important routines (lead processing and offer-cap resets) are moved last, with close monitoring and an instant fallback if needed. (#46)
- **[Task]** **Reviewing an old stats routine** — Checking whether a legacy stats job is still needed or can be safely retired. (#33)
- **[Task]** **Documented recovery steps** — Clear rollback instructions are being written for each major system so any issue can be reversed quickly. (#48)
- **[Task]** **Troubleshooting guides for the support team** — Step-by-step guides for common situations (like lead processing or stats hiccups) so problems get resolved faster. (#49)

## General / Across the App
- **[Feature]** **Dark and light mode** — You'll be able to switch the whole Admin between dark and light themes from your user menu, and your choice is remembered next time you sign in. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, you'll see who else is editing it and be warned before saving over someone else's recent changes, preventing accidental loss of work. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you on the dashboard. It will instead show a clear failure message so you know the link didn't work. (#239)
- **[Task]** **Brand guidelines to guide AI output** — A single, thorough brand-guidelines document will be used as the main input for AI-generated content, improving the quality and consistency of results. (#264)

## Pre-Pings
- **[Feature]** **Stop incomplete leads at the pre-ping step** — When a pre-ping runs before pushing data, leads missing required fields will be blocked up front rather than slipping through, keeping bad data out. (#218)
- **[Feature]** **Per-advertiser pre-ping checks** — Each active advertiser's pre-ping will be verified for correct field mapping and pass/fail handling before the switch-over, so nothing breaks during the transition. (#41)
- **[Task]** **Side-by-side pre-ping testing** — The new pre-ping system will run alongside the old one to compare results and response times, catching any differences before it goes live. (#40)

## Flows
- **[Task]** **Tidy up the Flow form's appearance** — Remaining styling gaps on the Flow form (text boxes, color pickers, checkboxes, and side-by-side fields) will be cleaned up so it looks consistent with the Placement and Modal forms. (#152)
- **[Feature]** **Make "Step order" understandable** — The "Step order" setting will get a clearer label and inline help explaining what it controls and what the values mean, so it's no longer a mystery. (#226)

## Placements
- **[Feature]** **Better control over selected offers** — On Placements, selected offers will default to manual order with drag-and-drop reordering, an "X" button to remove an offer, and the ability to filter the offer list by category. (#235)

## Campaigns
- **[Feature]** **Bring back the Campaigns area** — The Campaigns module is missing from New Adsmith Frontend. This high-priority work adds the ability to view, create, edit, and configure campaigns and offer groups, matching the previous system. (#200)

## Users
- **[Task]** **Review of the Users area against the old system** — A documented comparison of the Users screens to spot missing features (like bulk actions and extra columns) and prioritize what to add next. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
