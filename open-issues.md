# Open Issues — Plain-Language Overview

_Last updated 2026-06-29 00:35:46 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Feature]** **Faster, accurate "today" numbers** — Behind-the-scenes work to pull up-to-the-hour figures for impressions, clicks, leads, and revenue so the "today" view reflects current activity in the right time zone. (#34)
- **[Feature]** **Reliable historical reporting totals** — Daily roll-ups of activity are being set up so longer-term reports stay accurate and quick to load. (#35)
- **[Task]** **Speed improvements for surveys and offers** — A new caching layer will make survey, offer, and cap information load faster in real time. High priority. (#42)
- **[Task]** **Review of an old stats job** — Checking whether an older background statistics process is still needed or can be retired, with no change to what you see. (#33)
- **[Task]** **Pre-ping accuracy testing** — Running the new pre-ping system alongside the existing one to confirm results match before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each advertiser's pre-ping setup so leads are validated correctly after the switch. (#41)
- **[Task]** **Rolling out new background jobs safely** — New scheduled processes will run in parallel with the existing ones and be watched daily before anything is switched off. (#43)
- **[Task]** **Phased switchover of background jobs (lower risk)** — Retiring the first batch of older survey-stats processes once their replacements prove stable. (#44)
- **[Task]** **Phased switchover of background jobs (medium risk)** — Retiring additional statistics and reporting processes after a monitoring period. (#45)
- **[Task]** **Phased switchover of the most critical background jobs** — Carefully retiring the most important lead-processing and offer-cap processes last, with the ability to roll back immediately if needed. (#46)
- **[Task]** **Documented recovery steps** — Writing and testing clear rollback procedures for each major system so issues can be reversed quickly. (#48)
- **[Task]** **Troubleshooting guides for the support team** — Creating step-by-step guides for common operational issues so problems get resolved faster. (#49)

## Dashboard

- **[Task]** **Restore missing dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date range will update them. Right now only the system overview loads. High priority. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds an "Offers with Legs" view and a CLP performance view that flags offers converting under 30%, plus a searchable log of changes (pauses, cap updates, status changes) showing who did what and when. (#256)
- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open a date range picker with start and end dates so you can view data for any period you need. (#58)
- **[Task]** **A polished, consistent dashboard look** — A defined color palette will be applied across dashboard views for better readability and a more uniform appearance. (#263)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is editing a record (an offer, flow, placement, advertiser, and more), others will see it's locked and by whom, and saves will warn you if the record changed since you opened it — so no one's work gets silently lost. (#267)
- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole admin between dark and light themes, and your choice will be remembered the next time you log in. (#59)
- **[Task]** **Stronger brand guidelines for AI output** — A comprehensive brand-guidelines document will be used as the main input for AI-generated content to improve quality and consistency. (#264)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain-language label and helpful explanation so you can tell exactly what it controls and what its values do. (#226)
- **[Task]** **Tidy up the Flow form's appearance** — Fixes for unstyled text boxes, color pickers, checkboxes, and side-by-side fields so the Flow form looks consistent with the Placement and Modal forms. (#152)

## Placements

- **[Feature]** **Better control over selected offers** — Offers will default to manual order, with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)

## Offers & Pre-Pings

- **[Feature]** **Stop incomplete leads at push time** — When a pre-ping runs before sending data, leads missing required fields will be blocked right away instead of being passed along, closing a gap where bad data could slip through. (#218)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — The Campaigns area from the older system will be rebuilt so you can view, create, edit, and configure campaigns and offer groups in New Adsmith Frontend. Critical, high priority. (#200)

## Users

- **[Task]** **Review of the Users area against the old system** — A documented comparison of the older Users screens versus the new ones, identifying missing pieces (like bulk actions and certain columns) to guide upcoming improvements. (#80)

## Link Testing

- **[Bug]** **Show a clear error for invalid links** — Testing an invalid link will display a proper error message instead of sending you to the Dashboard. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
