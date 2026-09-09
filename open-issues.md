# Open Issues — Plain-Language Overview

_Last updated 2026-09-09 06:07:37 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Retiring the most critical background jobs last** — The oldest, most important automated jobs (lead processing and offer-cap resets) will be switched over to their new replacements last and watched closely, so nothing critical is disrupted. (#46)
- **[Task]** **Running new lead pre-checks in parallel first** — Before switching over, the new lead pre-check system runs alongside the old one so we can confirm they produce matching results. (#40)
- **[Task]** **Rolling out new background jobs side-by-side** — New scheduled jobs will run at the same time as the old ones for a while, so we can confirm everything matches before relying on them. (#43)
- **[Task]** **Retiring a batch of older stats jobs** — Several older automated stats jobs will be turned off after their replacements prove stable, with a week of monitoring. (#45)
- **[Task]** **Retiring an older survey-stats job** — An older survey-stats job will be switched off once its replacement is proven reliable. (#44)
- **[Task]** **Reviewing an old stats job** — Checking whether an older background stats job is still needed or can be safely retired. (#33)
- **[Task]** **Documenting how to safely undo changes** — Writing clear steps to quickly revert each system if a problem appears, so recovery is fast. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Creating step-by-step guides so the team can quickly resolve common problems like lead-processing or stats hiccups. (#49)
- **[Bug]** **Preventing lead submissions from timing out** — When a lead relies on several outside services at once, we'll make sure it doesn't stall, so visitors get a clean result instead of an error. (#367)
- **[Bug]** **Correcting how campaign offer lists are read** — Fixing a data-reading issue so campaign offer-group counts display correctly. (#372)
- **[Task]** **A tracker for matching the old system** — An overall effort that measures, feature by feature, how closely New Adsmith Frontend matches the older system it's replacing. (#319)
- **[Task]** **A weekly "matching" scorecard** — An automatic weekly report card showing how much of the old system's behavior the new platform now matches. (#323)
- **[Feature]** **Turning conversations into tracked tasks** — A helper that reads team conversations and automatically files the action items, cutting out manual note-taking. (#272)
- **[Task]** **Automated checks before changes go live** — The full behind-the-scenes test suite will run automatically after each update, catching admin-screen problems before users see them. (#376)
- **[Task]** **More reliable automated testing** — Improving cleanup of leftover test data so automated testing stays dependable. (#377)
- **[Task]** **Improving the testing setup** — Tracking a set of fixes to make automated testing more trustworthy overall. (#379)

## Offers

- **[Bug]** **All saved offer settings will actually take effect** — Some offer options you set weren't reaching the live offer display; this fix makes every configured option apply as expected. (#295)
- **[Bug]** **Auto-firing offers will respect duplicate and conflict rules** — Offers that register automatically currently skip some duplicate and conflict checks. They'll be brought in line with the same rules other offers follow. (#355)
- **[Bug]** **Conflicting-offer rules will work again** — For offers edited in the current admin, the "these offers can't show together" setting had quietly stopped working; this restores it. (#358)
- **[Feature]** **Predicting how a new offer will perform** — Instead of a manual gut-check, you'll get a data-driven estimate of how a new offer is likely to perform, based on your past offers. (#322)
- **[Feature]** **Deciding the future of the HubSpot List ID field** — The HubSpot List ID field currently does nothing; we'll either build a real HubSpot connection for it or remove the unused field. (#362)

## Placements

- **[Bug]** **Hand-picked offers will show on manual placements** — On manual-delivery placements, the manually selected offer list wasn't carried over; this restores the correct offers in the correct order. (#370)
- **[Feature]** **Preview will reflect your unsaved edits** — On placement and offer edit pages, Preview will show your current in-progress changes so you can check them without saving first. (#292)
- **[Bug]** **Tracking-pixel placeholders will fill in correctly** — Fixing a mismatch in pixel placeholder wording so attribution data is sent cleanly instead of corrupted. (#384)

## Data Clients

- **[Feature]** **Restoring custom lead pre-checks for clients** — Hundreds of clients rely on custom lead pre-checks that don't yet run on the new platform; this brings that validation back. (#338)
- **[Feature]** **Restoring post-conversion delivery behavior** — Certain clients' after-success delivery steps weren't carried over; this ports them so those hand-offs work again. (#327)
- **[Bug]** **Real lead validation in the manual/broker pipeline** — Leads entered manually or via brokers currently always report "passed"; this makes their validation genuine. (#366)

## Reports / Dashboard

- **[Task]** **Confirming report numbers match the old system** — Investigating why some dashboard report figures didn't line up with the older system, and confirming they agree. (#271)
- **[Feature]** **Accurate "today" numbers on the dashboard** — The dashboard's "today" view will show accurate, up-to-the-hour totals for impressions, clicks, leads, and revenue. (#34)
- **[Feature]** **Faster, accurate historical report numbers** — Daily data will be summarized behind the scenes so historical reports load quickly and read correctly. (#35)

## Surveys

- **[Feature]** **Every design option will show in the live survey** — All the customizations you set on the design tab will actually appear to visitors, with a check that no option is left disconnected. (#288)
- **[Task]** **Faster-loading surveys** — Behind-the-scenes speed improvements so surveys load more quickly for visitors. (#42)

## Admin / General

- **[Feature]** **Removing settings that do nothing** — Admin controls that are saved but never actually used will be hidden or removed, so screens only show settings that genuinely work. (#296)
- **[Task]** **Reviewing the Users area against the old system** — A full comparison of the Users screen to identify missing capabilities like bulk actions, login history, and two-factor status. (#80)

## Advertisers

- **[Feature]** **Verifying each advertiser's lead pre-check** — Confirming that every active advertiser's lead pre-check works correctly before switching to the new system. (#41)

## Modals

- **[Feature]** **A polished voucher-style visitor modal** — The visitor offer modal will be redesigned to match the richer legacy look, with a personalized header and voucher number, a color-coded progress bar, branded offer rows, and secure-branding footer. (#386)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
