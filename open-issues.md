# Open Issues — Plain-Language Overview

_Last updated 2026-06-28 16:26:29 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a proper start- and end-date picker, so you can view Dashboard numbers for exactly the range you care about instead of only the preset options. (#58)
- **[Task]** **Bring back the missing Dashboard sections** — A high-priority fix to restore the campaign stats, top offers, and watch list sections so the Dashboard shows full reporting again, with the date range updating them as expected. (#240)
- **[Feature]** **New "Other Dashboard" views plus a change history** — Adds "Offers with Legs" and "CLP Performance" views (flagging CLP offers converting under 30%) and a searchable log that records offer pauses, cap changes, and other updates with who made them and when. (#256)
- **[Task]** **Consistent Dashboard color scheme** — A defined color palette will be applied across the Dashboard so charts and sections are easier to read at a glance. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole Admin between dark and light themes from your user menu, and your choice will be remembered next time you log in. (#59)
- **[Feature]** **Protection against two people overwriting each other's edits** — When you open a record to edit, it will be locked and clearly labeled if someone else already has it open, and if a record changes while you're working you'll be prompted to reload — preventing one person from silently wiping out another's changes. (#267)
- **[Task]** **Users area review against the old system** — A behind-the-scenes comparison of the old and new Users screens to identify which features (like bulk role changes, last-login, and two-factor status) still need adding, so the new Users area can reach full parity. (#80)
- **[Bug]** **Invalid link test should show an error, not the Dashboard** — When you test a link that isn't valid in Link Testing, you'll get a clear failure message instead of being unexpectedly sent to the Dashboard. (#239)

## Offers, Campaigns & Placements

- **[Feature]** **Bring back the Campaigns module** — A high-priority addition so you can again view, create, edit, and configure campaigns and offer groups (titles, CTA text, offer handling, order, and partners) directly in the new Admin. (#200)
- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and a taxonomy filter to find offers faster. (#235)
- **[Feature]** **Enforce required fields on pre-pings before sending** — When a pre-ping runs before a data push, leads missing required fields will be stopped right away rather than being sent out and relying on the advertiser to reject them. (#218)

## Flows

- **[Task]** **Tidy up the Flow form styling** — Cleans up unstyled areas of the Flow form (text boxes, color pickers, checkboxes, and side-by-side fields) so it looks consistent with the Placement and Modal forms. (#152)
- **[Feature]** **Make "Step order" easy to understand** — The Flow form's step order setting will get a clearer label and inline help explaining what it controls and what the values mean, so it's no longer guesswork. (#226)

## Behind the Scenes

- **[Feature]** **Live "today" stats** — Work to power the Dashboard's "today" view with up-to-the-hour impressions, clicks, leads, and revenue in the correct Eastern time zone. (#34)
- **[Feature]** **Faster historical reporting** — A new process to roll up live stats into daily totals so historical reports load reliably. (#35)
- **[Task]** **Survey performance caching** — High-priority groundwork to speed up surveys by caching placement, offer, and cap information for quicker responses. (#42)
- **[Task]** **Review of an old stats job** — Checking whether a legacy stats routine is still needed or can be retired without affecting your reports. (#33)
- **[Task]** **Safety testing of the new pre-ping system** — Running the new pre-ping process alongside the old one to confirm results match before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Validating each active advertiser's pre-ping setup so nothing breaks during the switchover. (#41)
- **[Task]** **Rolling out the new scheduled jobs** — Running the new automated jobs alongside the existing ones and watching for any differences. (#43)
- **[Task]** **Retiring older scheduled jobs (survey stats)** — Carefully switching off a lower-risk legacy job once its replacement is proven stable. (#44)
- **[Task]** **Retiring more scheduled jobs (stats aggregation)** — Switching off the next group of legacy stats jobs after a monitoring period. (#45)
- **[Task]** **Retiring the most critical scheduled jobs** — The final, closely monitored switch-off of the most important legacy jobs (lead processing and offer cap resets), with an immediate fallback ready. (#46)
- **[Task]** **Documented recovery steps** — Writing and testing clear rollback procedures so any system can be reverted quickly if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides** — Creating step-by-step guides for handling common issues like lead processing or cap reset failures. (#49)
- **[Task]** **Brand guidelines for AI output** — Establishing a single, thorough brand-guidelines document to use as the main reference for AI-generated content, improving quality and consistency. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
