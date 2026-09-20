# Open Issues — Plain-Language Overview

_Last updated 2026-09-20 06:07:26 UTC · 35 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Saved offer options now reach live offers** — Several settings you save on an offer (Modal-tab options, Display URL, and certain delivery flags) weren't carrying through to what visitors actually see. This high-priority fix ensures every option either takes effect or is cleaned up so it can't mislead. (#295)
- **[Bug]** **"Conflicting Offers" rule enforced again** — When you mark offers that shouldn't appear together, that rule was being silently ignored for offers edited in the current admin. This restores the block so conflicting offers won't show side by side. (#358)
- **[Bug]** **Manually selected offers carry over correctly** — For placements using manual offer selection, the new platform showed an empty selection and the wrong offers to visitors. This fix makes your chosen offers, and their order, match what you configured. (#370)
- **[Bug]** **Auto-registering offers respect all eligibility checks** — Auto-register offers were skipping duplicate, conflict, and address de-dupe checks, so they could fire leads that should have been blocked. This applies the same safeguards used everywhere else. (#355)
- **[Feature]** **Preview your unsaved changes on placements and offers** — The Preview button will show your current in-progress edits instead of the last saved version, so you can check a change before saving it. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, new offers could get an estimated performance projection based on your own historical offer data, helping you judge them at intake. (#322)
- **[Feature]** **Decide the future of the HubSpot List ID field** — This offer field currently does nothing because there's no HubSpot connection behind it. This work decides whether to build the integration properly or remove the field so it isn't misleading. (#362)

## Data Clients & Lead Delivery

- **[Feature]** **Restore custom pre-send lead checks** — Legacy per-client validation that ran before sending a lead isn't yet active on the new platform for a large number of clients. This high-priority work ports those checks so leads are validated as before. (#338)
- **[Feature]** **Restore post-conversion delivery steps** — After-success delivery and redirect behaviors for certain clients weren't carried over. This brings them back on the new platform. (#327)
- **[Bug]** **Accurate lead-validation flag for manual and broker leads** — Leads processed through the manual/broker pipeline reported a fixed "valid" value instead of a real check result. This fix makes that flag reflect the true validation outcome. (#366)
- **[Feature]** **Verify pre-send checks for each advertiser** — Confirms every active advertiser's pre-send lead check works correctly before switching over. A high-priority step ahead of go-live. (#41)
- **[Task]** **Side-by-side test of the new pre-send checks** — Runs the new system alongside the old one on the same leads to compare results and catch any differences before switching. (#40)

## Admin & General

- **[Task]** **Keeping the new platform in step with the legacy app** — An overarching, high-priority effort that tracks every remaining gap between the old and new systems in one place until the old app is retired. (#319)
- **[Task]** **Users area gap review** — A detailed comparison of the Users screens against the legacy app to pinpoint missing pieces like bulk actions, extra filters, and login/2FA details. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Some saved settings (certain user-permission, data-client, and pre-ping options) have no actual effect. Hiding or removing them prevents confusion and false expectations. (#296)
- **[Task]** **Weekly parity scorecard** — An automatically updated weekly summary showing how close the new platform is to matching the legacy app, so progress and any slips are easy to see. (#323)

## Reports & Dashboard

- **[Feature]** **Today's live numbers on the Dashboard** — Adds up-to-the-hour impressions, clicks, leads, and revenue for the current day, in Eastern Time. (#34)
- **[Task]** **Investigate report numbers not matching the legacy system** — A high-priority look into why some Dashboard report figures differed from the old app, to find the cause and confirm the numbers are trustworthy. (#271)
- **[Feature]** **Faster, reliable historical report totals** — Behind the reports, daily totals are rolled up so historical report views load quickly and stay accurate. (#35)

## Surveys

- **[Feature]** **Design tab changes fully reflected in the live survey** — Ensures every customization you set on the Design tab actually appears in the survey visitors see, with a full audit across all entities to catch any options that aren't wired through. (#288)
- **[Task]** **Faster survey loading for visitors** — Adds a caching layer so placement settings, offers, and targeting rules load faster during a survey. A high-priority performance improvement. (#42)
- **[Bug]** **Prevent lead submissions from timing out** — When several outside checks run during a submission, a slow response could cause the whole thing to fail. This reworks the timing so submissions finish cleanly. (#367)

## Modals

- **[Feature]** **Redesigned visitor modal (voucher style)** — Rebuilds the visitor pop-up to match the legacy "voucher" look: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with "Claim Offer" and "No Thanks", and a secure "Powered by (ad)smith" footer. (#386)

## Campaigns

- **[Bug]** **Fix campaign offer-group lists showing empty** — Corrects a data-reading issue so campaign offer groups display correctly, matching a fix already applied to placements, modals, and flows. (#372)

## Behind the Scenes

- **[Task]** **Run new background jobs alongside the old ones** — Deploys the new scheduled jobs to run in parallel with the existing ones so results can be compared before anything is switched over. High priority. (#43)
- **[Task]** **Switch over the most critical background jobs** — The final, closely monitored step of moving core lead-processing and offer-cap jobs to the new system, with an immediate rollback plan ready. (#46)
- **[Task]** **Switch over secondary stats jobs** — Retires the older stats-aggregation and reporting jobs once their replacements have proven stable. (#45)
- **[Task]** **Switch over lower-risk background jobs** — Retires the hourly survey-stats job after its replacement runs cleanly. (#44)
- **[Task]** **Review whether an old stats job is still needed** — Evaluates a legacy stats job to decide whether to keep, merge, or retire it. (#33)
- **[Task]** **Document rollback procedures** — Written, tested steps to safely revert each system if something goes wrong during the switch-over. (#48)
- **[Task]** **Create troubleshooting runbooks** — Step-by-step guides for quickly handling common issues like lead-processing or stats problems. (#49)
- **[Feature]** **Turn Slack conversations into tracked tasks** — A helper that reads designated Slack discussions and automatically files or updates work items, cutting out manual note-taking. (#272)
- **[Task]** **Run the automated test suite on every release** — Ensures the admin UI's end-to-end tests run automatically after each release so regressions get caught early. High priority. (#376)
- **[Task]** **More reliable automated testing** — Adds cleanup and isolation so automated tests don't collide with each other or leave stale data behind. (#377)
- **[Task]** **Automated testing framework review** — A review of the test suite that identified several improvements, now tracked and being addressed. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
