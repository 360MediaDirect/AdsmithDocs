# Open Issues — Plain-Language Overview

_Last updated 2026-06-28 03:06:07 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

These items are largely under-the-hood maintenance and reliability work. Most won't change what you see day to day, but they make reporting faster and the platform more dependable.

- **[Task]** **Review an older stats-tracking job** — We're checking whether a legacy stats process is still needed or can be safely retired, so the system isn't doing duplicate work. (#33)
- **[Feature]** **Up-to-the-minute "today" numbers** — Today's impressions, clicks, leads, and revenue will reflect current-day activity more accurately on the Dashboard and reports. (#34)
- **[Feature]** **Automatic roll-up of historical stats** — Daily totals will be compiled automatically so historical reports stay fast and accurate. (#35)
- **[Task]** **Side-by-side testing of the new pre-ping system** — We're running the new and old lead-checking systems together to confirm the new one behaves identically before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping validation** — Each advertiser's pre-ping setup will be verified before the switch, reducing the risk of misrouted or rejected leads. (#41)
- **[Task]** **Speed improvements for the Survey engine** — A new caching layer will make surveys and offers load faster for visitors. This is high priority. (#42)
- **[Task]** **Run new scheduled jobs alongside the old ones** — The new automated jobs will run in parallel with the existing ones so we can compare results before relying on them. (#43)
- **[Task]** **Retire older scheduled jobs (first group)** — A first set of legacy background jobs will be turned off once their replacements prove stable. (#44)
- **[Task]** **Retire older scheduled jobs (second group)** — A further set of legacy stats jobs will be switched off after a monitoring period. (#45)
- **[Task]** **Retire the most critical scheduled jobs (final group)** — The most important background jobs (lead processing and offer-cap resets) will be moved over last, with close monitoring and the ability to roll back instantly. (#46)
- **[Task]** **Document recovery procedures** — Clear, tested steps for reverting each system if something goes wrong, so issues can be resolved quickly. (#48)
- **[Task]** **Create troubleshooting guides** — Step-by-step guides for the support team to resolve common issues like lead processing or stats hiccups faster. (#49)

## Entity Screens (Campaigns, Placements, Offers & Users)

- **[Feature]** **Bring back the Campaigns module** — A core part of the legacy system, Campaigns isn't yet available in New Adsmith Frontend. This will let you create, edit, and manage campaigns and offer groups again. High priority. (#200)
- **[Feature]** **Better offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter offers by taxonomy — making it much easier to arrange offers exactly how you want. (#235)
- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping runs before pushing data, leads missing required information will be stopped up front instead of being sent out and relying on the advertiser to reject them. (#218)
- **[Bug]** **Invalid link should show an error, not the Dashboard** — In Link Testing, entering an invalid link currently dumps you onto the Dashboard. Once fixed, you'll get a clear failure message instead. (#239)
- **[Task]** **Users area feature review** — A documented comparison of the old and new Users screens, highlighting features still to be added (such as bulk actions, last-login, and 2FA status) so nothing important is lost in the move. (#80)

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open a start/end date picker so you can view Dashboard data for any range you like, not just preset periods. (#58)
- **[Task]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date-range selector will update them. High priority. (#240)
- **[Feature]** **New Dashboard views plus an activity log** — Adds "Offers with Legs" and "CLP Performance" views (flagging CLP offers converting under 30%) and a searchable log of changes like pausing offers or adjusting caps, with who made them and when. (#256)
- **[Task]** **Consistent Dashboard color scheme** — A defined color palette will be applied across the Dashboard for cleaner, more readable visuals. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the entire admin between dark and light themes, with your choice remembered between visits. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — If two people open the same record, you'll see a clear "locked by" notice and a warning if it changed while you had it open — preventing one person's changes from silently erasing another's. (#267)
- **[Task]** **Brand guidelines as the basis for AI output** — A comprehensive brand-guidelines document will be used as the main input for AI-generated content, improving the quality and consistency of results. (#264)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Several parts of the Flow form look unstyled or misaligned (text boxes, color pickers, checkboxes, and side-by-side fields). This cleanup will make the form match the polished look of the Placement and Modal forms. (#152)
- **[Feature]** **Make the "Step order" setting understandable** — This setting is currently confusing. A clearer label and inline help text will explain what it controls and what the values mean, so you can use it confidently without outside help. (#226)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
