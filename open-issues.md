# Open Issues — Plain-Language Overview

_Last updated 2026-09-11 06:07:11 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach live offers** — A number of options you set on an offer aren't currently being applied to the live experience. Once fixed, the choices you make in the offer form (including modal and display settings) will actually take effect. (#295)
- **[Bug]** **Auto-registering offers now respect duplicate and conflict rules** — Offers that fire automatically currently skip the duplicate, conflict, and address de-duplication checks that normal offers follow. This fix makes them behave consistently, so an auto-offer won't slip through against those rules. (#355)
- **[Bug]** **"Conflicting Offers" rule will work again for offers edited in the new admin** — This mutual-exclusion setting is quietly being ignored for any offer saved through the new interface. The fix restores enforcement so conflicting offers won't show together. (#358)
- **[Bug]** **Campaign offer-group counts will display correctly** — Certain campaigns can show an empty or missing offer-group count due to how the underlying list is read. This fix makes those counts accurate again. (#372)
- **[Feature]** **AI-assisted performance projection for new offers** — Instead of a manual gut-check, new offers could get an automatic estimate of likely performance based on your historical offer data, helping you gauge an offer at intake. (#322)
- **[Feature]** **Decision on the HubSpot List ID field** — This field currently does nothing because there's no HubSpot connection behind it. The team will either build the integration or remove the field, so what you see in the form matches reality. (#362)

## Behind the Scenes

- **[Task]** **Trial run of the new offer pre-check system** — The new pre-ping (pre-submission) checks will run alongside the current one and be compared, so accuracy is proven before switching over. (#40)
- **[Task]** **Faster survey performance with a caching layer** — Frequently used placement and offer data will be kept ready-to-serve, making surveys respond more quickly. (#42)
- **[Task]** **New automated background jobs go live alongside the old ones** — The replacement scheduled jobs will run in parallel with the existing ones and be monitored for a clean handover. (#43)
- **[Task]** **Phased retirement of legacy scheduled jobs (part 1)** — The lowest-risk background jobs will be switched to their new versions first, with monitoring in place. (#44)
- **[Task]** **Phased retirement of legacy scheduled jobs (part 2)** — The next set of stats-related background jobs moves to their new versions after the first batch proves stable. (#45)
- **[Task]** **Phased retirement of legacy scheduled jobs (part 3, critical)** — The most important jobs, including lead processing and offer-cap resets, switch over last with close monitoring and instant rollback ready. (#46)
- **[Task]** **Documented rollback plans** — Clear step-by-step recovery procedures for each major system, so any issue can be reversed quickly. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Reference guides for the support team to resolve problems like lead-processing or stats hiccups faster. (#49)
- **[Task]** **Review of an older stats job** — A quick evaluation of whether one legacy stats job is still needed or can be retired. (#33)
- **[Feature]** **Turn conversations into tracked work automatically** — An assistant that reads discussion notes and files them as tracked tasks, reducing manual copy-and-paste. (#272)
- **[Task]** **Single view of legacy-to-new progress** — An overarching tracker that rolls up all the "match the old system" work into one clear progress picture. (#319)
- **[Task]** **Weekly progress scorecard** — An automatically updated weekly summary showing how close the new platform is to fully matching the legacy system. (#323)
- **[Task]** **Automated safety testing after each release** — The full set of admin-interface tests will run automatically after updates, catching regressions before they reach you. (#376)
- **[Task]** **Cleaner, more reliable automated testing** — Improvements so automated tests don't leave behind stray test data or interfere with each other, making results more trustworthy. (#377)
- **[Task]** **Automated-testing improvement plan** — A summary of testing gaps and fixes to keep the safety net dependable. (#379)

## Placements

- **[Bug]** **Manually selected offers now carry over correctly** — On placements using manual offer selection, the chosen offers weren't transferring to the new platform, so the wrong offers appeared. This is fixed so your selected offers and their order display as configured. (#370)
- **[Bug]** **Tracking pixels will fire with the correct values** — The in-app pixel example used a format the system didn't recognize, so pixels sent broken or placeholder values. This fix makes the documented format work cleanly, protecting your attribution data. (#384)
- **[Feature]** **Preview your unsaved edits** — On placement and offer edit pages, Preview will show your current in-progress changes instead of only the last saved version, so you can check edits before saving. (#292)

## Data Clients

- **[Feature]** **Post-conversion delivery steps restored** — Custom "after success" client handling from the legacy system is being brought over, so all active clients keep the delivery behavior they rely on. (#327)
- **[Feature]** **Custom pre-submission checks restored for data clients** — Legacy per-client validation that runs before a lead is delivered is being ported so those checks work again on the new platform. (#338)
- **[Bug]** **Lead validation applied consistently across lead paths** — One lead-processing path wasn't running real UserTrue validation and always reported a fixed value. This fix makes it report the true validation result, matching the other path. (#366)

## Reports & Dashboard

- **[Feature]** **Live "today" numbers on the Dashboard** — The Dashboard will show up-to-date figures for the current day, including impressions, clicks, leads, and revenue, in the correct time zone. (#34)
- **[Feature]** **Accurate historical report totals** — Daily data will be rolled up automatically so historical reports stay complete and consistent over time. (#35)
- **[Task]** **Investigating report numbers vs. the legacy system** — A focused review to find why some dashboard report figures didn't match the old system and to confirm the numbers can be trusted. (#271)

## Surveys

- **[Feature]** **Design tab settings reflected in the live survey** — A review to make sure every customization option on the Design tab actually shows up in the survey visitors see, with no settings that quietly do nothing. (#288)
- **[Bug]** **More reliable lead submissions** — When several outside checks run during a submission, they could occasionally add up to a timeout and fail the request. This fix keeps submissions within safe time limits so they finish cleanly. (#367)

## Admin & Users

- **[Task]** **Users area gap review vs. the legacy system** — A detailed comparison of the Users area against the old system to identify missing features like bulk actions and login details, guiding what gets added next. (#80)
- **[Feature]** **Removing controls that don't do anything** — Several admin settings are saved but not actually used. They'll be hidden or removed so the interface only shows controls that truly work. (#296)

## Advertisers

- **[Feature]** **Per-advertiser pre-check validation** — Each active advertiser's pre-submission checks will be verified individually before switching over, ensuring their field mapping and success rules work correctly. (#41)

## Modals

- **[Feature]** **Redesigned visitor modal in the "voucher" style** — The visitor modal will gain the richer legacy look: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with clear Claim buttons, and a trusted footer badge. (#386)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
