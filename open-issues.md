# Open Issues — Plain-Language Overview

_Last updated 2026-09-23 06:07:13 UTC · 35 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on Placements and Offers** — You'll be able to hit Preview and see your in-progress edits right away, instead of having to save first before you can check how a change looks. (#292)
- **[Bug]** **Saved offer options that never reach the live ad** — A fix so that offer settings you configure actually take effect on what visitors see; today several saved options are quietly dropped before they reach the live experience. (#295)
- **[Feature]** **Automatic performance estimate for new offers** — When a new offer comes in, the product will project how it's likely to perform based on your own historical offer data, replacing the old manual gut-check review. (#322)
- **[Bug]** **Auto-register offers skipping duplicate and conflict checks** — A fix so auto-registering offers respect the same duplicate, conflict, and address de-dupe rules as every other offer, preventing leads that duplicate or clash with offers already shown. (#355)
- **[Bug]** **"Conflicting Offers" setting not being enforced** — A fix so the mutual-exclusion rules you set in the current admin actually take effect; right now editing that list here can silently turn the protection off. (#358)
- **[Feature]** **Decide the fate of the HubSpot List ID field** — The HubSpot List ID field on offers currently does nothing behind the scenes. This will either connect it to a real HubSpot integration or remove the field so it stops implying something it can't do. (#362)
- **[Bug]** **Manually selected offers not carried over** — A high-priority fix so placements set to Manual delivery show the exact offers (in the right order) you chose, instead of an empty selection that falls back to the wrong offer. (#370)

## Data Clients & Pre-Pings

- **[Task]** **Side-by-side pre-ping testing before switchover** — Behind-the-scenes validation running the new pre-ping checks alongside the old system to confirm they agree before the new one takes over. (#40)
- **[Feature]** **Pre-ping validation for each advertiser** — Every active advertiser's pre-ping will be checked individually so the right fields and success rules carry over correctly before go-live. (#41)
- **[Feature]** **Restore post-conversion delivery steps** — The after-success delivery and redirect behavior for certain clients is being rebuilt in New Adsmith Frontend so leads continue to be handed off correctly after a conversion. (#327)
- **[Feature]** **Bring over legacy per-client pre-ping checks** — Hundreds of data clients rely on custom serve-time validation that doesn't run yet in the new platform; this high-priority work ports those checks so leads are screened the same way as before. (#338)
- **[Bug]** **Real lead validation in the manual/broker lead pipeline** — A fix so manually entered and broker leads are checked against the real validation service instead of always being marked valid, keeping lead quality signals honest across the board. (#366)

## Surveys

- **[Task]** **Faster survey loading** — Behind-the-scenes speed work that caches placement and offer settings so surveys respond more quickly for visitors. (#42)
- **[Feature]** **Design tab settings that fully show up in the survey** — Every customization option on the Design tab will actually appear in the live survey, with a full check across entities to catch any option that isn't currently connected. (#288)
- **[Bug]** **Survey submissions timing out on slow third parties** — A fix so lead submissions don't get cut off when several outside services are slow at once, giving visitors a clean result instead of an error. (#367)

## Reports / Dashboard

- **[Feature]** **Today's numbers in near real time** — The Dashboard's "today" view will show up-to-date impressions, clicks, leads, and revenue for the current day, in Eastern Time. (#34)
- **[Feature]** **Accurate historical totals in reports** — Daily numbers will be rolled up automatically so historical report figures stay complete and reliable. (#35)
- **[Task]** **Investigate report numbers not matching the old system** — A high-priority look into why some dashboard report figures differ from the legacy app, to pin down the cause and confirm the numbers can be trusted. (#271)

## General / Across the App

- **[Task]** **Users screen feature review** — A documented comparison of the old Users management against the new one, listing what's still missing (like bulk role changes and last-login info) so the gaps can be prioritized. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Settings that look like they control something but currently have no effect (certain user permissions, data-client, and pre-ping options) will be hidden or removed so the admin area is trustworthy and clear. (#296)
- **[Task]** **Overall progress toward matching the old system** — An ongoing tracking effort that rolls up every "catch up to the legacy app" item into a single view of how close the new platform is to full parity. (#319)

## Modals

- **[Feature]** **Refreshed voucher-style visitor modal** — The visitor modal will match the polished legacy look: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with clear "Claim Offer" and "No Thanks" actions, and a trust footer. (#386)

## Behind the Scenes

- **[Task]** **Review an old stats job** — Checking whether a legacy stats process is still needed or can be retired now that newer reporting covers it. (#33)
- **[Task]** **Slack-to-issue helper** — Exploring a Slack assistant that turns meeting conversations into tracked work items automatically, reducing manual copy-paste. (#272)
- **[Task]** **Run new and old scheduled jobs together** — Deploying the new background jobs alongside the existing ones so results can be compared before anything is switched off. (#43)
- **[Task]** **Retire low-risk background jobs first** — Turning off the least critical legacy scheduled jobs once their replacements prove stable. (#44)
- **[Task]** **Retire mid-tier background jobs** — Switching off the next set of legacy stats jobs after the earlier ones run cleanly. (#45)
- **[Task]** **Retire the most critical background jobs last** — Carefully switching off the core lead-processing and offer-cap jobs, with close monitoring and a fast rollback plan. (#46)
- **[Task]** **Document how to roll back safely** — Writing and testing step-by-step recovery procedures for each production system. (#48)
- **[Task]** **Create troubleshooting guides** — Preparing quick-reference guides for common issues so problems can be resolved faster. (#49)
- **[Task]** **Weekly parity progress report** — An automated weekly scorecard that tracks how close the new platform is to the old one, so the team can watch the trend. (#323)
- **[Bug]** **Fix a data-parsing issue on Campaigns** — Correcting a behind-the-scenes flaw that can cause a campaign's offer-group list to come back empty, matching a fix already applied elsewhere. (#372)
- **[Task]** **Run automated UI tests during release** — Wiring the existing end-to-end test suite into the release process so admin-screen regressions are caught automatically. (#376)
- **[Task]** **Keep test data from cluttering the shared environment** — Adding automatic cleanup and isolation so leftover test records don't build up or interfere with real data. (#377)
- **[Task]** **Automated-testing health review** — A summary of findings from auditing the UI test suite, tracking the fixes needed to make it a reliable safety net. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
