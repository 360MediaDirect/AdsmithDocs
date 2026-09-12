# Open Issues — Plain-Language Overview

_Last updated 2026-09-12 06:07:00 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Saved offer settings not reaching the live ad** — Several options you set on an offer (like the Modal-tab fields, Display URL, and certain data-handling flags) aren't currently carried through to what visitors actually see. This makes sure the choices you save take effect. (#295)
- **[Feature]** **Automatic performance projections for new offers** — When a new offer comes in, New Adsmith Frontend will estimate how it's likely to perform based on your past offers and results, giving a data-driven gut-check in place of a manual review. (#322)
- **[Bug]** **Auto-registered offers now respect the same rules** — Auto-register offers will be held to the same duplicate, conflict, and address-matching checks as every other offer, so they won't fire when they shouldn't. (#355)
- **[Bug]** **"Conflicting Offers" setting works again** — Offers whose conflicting-offer list was set in the current admin weren't actually being kept apart. This restores that protection so mutually exclusive offers don't show together. (#358)
- **[Feature]** **Decide the future of the HubSpot List ID field** — The HubSpot List ID on offers currently does nothing behind the scenes. This work decides whether to build a real HubSpot connection or remove the unused field. (#362)

## Reports / Dashboard

- **[Feature]** **"Today" numbers on the Dashboard** — Adds up-to-the-hour impressions, clicks, leads, and revenue for the current day so your Dashboard reflects today's activity. (#34)
- **[Feature]** **Faster, reliable historical reporting** — Daily totals will be rolled up automatically so historical reports load quickly and stay accurate. (#35)
- **[Task]** **Making report numbers match the old system** — Investigating why some Dashboard report figures differ from the legacy app so the numbers you see can be trusted. (#271)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery steps** — Bringing over the "after-success" delivery and redirect steps for clients that had them in the old system, so post-conversion handoffs work as before. (#327)
- **[Feature]** **Restoring custom lead pre-checks** — Re-adds the custom per-client lead screening that ran in the old system for hundreds of clients, so leads are validated the same way before delivery. (#338)
- **[Bug]** **Real lead verification for manually processed leads** — Leads sent through the manual/broker path will be checked against the real verification service instead of always reporting "verified". (#366)

## Placements

- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show your current, unsaved edits instead of forcing you to save first. (#292)
- **[Bug]** **Manually selected offers now carry over** — Manual-delivery placements were showing the wrong offers (or none) because the hand-picked offer list wasn't migrating. This restores the correct selected offers and their order. (#370)
- **[Bug]** **Pixel codes that match the instructions** — The on-screen example for setting up a pixel didn't match what the system actually understood, which corrupted tracking data. Pixels set up per the instructions will now fire correctly. (#384)

## Advertisers

- **[Task]** **Safely testing the new lead pre-check system** — Running the new pre-check alongside the old one to confirm they match before switching over, so lead screening stays reliable. (#40)
- **[Feature]** **Per-advertiser pre-check validation** — Verifying each active advertiser's lead pre-check before the switch, so every advertiser's rules keep working correctly. (#41)

## Surveys

- **[Feature]** **Every design option shows up in the survey** — A full audit so that each customization you set on the Design tab actually appears in the live survey, with no options that quietly do nothing. (#288)
- **[Bug]** **Preventing timeouts during lead submission** — Lead submissions that check several outside services can currently run long enough to fail abruptly. This keeps them within safe limits so they finish gracefully. (#367)

## Modals

- **[Feature]** **New voucher-style visitor modal** — A refreshed modal with a personalized header and voucher number, a progress bar that updates as offers are claimed, branded offer rows, and a "Secure" footer, matching the polished legacy look. (#386)

## General / Across the App

- **[Task]** **Users area feature review** — Comparing the Users area against the old system to spot missing capabilities (like bulk actions and last-login info) and plan what to add. (#80)
- **[Feature]** **Removing controls that do nothing** — Hiding or removing admin settings that currently have no effect (certain user permissions, data-client, and pre-ping options) so the screens only show controls that actually work. (#296)

## Behind the Scenes

- **[Task]** **Reviewing an old stats job** — Checking whether a legacy statistics process is still needed or can be retired. (#33)
- **[Task]** **Speeding up the survey engine** — Adding a caching layer so placements and offers load faster for visitors. (#42)
- **[Task]** **Running new scheduled jobs alongside the old ones** — Deploying updated background jobs in parallel to confirm they match before anything is switched over. (#43)
- **[Task]** **Retiring older background jobs (group 3)** — Turning off a lower-risk set of legacy scheduled jobs after the new versions prove stable. (#44)
- **[Task]** **Retiring more background jobs (group 2)** — Switching off the next set of legacy scheduled jobs once the earlier group runs cleanly. (#45)
- **[Task]** **Retiring the most critical background jobs (group 1)** — Carefully switching off the core lead-processing and offer-cap jobs last, with quick rollback ready if needed. (#46)
- **[Task]** **Documented rollback plans** — Writing step-by-step recovery procedures for each core system in case something needs to be reversed. (#48)
- **[Task]** **Troubleshooting guides** — Creating quick-reference guides for handling common operational issues. (#49)
- **[Feature]** **Turning conversations into tracked tasks** — A helper that reads team chat and automatically files or updates work items, reducing manual note-taking. (#272)
- **[Task]** **Overall old-to-new tracking** — An umbrella effort that tracks how completely New Adsmith Frontend matches the old app until the old app is retired. (#319)
- **[Task]** **Weekly progress scorecard** — An automatic weekly report showing how close the new platform is to fully matching the old one. (#323)
- **[Bug]** **Correct offer counts on campaigns** — Fixing a data-reading issue that could make a campaign's offer groups show up as empty. (#372)
- **[Task]** **Automated testing in the release process** — Running the full automated screen-test suite after each update so admin-screen problems are caught before they reach you. (#376)
- **[Task]** **Cleaner, more reliable automated tests** — Preventing leftover test data and scheduling overlaps so automated checks stay dependable. (#377)
- **[Task]** **Automated testing review** — Findings from an audit of the automated test suite, tracked as follow-up improvements. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
