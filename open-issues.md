# Open Issues — Plain-Language Overview

_Last updated 2026-09-08 06:07:33 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers & Placements

- **[Bug]** **Saved offer options now reach live offers** — Several options you set on an offer (like the modal-tab settings and display URL) currently never make it onto the live offer. This fix ensures the choices you save actually take effect where visitors see them. (#295)
- **[Bug]** **Manually selected offers now carry over to placements** — On placements set to show a hand-picked offer list, the live page will display the exact offers you selected, in the right order, matching the old system instead of showing the wrong or no offers. (#370)
- **[Bug]** **"Conflicting Offers" rule is actually enforced** — When you mark offers as mutually exclusive, that rule will now be honored so conflicting offers don't appear together. A high-priority fix. (#358)
- **[Bug]** **Auto-firing offers now respect duplicate and conflict checks** — Auto-register offers will follow the same duplicate, conflict, and address de-duplication rules as regular offers, preventing duplicate or conflicting leads. (#355)
- **[Bug]** **Placement tracking pixels fill in the right values** — Pixels set up using the in-app example will now insert real tracking values instead of leaving placeholder text, keeping your attribution data accurate. (#384)
- **[Feature]** **Preview your unsaved edits** — On placement and offer edit pages, the Preview button will show your current in-progress changes without forcing you to save first. (#292)
- **[Feature]** **Automated performance projection for new offers** — When a new offer comes in, you'll get a data-driven estimate of how it's likely to perform based on your historical offers, replacing the manual gut-check review. (#322)
- **[Feature]** **Decision on the HubSpot List ID field** — This offer field currently does nothing. It will either be connected to a real HubSpot integration or removed, so the form only shows controls that actually work. (#362)

## Behind the Scenes

- **[Feature]** **Faster historical reports** — A new automated process rolls up daily activity into historical totals so report queries return quickly. (#35)
- **[Task]** **Faster survey loading** — A new caching layer for the survey engine will speed up how quickly offers and placements load for visitors. High priority. (#42)
- **[Feature]** **Per-advertiser lead pre-check validation** — Each advertiser's pre-checks are being verified before the new system takes over, so nothing slips through the switch. High priority. (#41)
- **[Task]** **Side-by-side testing of the new lead pre-check system** — The new system runs in parallel with the old one to confirm the results match before it goes live. High priority. (#40)
- **[Task]** **Running new and old scheduled jobs together** — Both versions run at once so we can confirm the new ones match before retiring the old. High priority. (#43)
- **[Task]** **Retiring the most critical old scheduled jobs (final stage)** — The last and most important legacy jobs are switched off once their replacements prove stable, with an instant fallback ready. High priority. (#46)
- **[Task]** **Retiring the second batch of old scheduled jobs** — Several stats-related legacy jobs are switched off after the first batch proves stable. (#45)
- **[Task]** **Retiring the first batch of old scheduled jobs** — A low-risk survey-stats job is switched off first as a trial run. (#44)
- **[Task]** **Reviewing an old stats job** — Checking whether a legacy statistics job is still needed or can be safely retired. (#33)
- **[Task]** **Documented rollback steps** — Clear, tested procedures for undoing changes to each system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Step-by-step guides for the support team to quickly resolve common problems. (#49)
- **[Feature]** **Slack tool to capture action items** — A helper that reads Slack conversations and automatically turns identified needs into tracked to-do items, cutting out manual copy-paste. (#272)
- **[Task]** **Automated testing after each admin release** — The admin test suite will run automatically after each release to catch problems before they reach you. High priority. (#376)
- **[Task]** **Cleaner, more reliable testing** — Improving the test setup so runs don't leave behind stray data or interfere with shared information. (#377)
- **[Task]** **Test-suite review findings** — A summary of an audit of the admin test suite and the follow-up items it identified. (#379)

## Data Clients

- **[Feature]** **Custom lead-validation checks brought over** — Hundreds of clients relied on custom serve-time validation in the old system that isn't running yet. This work restores those checks so leads are validated as before. High priority. (#338)
- **[Feature]** **After-success delivery actions restored** — Post-conversion delivery and redirect behavior for certain clients is being brought over so their after-success steps work like they used to. Nearly complete. (#327)
- **[Bug]** **Real lead verification for manually entered leads** — Leads added manually or via broker will be checked against the real verification service instead of always being reported as "valid." (#366)

## Admin

- **[Task]** **Users screen gap review** — A detailed comparison of the old and new Users screens, listing missing pieces (like bulk actions and last-login info) to guide what gets added next. (#80)
- **[Feature]** **Cleaning up controls that do nothing** — Admin settings that are saved but never actually used (some user-permission toggles and data-client/pre-ping options) will be hidden or removed so screens only show controls that work. (#296)

## Reports & Dashboard

- **[Feature]** **Live "today" numbers on the Dashboard** — The Dashboard's "today" view will show up-to-the-hour impressions, clicks, leads, and revenue for the current day. (#34)
- **[Task]** **Investigating report figures that don't match the old system** — Looking into why some Dashboard report numbers differ from the legacy app, so we can pinpoint and fix the cause and you can trust the figures. High priority. (#271)

## Surveys

- **[Feature]** **Design tab choices reliably show in surveys** — Every customization you make on the Design tab will be reflected in the live survey, and all form options across entities are being checked to confirm they actually take effect. (#288)
- **[Bug]** **Survey submissions won't time out** — Fixing a case where a submission involving several outside checks could run too long and fail; submissions will complete reliably. High priority. (#367)

## General / Across the App

- **[Task]** **Master tracker for matching the old system** — A single view that rolls up all the work needed for the new platform to fully match the old one before it's retired, so progress is visible in one place. High priority. (#319)
- **[Task]** **Weekly parity scorecard** — An automated weekly report that tracks how close the new platform is to full parity with the old system. (#323)

## Modals

- **[Feature]** **Refreshed visitor offer modal** — The visitor modal will gain the richer "voucher" style: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with clear "Claim Offer" and "No Thanks" options, and a secure, branded footer. (#386)

## Campaigns

- **[Bug]** **Campaigns show their selected offer groups correctly** — Fixing a data issue so campaigns display the offer groups you selected (in the right order) instead of appearing empty. (#372)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
