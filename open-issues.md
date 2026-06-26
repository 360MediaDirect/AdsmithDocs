# Open Issues — Plain-Language Overview

_Last updated 2026-06-26 17:34:07 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Reviewing an older stats job** — We're checking whether an aging behind-the-scenes process for sub-ID statistics is still needed or can be retired, so reporting stays clean and efficient. (#33)
- **[Feature]** **Up-to-the-hour "today" numbers** — Work to power the Dashboard's "today" figures from a faster data source, so impressions, clicks, leads, and revenue for the current day stay accurate and timely (in Eastern Time). (#34)
- **[Feature]** **Faster, reliable historical totals** — A new background process will roll up daily numbers for historical reporting, helping past-period reports load quickly and consistently. (#35)
- **[Task]** **Safer pre-ping switchover** — We'll run the new lead pre-check system side by side with the old one and compare results, so nothing changes for advertisers until the new system is proven correct. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Each active advertiser's pre-ping will be tested individually to confirm fields and success rules are handled correctly before the switch. (#41)
- **[Task]** **Faster surveys through caching** — A new performance layer will speed up survey delivery by keeping placement, offer, and cap information ready for instant checks. High priority. (#42)
- **[Task]** **Bringing new scheduled jobs online** — The new automated background jobs will run alongside the existing ones, monitored daily, so we can confirm they match before relying on them. (#43)
- **[Task]** **Switchover of survey stat jobs** — As part of a careful, staged rollout, the least-risky scheduled jobs (survey stats) move to the new system first, with the old ones ready to turn back on if needed. (#44)
- **[Task]** **Switchover of stats and reporting jobs** — The next group of background jobs (stats aggregation and daily reporting) moves over once the first stage is stable, monitored for a week. (#45)
- **[Task]** **Switchover of critical lead and cap jobs** — The most important background jobs (lead processing and offer-cap resets) move last, with close monitoring and instant rollback ready. (#46)
- **[Task]** **Documented recovery steps** — We're writing clear rollback procedures for each major system, so any issue can be reversed quickly and safely. (#48)
- **[Task]** **Troubleshooting guides for the team** — Step-by-step guides for common situations (like lead-processing or stats hiccups) will help the team resolve issues faster. (#49)

## Dashboard

- **[Task]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date range will update them — so the Dashboard is useful again instead of showing only the system overview. High priority. (#240)
- **[Task]** **Custom date range on the Dashboard** — Choosing "Custom" in the date filter will open a start- and end-date picker so you can view Dashboard data for any time period, with the selected range shown right on the filter button. (#58)
- **[Feature]** **Light and dark mode** — You'll be able to switch the Admin between dark and light themes from the user menu or settings, with your choice remembered next time you sign in. (#59)
- **[Feature]** **New monitoring views and an activity log** — New "Offers with Legs" and CLP performance views will help you spot strong offers and flag CLP offers converting under 30%, plus a searchable log of changes (like pausing offers or adjusting caps) for easy auditing. (#256)
- **[Task]** **Cleaner, consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for better readability and a more polished look. (#263)

## General / Across the App

- **[Feature]** **Prevent two people overwriting each other's edits** — When you open a record to edit, others will see it's being edited by you, and if someone changed it since you opened it you'll be prompted to reload — so edits to offers, flows, placements, advertisers, and more are never silently lost. (#267)
- **[Task]** **Closing the gap with the older Users area** — A detailed review of the older Users screens versus the new one, so missing tools (like bulk actions, last-login, and more) can be prioritized and brought over. (#80)
- **[Task]** **Stronger brand guidelines for better AI output** — We'll establish a single, comprehensive brand-guidelines document to use as the main input for AI-generated content, improving quality and consistency. (#264)
- **[Bug]** **Clear error when testing an invalid link** — Testing an invalid link will show a proper error message instead of unexpectedly sending you back to the Dashboard. (#239)

## Flows

- **[Task]** **Polishing the Flow form's appearance** — We're fixing styling on the Flow form so text boxes, color pickers, checkboxes, and paired fields look consistent and tidy, like the Placement and Modal forms. (#152)
- **[Feature]** **Clearer "Step order" setting** — The Step order setting will get a plain-language label and helpful inline text explaining what it controls and what its values mean, so it's understandable at a glance. (#226)

## Placements & Offers

- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)
- **[Feature]** **Enforce required fields before a lead is pushed** — When a pre-ping runs before pushing data, missing required fields will block the lead up front rather than relying solely on the advertiser's response, helping stop incomplete leads from slipping through. (#218)

## Campaigns

- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — The Campaigns area from the older admin will be added, letting you view, create, and edit campaigns and manage offer groups, settings, and assigned offers. Critical, high priority. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
