# Open Issues — Plain-Language Overview

_Last updated 2026-09-21 06:09:02 UTC · 35 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Check whether an old stats job is still needed** — Behind-the-scenes review to decide if an older reporting job can be retired now that newer reporting handles the same work. No visible change for you. (#33)
- **[Task]** **Trial the new lead pre-check system alongside the old one** — High priority. The new system that checks leads before they're sent will run in parallel with the existing one so results can be compared before switching over, protecting accuracy during the transition. (#40)
- **[Task]** **Speed up the survey engine with a caching layer** — High priority behind-the-scenes work to make surveys load and respond faster for visitors. (#42)
- **[Task]** **Run new scheduled jobs in production alongside the old ones** — High priority. The new automated background jobs will run side by side with the current ones so they can be verified before the old ones are turned off. (#43)
- **[Task]** **Retire the first batch of old scheduled jobs** — Once the new survey-stats job proves stable, the matching old one will be switched off, with the ability to turn it back on if needed. (#44)
- **[Task]** **Retire the second batch of old scheduled jobs** — Continues the safe handover of stats and reporting jobs to the new system, monitored for a week afterward. (#45)
- **[Task]** **Retire the most critical old scheduled jobs last** — High priority. The most important jobs (lead processing and offer cap resets) are switched over last and watched closely, with an immediate fallback ready. (#46)
- **[Task]** **Write step-by-step recovery plans** — Documented procedures for quickly reverting each production system if something goes wrong, so issues can be handled calmly and consistently. (#48)
- **[Task]** **Create troubleshooting guides for common issues** — Reference guides for handling problems like lead-processing or stats hiccups, helping the team resolve incidents faster. (#49)
- **[Feature]** **A Slack helper that turns conversations into tracked tasks** — An assistant that reads designated Slack channels and automatically files action items so nothing from meetings slips through the cracks. (#272)
- **[Task]** **A weekly progress report on matching the legacy system** — A living scorecard that tracks, week by week, how close New Adsmith Frontend is to fully matching the old app, so progress and any slips are visible at a glance. (#323)
- **[Task]** **Run the automated admin tests automatically** — High priority. The large suite of automated checks for the Admin area will run after each release so problems in navigation, forms, and reports are caught before you see them. (#376)
- **[Task]** **Keep automated test data clean and separated** — Adds a routine cleanup so leftover test records don't pile up and interfere with the shared testing environment. (#377)
- **[Task]** **Review of the automated admin test suite** — A completed audit of the automated checks that identified several improvements, now being addressed as their own items. (#379)

## Offers

- **[Bug]** **Some saved offer settings never reach the live offer** — A number of options you can set on an offer (including Modal-tab fields, Display URL, and several data settings) currently aren't carried through to what visitors actually see. This fix makes each saved setting either take effect or be cleaned up so nothing is misleading. (#295)
- **[Bug]** **Manually selected offers now show correctly** — On placements set to manual delivery, the chosen offers (and their order) weren't carrying over, so the wrong offers appeared. This restores your hand-picked selections so live results match what you configured. (#370)
- **[Bug]** **Auto-registering offers will respect all eligibility rules** — Offers that fire automatically were skipping duplicate, conflict, and address de-duplication checks. Fixing this prevents auto offers from firing when they shouldn't, matching the old app's behavior. (#355)
- **[Bug]** **"Conflicting Offers" rule will actually be enforced** — For offers edited in the current admin, the mutual-exclusion setting was quietly doing nothing. This ensures conflicting offers are properly kept apart at serve time. (#358)
- **[Feature]** **Preview offers and placements with your unsaved edits** — The Preview button will show your current in-progress changes instead of the last saved version, so you can check edits before committing them. (#292)
- **[Feature]** **Automatic performance estimate for new offers** — An exploratory tool to project how a new offer is likely to perform based on your historical offer data, replacing the manual gut-check review. (#322)
- **[Feature]** **Decide the future of the HubSpot List ID field** — This offer field currently does nothing because there's no HubSpot connection built. This item decides whether to build that integration or remove the unused field to avoid confusion. (#362)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back file-based pre-ping checks for clients** — High priority. Custom pre-send validation that many clients relied on in the old system isn't running on the new platform yet. This ports it over so those checks are applied again before leads go out. (#338)
- **[Feature]** **Validate each advertiser's pre-send checks before switching** — High priority. Every active advertiser's pre-send lead check will be tested and confirmed correct before the new system takes over. (#41)
- **[Feature]** **Restore post-conversion delivery steps for clients** — Certain "after success" delivery and redirect steps from the old system weren't carried over. This brings them back as a reusable, configurable option. (#327)
- **[Bug]** **Real lead validation for manually submitted leads** — Leads sent through the manual/broker path were always marked as validated even when they weren't checked. This adds genuine validation so the result reflects reality. (#366)

## Reports & Dashboard

- **[Task]** **Investigate why dashboard numbers differ from the old app** — High priority. During testing, dashboard report figures didn't match the legacy system. This traces where the difference comes from and confirms the numbers can be trusted. (#271)
- **[Feature]** **Live "today" numbers on the dashboard** — The dashboard's "today" view will pull up-to-the-hour figures for impressions, clicks, leads, and revenue, with correct time-zone handling. (#34)
- **[Feature]** **Reliable historical reporting totals** — Behind-the-scenes rollups keep past-period numbers accurate and fast to load when you look back over time. (#35)

## Admin & General

- **[Task]** **Full comparison of the Users screen vs. the old app** — A documented review of what the Users area is missing compared to the legacy version (like bulk actions, last-login, and two-factor status), guiding what gets added next. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Some settings (certain user-permission, data-client, and pre-ping options) are saved but have no effect. These will be hidden or removed so the admin screens only show controls that actually work. (#296)
- **[Task]** **Master checklist for matching the old app** — High priority. A single tracking hub that rolls up all the work needed to fully match the legacy system, so overall progress is visible in one place instead of scattered across many items. (#319)

## Surveys

- **[Feature]** **Every design option shows up in the live survey** — An end-to-end check to make sure each design and form option you set is actually reflected in what visitors see, with any unused options fixed or removed. (#288)
- **[Bug]** **Prevent slow lead submissions from timing out** — When several outside services respond slowly at once, a lead submission could be cut off before finishing. This reworks the process to stay within safe limits so submissions complete reliably. (#367)

## Campaigns

- **[Bug]** **Fix campaign offer groups not loading correctly** — High priority. In certain cases a campaign's offer groups could read as empty and silently show nothing. This applies the same fix already used elsewhere so campaign offer groups load and display properly. (#372)

## Modals

- **[Feature]** **Refreshed "voucher-style" visitor modal** — The visitor modal will match the legacy voucher look: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with clear Claim/No Thanks buttons, and a trusted-branding footer. (#386)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
