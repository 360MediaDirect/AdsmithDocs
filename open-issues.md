# Open Issues — Plain-Language Overview

_Last updated 2026-09-13 06:08:53 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Saved offer options that never take effect will actually work** — Several settings you can save on an offer (including the Modal-tab options, Display URL, and some delivery flags) currently never reach the live offer. This fix makes those saved options actually apply. (#295)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check review, you'll get a data-driven estimate of how a new offer is likely to perform, based on your own past offers and their results. (#322)
- **[Bug]** **Auto-register offers will respect duplicate and conflict rules** — Auto-registering offers will be held to the same duplicate, conflict, and address de-duplication checks as regular offers, so they won't fire a lead that conflicts with or duplicates one already shown. (#355)
- **[Bug]** **The Conflicting Offers setting will actually be enforced** — For offers edited in the new admin, the Conflicting Offers list currently does nothing. This fix makes it properly stop those offers from appearing together as intended. (#358)
- **[Feature]** **Decide the future of the HubSpot List ID field** — This field currently has no effect anywhere. The team will either build a real HubSpot connection behind it or remove it so it no longer misleads you. (#362)

## General / Across the App

- **[Feature]** **Hide admin controls that don't do anything** — Certain settings (a few user permission toggles, a couple of Data-Client options, and a Pre-Ping option) that currently have no real effect will be removed or hidden so they don't imply features that aren't there. (#296)
- **[Task]** **Master tracking of old-vs-new feature matching** — A high-priority coordination effort that tracks every remaining gap between the old system and New Adsmith Frontend, so nothing is missed before the old app is retired. (#319)
- **[Task]** **Weekly progress scorecard for matching the old system** — A regularly updated report showing how close New Adsmith Frontend is to fully matching the old app across features, behavior, and data. (#323)
- **[Task]** **Review of missing features in the Users area** — A documentation review comparing the old Users screen with the new one to catch features still to be added, such as bulk actions, last-login, and two-factor status. (#80)
- **[Bug]** **Campaign offer groups won't come back empty** — A fix ensuring Campaigns correctly read their saved offer-group lists, so counts and selections display properly instead of appearing blank. (#372)

## Placements

- **[Bug]** **Manually selected offers now carry over correctly** — Placements set to manual offer delivery will show the same chosen offers, in the same order, as the old system, instead of appearing empty and defaulting to the wrong offer. (This one is essentially wrapped up.) (#370)
- **[Feature]** **Preview your unsaved changes on placements and offers** — The Preview button will show the edits you've just made before saving, instead of only showing the last saved version. (#292)
- **[Bug]** **Pixel placeholders will match the on-screen instructions** — Following the pixel setup example shown in the placement form will now produce correct tracking values instead of broken or blank ones. (#384)

## Data Clients

- **[Feature]** **Custom pre-ping checks restored for data clients** — Custom lead-validation steps that ran in the old system for hundreds of data clients will run again on the new platform, so those checks aren't silently skipped. (#338)
- **[Feature]** **After-conversion delivery steps restored** — Post-conversion redirect and delivery behavior from the old system is being brought over so affected clients keep working after a lead converts. (#327)
- **[Bug]** **Consistent lead validation for manually entered leads** — Leads added through the manual/broker path will get the same real lead-validation as survey leads, instead of always being reported as valid. (#366)

## Dashboard & Reports

- **[Task]** **Investigating report numbers that don't match the old system** — High-priority work to find why some Dashboard report figures differ from the old app and confirm the numbers can be trusted. (#271)
- **[Feature]** **Live "today" numbers on the Dashboard** — The Dashboard will show up-to-the-hour impressions, clicks, leads, and revenue for the current day. (#34)
- **[Feature]** **More reliable historical reporting** — Behind-the-scenes summarizing of daily stats so historical reports stay accurate and load dependably. (#35)

## Surveys

- **[Feature]** **Design-tab options fully reflected in the live survey** — Every customization you set on the Design tab will actually appear in the live survey, with a review across all screens to catch any options that currently don't take effect. (#288)
- **[Bug]** **Preventing survey submissions from timing out** — A fix to stop lead submissions that rely on several outside services from occasionally hitting a hard time limit and failing. (#367)

## Modals

- **[Feature]** **Redesigned visitor offer modal** — The visitor modal will gain the richer "voucher" look from the old system: a personalized header with a voucher number, a color-coded progress bar for each offer, branded offer rows with clear Claim buttons, and a secure footer. (#386)

## Behind the Scenes

- **[Task]** **Testing the new lead pre-check system in parallel** — Running the new lead pre-check alongside the old one and comparing results to make sure it behaves correctly before switching over. (#40)
- **[Feature]** **Verifying pre-checks for each advertiser** — Confirming every active advertiser's lead pre-check works correctly before the switchover. (#41)
- **[Task]** **Speeding up survey delivery** — Adding a caching layer so surveys and offer rules load faster during real-time serving. (#42)
- **[Task]** **Running new scheduled jobs alongside the old ones** — Deploying the new automated background jobs to run in parallel with the old ones while they're monitored for accuracy. (#43)
- **[Task]** **Retiring the first batch of old scheduled jobs** — Turning off the lowest-risk old background jobs once the new versions prove stable. (#44)
- **[Task]** **Retiring the next batch of old scheduled jobs** — Turning off additional old stats and reporting jobs after the first batch is confirmed stable. (#45)
- **[Task]** **Retiring the most critical old scheduled jobs** — Carefully switching off the last and most important background jobs, with the ability to roll back instantly if needed. (#46)
- **[Task]** **Reviewing an old stats job for removal** — Checking whether a legacy stats job is still needed or can be safely retired. (#33)
- **[Task]** **Documented recovery steps** — Writing and testing clear rollback procedures for each production system in case something needs to be reverted. (#48)
- **[Task]** **Troubleshooting guides for support** — Creating step-by-step guides for handling common issues so problems can be resolved quickly. (#49)
- **[Feature]** **A helper that turns Slack notes into tracked tasks** — An internal tool to automatically capture action items from Slack conversations and file them as tracked work items. (#272)
- **[Task]** **Automated testing after each release** — Setting up the full automated test suite to run automatically after each update, catching problems before they reach users. (#376)
- **[Task]** **Cleaner, more reliable automated testing** — Improving how automated tests handle their data so leftover test records are cleaned up and results stay dependable. (#377)
- **[Task]** **Tracking improvements to the automated test suite** — An overview issue coordinating several fixes to make the automated testing more trustworthy. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
