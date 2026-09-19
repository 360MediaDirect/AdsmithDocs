# Open Issues — Plain-Language Overview

_Last updated 2026-09-19 06:06:42 UTC · 35 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Manually selected offers now carry over** — For Manual-delivery placements, the exact offers you picked (and their order) will display correctly, matching the legacy app instead of showing the wrong or empty set. (#370)
- **[Bug]** **"Conflicting Offers" rule works again** — Offers you marked as mutually exclusive in the current admin will actually be enforced, so conflicting offers won't show together anymore. A high-priority fix. (#358)
- **[Bug]** **Auto-register offers respect all eligibility rules** — Auto-registered offers will properly honor duplicate, conflict, and address de-duplication checks, so they won't fire when they shouldn't. A high-priority fix. (#355)
- **[Bug]** **Saved offer settings reach the live experience** — Fixing cases where certain options you saved on an offer weren't being applied on the live widget. A high-priority fix. (#295)
- **[Feature]** **Preview shows your unsaved edits** — When previewing a placement or offer while editing, you'll see your current changes immediately, without having to save first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — New offers could receive an estimated performance forecast based on your historical data, replacing the old manual gut-check review. (#322)
- **[Feature]** **Decide the fate of the HubSpot List ID field** — The offer-level HubSpot List ID field currently does nothing; this will either build the real integration or remove the unused field. (#362)

## Reports & Dashboard

- **[Task]** **Matching report numbers between old and new** — Investigating why some Dashboard report figures differ from the legacy system, so you can trust the numbers. A high-priority investigation. (#271)
- **[Feature]** **Today's numbers on the Dashboard** — The Dashboard's "today" view will show current-day impressions, clicks, leads, and revenue in near real time. (#34)
- **[Feature]** **Faster, reliable historical reporting** — Behind the scenes, daily totals are rolled up so historical reports load consistently. (#35)

## Pre-Pings

- **[Feature]** **Custom pre-ping rules for data clients restored** — Bringing legacy per-client pre-ping validation over to the new platform so those custom checks actually run. A high-priority item. (#338)
- **[Task]** **Safe, side-by-side testing of the new pre-ping** — Running the new pre-ping alongside the old one to confirm identical behavior before switching over. A high-priority item. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Confirming each advertiser's pre-ping works correctly before go-live. A high-priority item. (#41)

## Data Clients

- **[Feature]** **After-success delivery steps restored** — Post-conversion delivery and redirect behaviors from the legacy system are being ported so leads finish correctly. (#327)
- **[Bug]** **Real lead validation in the manual/broker lead flow** — Leads processed through the manual and broker path will report genuine validation results instead of an always-"true" placeholder. (#366)

## Admin / Users

- **[Task]** **Users area feature gap review** — A comparison of the legacy Users management against the new Admin area, guiding which features to add next (like bulk actions and last-login info). (#80)
- **[Feature]** **Removing controls that do nothing** — Admin settings that currently have no effect will be hidden or removed to avoid confusion and false expectations. (#296)

## Surveys

- **[Feature]** **Design settings reflected in the live survey** — Every customization on the Design tab will actually appear in the survey, with a full audit to fix any options that aren't connected. (#288)

## Modals

- **[Feature]** **Redesigned voucher-style visitor modal** — The visitor modal will gain the richer legacy look: a personalized header with a voucher number, a per-offer progress bar that updates as offers are claimed, branded offer rows, and a secure footer. (#386)

## Behind the Scenes

- **[Task]** **Faster survey loading** — Adding a caching layer so surveys and their offers load more quickly for visitors. (#42)
- **[Bug]** **Preventing lead-submission timeouts** — Making sure lead submission stays within its time limit even when several outside services respond slowly. A high-priority fix. (#367)
- **[Bug]** **Correct offer lists for campaigns** — Fixing how campaign offer groups are read so offers aren't accidentally dropped due to a data-format quirk. (#372)
- **[Task]** **One place to track legacy-to-new parity** — An overarching effort to ensure the new platform matches everything the legacy system did before it's retired. (#319)
- **[Task]** **Weekly parity progress report** — An automated weekly scorecard that tracks how close the new platform is to full parity with the legacy system. (#323)
- **[Task]** **Running new background jobs alongside the old ones** — Scheduled tasks run in parallel with the existing system to confirm results match before switching. (#43)
- **[Task]** **Retiring legacy background jobs, step one** — Turning off the first, lower-risk batch of legacy scheduled tasks once their replacements prove stable. (#44)
- **[Task]** **Retiring legacy background jobs, step two** — Turning off the next batch of legacy stats-related tasks after a monitoring period. (#45)
- **[Task]** **Retiring the most critical background jobs** — Carefully switching off the highest-priority legacy tasks (like lead processing and offer-cap resets), with rollback ready. A high-priority, critical step. (#46)
- **[Task]** **Rollback plans for each system** — Documenting how to quickly revert each major system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Creating step-by-step guides for handling problems like lead-processing or stats failures. (#49)
- **[Task]** **Automated testing on every release** — Wiring the admin area's end-to-end tests to run automatically so regressions are caught before they reach users. A high-priority item. (#376)
- **[Task]** **Cleaner, more reliable automated tests** — Adding cleanup and isolation so automated tests don't leave stray data behind or interfere with one another. (#377)
- **[Task]** **Automated test review follow-ups** — Addressing findings from a review of the admin area's automated test suite. (#379)
- **[Task]** **Review of an old stats job** — Checking whether a legacy background stats process is still needed or can be retired. (#33)
- **[Feature]** **Auto-filing tasks from chat** — Exploring a Slack assistant that turns conversation action items into tracked work items automatically. (#272)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
