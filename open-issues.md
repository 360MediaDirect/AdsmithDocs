# Open Issues — Plain-Language Overview

_Last updated 2026-09-07 06:08:59 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes
- **[Task]** **Review an old stats-collection routine** — Checking whether a legacy background data job is still needed or can be retired. No visible change; general housekeeping. (#33)
- **[Task]** **Speed up survey loading** — Adding a caching layer so surveys and their offers respond faster for visitors. (#42)
- **[Task]** **Run new automated jobs alongside the old ones** — The new background jobs will run in parallel with the existing ones so we can confirm they produce matching results before switching over. (#43)
- **[Task]** **Begin retiring old background jobs (first stage)** — Turning off a low-risk set of legacy scheduled jobs once their replacements are proven stable, with the ability to switch back if needed. (#44)
- **[Task]** **Retire more background jobs (second stage)** — Switching off the next group of legacy stats jobs after the first stage runs cleanly. (#45)
- **[Task]** **Retire the most critical background jobs (final stage)** — Carefully turning off the last and most important legacy jobs, monitored closely with an instant rollback plan. (#46)
- **[Task]** **Write recovery procedures** — Documenting how to safely undo each major system change if something goes wrong. (#48)
- **[Task]** **Create troubleshooting guides** — Step-by-step guides for the support team to resolve common issues quickly. (#49)
- **[Feature]** **Slackbot that turns conversations into tracked tasks** — A helper that reads designated Slack channels and automatically files action items, reducing manual note-taking. (#272)
- **[Bug]** **Prevent lead submissions from timing out** — A reliability fix so that when several outside checks run slowly at once, a lead submission still finishes cleanly instead of erroring. (#367)
- **[Bug]** **Fix offer lists that fail to load on campaigns** — Correcting how certain saved offer selections are read, so campaign offer counts and lists appear correctly. (#372)
- **[Task]** **Automatically run the full test suite** — The complete set of end-to-end checks will run on its own after each update, catching problems before they reach users. (#376)
- **[Task]** **Make automated tests more reliable and self-cleaning** — Improving test isolation and clearing out leftover test data so results are trustworthy. (#377)
- **[Task]** **Test-suite review findings** — A summary of gaps found while auditing the automated test setup, tracked so each is addressed. (#379)

## Offers
- **[Bug]** **Saved offer settings will actually reach the live ad** — Several saved offer options weren't being carried through to what visitors see; the fix ensures each setting takes effect or is cleaned up if truly unused. (#295)
- **[Feature]** **Automatic performance projections for new offers** — When a new offer comes in, you'll get a data-driven estimate of how it's likely to perform based on past offers, replacing the old manual gut-check. (#322)
- **[Bug]** **Auto-registering offers will respect duplicate and conflict rules** — These auto-firing offers currently skip some eligibility checks; the fix makes them follow the same duplicate, conflict, and address checks as every other offer. (#355)
- **[Bug]** **"Conflicting Offers" rule will be enforced again** — Editing this list in the new admin had quietly stopped the rule from working; the fix restores proper mutual-exclusion between conflicting offers. (#358)
- **[Feature]** **Decide the future of the HubSpot List ID field** — This field currently does nothing behind the scenes. We'll either build the HubSpot connection it implies or remove the field so it doesn't mislead. (#362)

## General / Across the App
- **[Task]** **Users area gap review** — Comparing the old and new Users management screens to find missing pieces (bulk actions, extra filters, and more) so we can close the gaps. (#80)
- **[Feature]** **Remove admin controls that do nothing** — Cleaning up settings and permission toggles that look functional but have no real effect, so the admin area is trustworthy and less confusing. (#296)
- **[Task]** **Master tracker for old-vs-new feature parity** — A single high-priority hub that rolls up every "does the new app match the old one" item so overall progress is visible in one place. (#319)
- **[Task]** **Weekly parity scorecard** — A living report, refreshed weekly, that shows how close the new platform is to matching the legacy system across features, behavior, and data. (#323)

## Placements
- **[Feature]** **Preview unsaved changes on placements and offers** — The Preview button will show your current edits as they'd appear live, without forcing you to save first. (#292)
- **[Bug]** **Manually selected offers now carry over correctly** — On manual-delivery placements, the chosen offers (and their order) were coming across empty after migration; they now match the legacy setup. (#370)
- **[Bug]** **Tracking pixels using the documented format now work** — Pixels set up following the in-app example were sending garbled values to advertisers; the fix makes the documented placeholders fill in cleanly. (#384)

## Data Clients
- **[Feature]** **Restore after-conversion delivery behaviors** — Bringing across the post-success delivery and redirect steps for clients that rely on them, so nothing is lost in the move to the new platform. (#327)
- **[Feature]** **Restore custom pre-send checks for data clients** — Re-adding the per-client validation that ran before delivering a lead, so hundreds of clients keep the checks they depend on. (#338)
- **[Bug]** **Real lead validation in the manual lead pipeline** — Leads sent through the manual/broker path will be validated against the real verification service instead of always reporting "valid." (#366)

## Reports & Dashboard
- **[Feature]** **Today's live numbers on the Dashboard** — You'll see up-to-the-hour impressions, clicks, leads, and revenue for the current day, in the correct time zone. (#34)
- **[Feature]** **Faster historical reporting** — Behind-the-scenes daily roll-ups keep past-date reports quick and accurate to look up. (#35)
- **[Task]** **Investigate report numbers that don't match the legacy system** — A high-priority look into why some dashboard figures differ from the old app, pinpointing the cause and confirming or fixing the numbers. (#271)

## Advertisers
- **[Task]** **Test new pre-send checks against the current system** — Running the new lead pre-checks side by side with the existing ones to confirm they behave identically before switching. (#40)
- **[Feature]** **Verify pre-send checks for each advertiser** — Confirming that every active advertiser's pre-send validation and field mapping works correctly before go-live. (#41)

## Surveys
- **[Feature]** **Make every survey design option actually apply** — Auditing the design settings so that each customization you choose is reflected in the live survey, with no options that quietly do nothing. (#288)

## Modals
- **[Feature]** **Redesign the visitor pop-up to the voucher style** — The visitor modal will match the legacy "voucher" look: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with clear "Claim Offer" and "No Thanks" actions, and a secure-branding footer. (#386)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
