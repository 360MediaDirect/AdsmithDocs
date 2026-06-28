# Open Issues — Plain-Language Overview

_Last updated 2026-06-28 10:44:09 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

These items are mostly behind-the-scenes maintenance to move the engine that powers reporting, leads, and scheduled jobs onto the new platform. You won't see changes on screen, but they keep New Adsmith Frontend fast, accurate, and reliable.

- **[Feature]** **Faster "today" stats** — Today's impressions, clicks, leads, and revenue will be pulled from a quicker, more current source so live numbers stay accurate (in Eastern Time). (#34)
- **[Feature]** **Automatic daily stats roll-up** — Daily totals will be assembled automatically in the background, keeping historical reporting consistent and up to date. (#35)
- **[Task]** **Tidy up an old stats job** — A review of a legacy statistics routine to decide whether it's still needed or can be retired, avoiding duplicate work. (#33)
- **[Task]** **Speed boost for the survey engine** — Groundwork to cache placement, offer, and cap information so surveys load and respond faster. High priority. (#42)
- **[Task]** **Side-by-side pre-ping testing** — The new lead pre-check system will be run alongside the old one to confirm it produces the same results before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Each active advertiser's pre-check will be verified for correct field handling before the switch, so leads are validated properly. (#41)
- **[Task]** **Roll out the new scheduled jobs** — The new background jobs go live alongside the existing ones, with daily monitoring to catch any differences. (#43)
- **[Task]** **Retire old scheduled jobs (first group)** — Lower-risk legacy jobs (such as hourly survey stats) are switched off once their replacements prove stable. (#44)
- **[Task]** **Retire old scheduled jobs (second group)** — Several statistics and reporting jobs are switched off after a week of stable monitoring. (#45)
- **[Task]** **Retire old scheduled jobs (most critical group)** — The most important jobs, including lead processing and offer-cap resets, are switched off last with close monitoring and a quick rollback ready. Critical. (#46)
- **[Task]** **Safety-net rollback plans** — Clear procedures to quickly revert any production system if something goes wrong, each tested in advance. (#48)
- **[Task]** **Troubleshooting guides** — Step-by-step guides for the support team to resolve common issues quickly, reducing downtime. (#49)

## Dashboard

- **[Task]** **Restore missing dashboard sections** — Campaign stats, top offers, and watch lists will return to the dashboard, and the date range selector will update them. Currently only the system overview loads. High priority. (#240)
- **[Feature]** **New "Other Dashboard" views and activity log** — Adds an "Offers with Legs" view, a CLP performance view that flags offers converting under 30%, and a searchable log of changes (such as pausing offers or editing caps) showing who changed what and when. (#256)
- **[Task]** **Custom date range on the dashboard filter** — Picking "Custom" will open a start/end date picker so you can view data for any range you choose, not just preset periods. (#58)
- **[Feature]** **Dark and light mode** — You'll be able to switch between dark and light themes from your account menu, with your choice remembered next time you sign in. (#59)
- **[Task]** **Consistent dashboard colors** — A defined color palette will be applied across the dashboard for cleaner, easier-to-read visuals. (#263)

## Flows

- **[Task]** **Fix Flow form styling** — Cleans up the look of the Flow form so text boxes, color pickers, checkboxes, and paired fields display neatly and consistently with other forms. (#152)
- **[Feature]** **Clearer "Step order" setting** — The "Step order" option will get a plain-language label and helpful inline explanation so it's obvious what it controls and what the values do. (#226)

## General / Across the App

- **[Feature]** **Prevent overwriting each other's edits** — When two people open the same record, New Adsmith Frontend will show who's currently editing and warn before anyone saves over someone else's changes, protecting your work across all entity forms. (#267)
- **[Task]** **Adopt brand guidelines for AI output** — A comprehensive brand-guidelines document will be used as the main input for AI-generated content to improve quality and consistency. (#264)

## Pre-Pings

- **[Feature]** **Enforce required fields before pushing a lead** — When a pre-ping runs before sending data, leads missing required information will be stopped up front rather than relying on the advertiser's system to catch them. (#218)

## Placements

- **[Feature]** **Better offer ordering and filtering** — Selected offers will default to manual order, support drag-and-drop reordering, include an "X" to remove an offer, and let you filter the offer list by taxonomy. (#235)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — Adds the missing Campaigns area so you can create, edit, and manage campaigns and offer groups in New Adsmith Frontend, matching the legacy admin. Critical, high priority. (#200)

## Link Testing

- **[Bug]** **Show an error for invalid links** — Testing an invalid link will return a clear failure message instead of sending you to the dashboard. (#239)

## Users

- **[Task]** **Users area gap review** — A documented comparison of the Users area against the legacy version, identifying missing features (like bulk actions, last-login, and 2FA details) to guide upcoming improvements. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
