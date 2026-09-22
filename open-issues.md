# Open Issues — Plain-Language Overview

_Last updated 2026-09-22 06:07:48 UTC · 35 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved edits on Placements and Offers** — When you're editing a placement or offer, the Preview button will reflect the changes you've made but not yet saved, so you can check your work before committing it. (#292)
- **[Bug]** **Saved offer settings that weren't reaching the live ad** — Several options you set on an offer weren't actually being applied to what visitors see. This fix makes sure each saved setting is honored (or the unused ones are cleaned up). (#295)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, New Adsmith Frontend will estimate how a new offer is likely to perform based on your own historical offer data. (#322)
- **[Bug]** **Auto-registering offers now follow the same eligibility rules** — Offers that fire automatically will now respect the same duplicate, conflict, and address de-duplication checks as regular offers, preventing unwanted or duplicate leads. (#355)
- **[Bug]** **"Conflicting Offers" rule being enforced again** — Offers edited in the current admin had their conflicting-offers restriction silently ignored. This restores enforcement so mutually exclusive offers stay exclusive. (#358)
- **[Feature]** **Decide the future of the HubSpot List ID field** — This field currently does nothing. The work will either build a real HubSpot connection behind it or remove the unused field to avoid confusion. (#362)
- **[Bug]** **Manually selected offers now carry over correctly** — Placements set to Manual delivery were showing the wrong offers (or none) because the selected-offer list wasn't migrated. Your manual selections and their order will now match what you set. (#370)

## Data Clients & Pre-Pings

- **[Feature]** **Post-conversion delivery steps restored** — The "after success" delivery and redirect actions from the old system are being brought over so leads finish the same way they used to. (#327)
- **[Feature]** **Custom pre-submission checks restored** — Legacy custom checks used by hundreds of clients will run again before a lead is sent, matching the old behavior. (#338)
- **[Bug]** **Accurate validation flag in the manual/broker lead path** — Leads processed through the manual and broker pathway will show their real validation result instead of an always-"true" placeholder. (#366)
- **[Feature]** **Per-advertiser pre-check verification** — Each advertiser's pre-submission check will be confirmed to work correctly before it's switched over to the new system. (#41)
- **[Task]** **Side-by-side testing of the new pre-checks** — Behind-the-scenes testing that runs the new pre-submission checks alongside the old ones to confirm they behave identically before the switch. (#40)

## Reports & Dashboard

- **[Feature]** **Today's live numbers on the Dashboard** — You'll see up-to-the-hour impressions, clicks, leads, and revenue for the current day. (#34)
- **[Task]** **Investigating report figures that don't match the old system** — We're comparing reports between the old and new platforms over a fixed date range to find and fix any differences so you can trust the numbers. (#271)

## Admin & Users

- **[Task]** **Users screen gap review** — A comparison of the old and new Users areas to catch missing capabilities (like bulk role changes and select-all) and plan them in. (#80)
- **[Feature]** **Removing admin controls that don't do anything** — Certain settings currently have no effect. They'll be hidden or removed so you're not misled into thinking they change something. (#296)

## Surveys

- **[Feature]** **Making every survey design option actually take effect** — A full audit to ensure each customization on the Design tab shows up in the live survey, with no settings that quietly do nothing. (#288)

## Modals

- **[Feature]** **Redesigned visitor modal in the voucher style** — The visitor modal will get the polished legacy look: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with a "Claim Offer" button, and a "Powered by (ad)smith / Verified Secure" footer. (#386)

## General / Across the App

- **[Task]** **Overall old-to-new parity tracking** — An umbrella effort to make sure the new platform reaches and holds full feature and data parity with the old system before it's retired. (#319)

## Behind the Scenes

- **[Task]** **Review of an older stats job** — Checking whether an outdated stats process is still needed or can be retired. No user-visible change. (#33)
- **[Feature]** **Rolling up historical stats** — Summarizing daily stats in the background so historical reporting stays fast. (#35)
- **[Task]** **Faster surveys through caching** — A performance improvement so survey and offer information loads more quickly. (#42)
- **[Task]** **Running new automated jobs alongside the old ones** — The new scheduled jobs will run in parallel with the old ones so we can confirm they match before switching over. (#43)
- **[Task]** **Retiring the first batch of old scheduled jobs** — Turning off a low-risk group of old background jobs once their replacements prove stable. (#44)
- **[Task]** **Retiring the next batch of old scheduled jobs** — Switching off additional old stats jobs after the earlier batch runs cleanly. (#45)
- **[Task]** **Retiring the most critical old scheduled jobs** — Carefully switching off the highest-priority background jobs last, with the ability to revert immediately if needed. (#46)
- **[Task]** **Documenting how to revert safely** — Written steps for quickly rolling back each system if a problem appears. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Reference guides so the team can resolve issues quickly. (#49)
- **[Feature]** **Internal Slack-to-task tool** — A helper that turns Slack conversations into tracked work items automatically, reducing manual copy-paste. (#272)
- **[Task]** **Weekly parity scorecard** — An automated weekly report that tracks how closely the new platform matches the old one. (#323)
- **[Bug]** **Preventing lead submissions from timing out** — Making sure lead submissions that involve several outside services finish cleanly instead of getting cut off. (#367)
- **[Bug]** **Fixing empty offer lists in Campaigns** — A data-reading fix so campaign offer groups load correctly instead of appearing empty. (#372)
- **[Task]** **Running automated tests automatically** — Setting up the automated test suite to run after each update so problems are caught early. (#376)
- **[Task]** **More reliable automated testing** — Keeping test data tidy and results dependable by improving how the test suite runs. (#377)
- **[Task]** **Automated-test suite audit** — A review of the automated tests to strengthen coverage and reduce false failures. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
