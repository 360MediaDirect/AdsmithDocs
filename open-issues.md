# Open Issues — Plain-Language Overview

_Last updated 2026-09-16 06:07:13 UTC · 35 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach the live offer** — Several options you set on an offer (including modal-tab settings, display URL, and a few advertiser-side flags) aren't currently carried through to what visitors actually see. This fix makes sure the choices you save are the choices that go live — or clearly removes options that do nothing. (#295)
- **[Bug]** **Auto-register offers skip important eligibility checks** — Offers that fire automatically on page load are bypassing duplicate, conflict, and address de-duplication rules that normal offers respect. Once fixed, these offers will honor the same guardrails, so an advertiser won't receive a lead that duplicates or conflicts with another. (#355)
- **[Bug]** **"Conflicting Offers" rule silently stops working after editing** — When you set or edit an offer's conflicting-offers list in the current admin, the mutual-exclusion rule quietly stops being enforced. This fix restores that protection so conflicting offers can't appear together. (#358)
- **[Bug]** **Manually selected offers weren't carrying over correctly** — On placements using manual offer selection, the chosen offer list could come across empty, causing the wrong offers to show. This fix ensures your selected offers (and their order) display exactly as configured. (#370)
- **[Feature]** **Preview offers and placements with your unsaved edits** — The Preview button will show your in-progress changes instead of only the last saved version, so you can check how an edit looks before committing to it. (#292)
- **[Feature]** **Automatic performance projections for new offers** — New offers could be scored against your historical offer data to estimate how they're likely to perform, giving you a data-based gut-check at intake instead of relying on a manual review. (#322)
- **[Feature]** **Clean up the offer "HubSpot List ID" field** — This field currently doesn't connect to anything. We'll either build a real HubSpot connection behind it or remove it, so the form only shows options that actually do something. (#362)

## Dashboard & Reports

- **[Task]** **Investigate report numbers not matching the old system** — During testing, dashboard report totals didn't line up with the legacy app. We're tracing exactly where the difference comes from and confirming the new reports are accurate. A high-priority effort. (#271)
- **[Feature]** **Live "today" numbers on the Dashboard** — The Dashboard will show up-to-the-hour impressions, clicks, leads, and revenue for the current day, correctly handled in Eastern Time. (#34)
- **[Feature]** **Reliable historical report totals** — Behind-the-scenes rollups will keep daily totals accurate over time so your longer-range reports stay dependable. (#35)

## Data Clients

- **[Feature]** **Bring back after-conversion delivery steps** — Certain post-conversion delivery and redirect behaviors from the old system weren't carried over. This restores them so clients that depend on those steps keep working. Nearly complete. (#327)
- **[Feature]** **Restore custom pre-check validation for data clients** — Hundreds of data clients relied on a legacy custom validation step that isn't running on the new platform yet. This ports that logic so leads are validated the same way before delivery. A high-priority item. (#338)
- **[Bug]** **Report the real UserTrue validation result on manual/broker leads** — In the manual and broker lead path, the UserTrue check currently always reports "true" instead of the real outcome. This wires in genuine validation so exports and deliveries reflect what actually happened. (#366)

## Surveys

- **[Feature]** **Make every Design-tab option actually take effect** — We're reviewing all customization options across entities to confirm each one is fully connected from the form to what visitors see, and fixing any that don't currently do anything. (#288)
- **[Bug]** **Prevent survey submissions from timing out** — When several outside checks run one after another, a submission can occasionally take too long and fail with an error. This work keeps submissions comfortably within safe time limits so visitors get a clean result. A high-priority fix. (#367)

## Admin Area

- **[Task]** **Users screen gap review vs. the old system** — A detailed comparison of the Users area against the legacy app, identifying missing pieces like bulk role changes, last-login and two-factor status, and more, so the new Users screen can catch up. Mostly documented. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — A few settings (certain user permissions, some data-client fields, and a pre-ping option) are saved but never actually used. Hiding or removing them prevents confusion and avoids implying access controls that aren't really in effect. (#296)

## General / Across the App

- **[Task]** **Ongoing effort to match everything the old system does** — A single tracking effort that rolls up all the work needed to reach and hold feature-for-feature parity with the legacy app before it's retired, so progress can be seen in one place. A high-priority initiative. (#319)
- **[Bug]** **Fix offer-group counts on Campaigns** — A data-reading quirk could cause a campaign's offer groups to come back empty or wrong. This applies the same fix used elsewhere so campaign offer-group counts display correctly. (#372)

## Modals

- **[Feature]** **Redesigned "voucher" style visitor modal** — The visitor modal will get a richer look inspired by the legacy design: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with clear "Claim Offer" and "No Thanks" actions, and a trusted footer. (#386)

## Behind the Scenes

- **[Feature]** **Automatically turn conversations into tracked work items** — Exploring a helper that reads team chat and files or updates work items automatically, reducing manual note-taking. (#272)
- **[Task]** **Weekly progress tracking on old-vs-new parity** — An automated weekly summary that measures how close the new platform is to the old one, so slips are caught early. (#323)
- **[Task]** **Run the automated admin test suite on every release** — The large automated check of the admin screens isn't currently run automatically; wiring it into the release process will catch regressions before they reach users. A high-priority maintenance item. (#376)
- **[Task]** **Keep automated tests clean and reliable** — Improvements so the automated tests don't leave behind stray test data or interfere with each other, making results more trustworthy. (#377)
- **[Task]** **Review of the automated test framework** — A summary of findings from auditing the admin test suite, tracking the fixes that came out of it. (#379)
- **[Feature]** **Faster survey experience through caching** — Setting up a caching layer so survey and offer settings load more quickly for visitors. A high-priority infrastructure task. (#42)
- **[Task]** **Validate the new pre-check system before switching over** — Running the new lead pre-check system alongside the old one and comparing results to confirm it behaves correctly. A high-priority step. (#40)
- **[Feature]** **Confirm pre-checks work for each advertiser** — Verifying every active advertiser's pre-check behaves correctly before the new system takes over. A high-priority step. (#41)
- **[Task]** **Roll out new scheduled jobs alongside the old ones** — Running the new background jobs in parallel with the existing ones and watching for any differences before fully switching. A high-priority step. (#43)
- **[Task]** **Carefully retire old background jobs, most critical last** — A staged plan to switch off the legacy scheduled jobs in tiers (least critical first, most critical last) with monitoring at each step. (#44, #45, #46)
- **[Task]** **Document how to roll back safely** — Writing clear rollback steps for each production system so any issue can be reversed quickly. (#48)
- **[Task]** **Create troubleshooting guides for common issues** — Preparing step-by-step guides for the most common operational hiccups so problems get resolved faster. (#49)
- **[Task]** **Review an older stats job for retirement** — Checking whether a legacy statistics job is still needed or can be safely removed. (#33)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
