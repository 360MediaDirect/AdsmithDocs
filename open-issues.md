# Open Issues — Plain-Language Overview

_Last updated 2026-09-25 06:07:31 UTC · 34 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Manually selected offers now carry over from the old system** — Placements set to "Manual" delivery will show the exact offers you chose (in the right order), instead of showing the wrong or a default offer. (#370)
- **[Bug]** **Saved offer settings will actually take effect on live ads** — Several options you set on an offer weren't reaching the live widget. This ensures the choices you make in the form are the ones visitors actually see. (#295)
- **[Bug]** **"Conflicting Offers" rule works for offers edited in the new admin** — Mutual-exclusion between offers was silently doing nothing for offers touched in the current admin. This restores that protection so conflicting offers don't run together. (#358)
- **[Bug]** **Auto-register offers respect duplicate and conflict rules** — Auto-firing offers will now honor the same group, conflict, and address de-duplication checks as regular offers, so they can't slip past rules that other offers follow. (#355)
- **[Feature]** **Preview shows your unsaved edits** — On placement and offer edit pages, the Preview button will reflect the changes you're currently making, so you no longer have to save first just to see how something looks. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Explore estimating how a new offer is likely to perform based on your historical offer data, replacing the manual gut-check review. (#322)
- **[Feature]** **Decision on the HubSpot List ID field** — This offer field currently does nothing. We'll either connect it to HubSpot or remove it, so the form only shows controls that work. (#362)

## Data Clients

- **[Feature]** **Post-conversion delivery scripts ported over** — The legacy "after success" client behaviors will work on New Adsmith Frontend, so leads continue to be delivered and redirected correctly after conversion. (#327)
- **[Feature]** **File-based pre-checks brought forward** — Hundreds of data clients rely on custom validation that runs before a lead is sent. This ports that logic so those checks keep running. (#338)
- **[Bug]** **Real lead validation for manually entered and broker leads** — Leads added outside the survey flow will be validated for real instead of always being marked "valid," keeping lead quality accurate. (#366)

## Reports & Dashboard

- **[Feature]** **Live "today" numbers on the Dashboard** — The Dashboard will show up-to-the-hour impressions, clicks, leads, and revenue for the current day. (#34)
- **[Task]** **Investigating report differences vs. the old system** — A high-priority review into why some dashboard/report totals didn't match the legacy app, so you can trust the numbers. (#271)

## Surveys

- **[Feature]** **Design tab options fully reflected in the survey** — Every customization you make on the Design tab will show up in the live survey, plus a full check across all entity forms to make sure no option is quietly ignored. (#288)
- **[Bug]** **Prevent survey lead submissions from timing out** — In rare cases a lead submission could hang and fail with an error. This reworks the timing so submissions finish cleanly instead of dropping. (#367)

## Advertisers

- **[Task]** **Testing the new lead pre-check system in parallel** — The new pre-check runs alongside the old one to confirm they agree before switching over, a high-priority safety step. (#40)
- **[Feature]** **Verifying pre-checks advertiser by advertiser** — Each active advertiser's pre-check is validated individually before the switch, so no advertiser's setup breaks in the transition. (#41)

## Admin

- **[Task]** **Users screen comparison against the old system** — A detailed review of what the old Users area could do versus the new one, guiding which missing pieces (like bulk actions and extra columns) to add. (#80)
- **[Feature]** **Removing admin controls that do nothing** — Some settings are saved but never used anywhere. Hiding or removing them means what you see in the admin actually has an effect. (#296)

## General / Across the App

- **[Task]** **Master tracking of legacy-to-new feature matching** — An overarching effort to make sure everything the old system did is covered in New Adsmith Frontend before the old one is retired. (#319)

## Behind the Scenes

- **[Feature]** **Rolling up stats for historical reporting** — Groundwork that summarizes daily activity so historical reports load reliably. (#35)
- **[Task]** **Speeding up surveys with caching** — Adding a caching layer so surveys and offers respond faster under load. (#42)
- **[Task]** **Reviewing an old stats job** — Checking whether a legacy background stats task is still needed or can be retired. (#33)
- **[Task]** **Running new background jobs alongside the old ones** — Scheduled tasks run in parallel so results can be compared before relying on the new versions. (#43)
- **[Task]** **Gradual switch-over of low-risk scheduled jobs** — Retiring the least critical legacy jobs first, with monitoring to switch back if needed. (#44)
- **[Task]** **Gradual switch-over of mid-tier scheduled jobs** — Moving the next set of stats and reporting jobs to the new system after the first tier proves stable. (#45)
- **[Task]** **Gradual switch-over of the most critical jobs** — Migrating lead processing and offer-cap tasks last, watched closely with instant rollback ready. (#46)
- **[Task]** **Documenting how to roll back safely** — Written, tested procedures to quickly revert any part of the new system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Step-by-step guides so support can resolve problems faster. (#49)
- **[Feature]** **Auto-filing tasks from Slack conversations** — An internal helper that turns discussion notes into tracked issues automatically. (#272)
- **[Task]** **Weekly progress scorecard** — An automated internal report tracking how close the new system is to matching the old one. (#323)
- **[Bug]** **Fixing offer-group counts for campaigns** — Correcting how saved offer-group lists are read so campaign counts and details display accurately. (#372)
- **[Task]** **Automated testing added to the release pipeline** — Running the full automated test suite on every release so regressions are caught before they reach you. (#376)
- **[Task]** **Cleaner, isolated automated test data** — Preventing leftover test records and data conflicts so automated checks stay reliable. (#377)
- **[Task]** **Automated testing review** — A quality audit of the automated test setup, tracking the fixes above. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
