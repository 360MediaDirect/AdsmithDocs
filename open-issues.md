# Open Issues — Plain-Language Overview

_Last updated 2026-09-10 06:07:50 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Retire duplicate stats jobs where possible** — We're checking whether an older behind-the-scenes stats process is still needed or can be safely switched off, keeping reporting simpler and cleaner. (#33)
- **[Task]** **Safety-test the new lead pre-checking before switching over** — We'll run the new and old lead pre-check systems side by side to confirm the new one matches the old one before it goes live, so nothing changes unexpectedly for advertisers. (#40)
- **[Feature]** **Confirm pre-checks work for every advertiser** — We're verifying each active advertiser's lead pre-check individually so leads are validated correctly once the new system takes over. (#41)
- **[Task]** **Set up faster performance for surveys** — Adding a caching layer so surveys and offers load and respond more quickly for visitors. (#42)
- **[Task]** **Roll out new automated background jobs in parallel** — The new scheduled jobs will run alongside the current ones so we can confirm they produce identical results before relying on them. (#43)
- **[Task]** **Gradually switch over background jobs (first batch)** — Turning off the first, lowest-risk set of old background jobs now that their replacements are proven stable. (#44)
- **[Task]** **Gradually switch over background jobs (second batch)** — Retiring the next group of older stats and reporting jobs after a week of monitoring their replacements. (#45)
- **[Task]** **Gradually switch over the most critical background jobs (final batch)** — The most important jobs — lead processing and offer cap resets — will be moved last, with close monitoring and an instant fallback if anything looks off. (#46)
- **[Task]** **Write clear "undo" procedures for each system** — Documenting how to quickly revert any production system if a problem appears, so recovery is fast and reliable. (#48)
- **[Task]** **Create troubleshooting guides for common issues** — Step-by-step guides for the support team to resolve lead, stats, offer-cap, and pre-check problems quickly. (#49)
- **[Feature]** **Turn Slack chats into tracked work items automatically** — A helper that reads designated Slack channels and files action items as tracked issues, reducing manual note-taking after meetings. (#272)
- **[Task]** **Weekly progress scorecard for the old-to-new transition** — An automatic weekly report shows how much of the old system the new platform has matched, giving everyone a single clear view of migration progress. (#323)
- **[Bug]** **Prevent slow lead submissions from timing out** — When several outside services respond slowly at once, a lead submission could get cut off. This fix keeps submissions within safe time limits so they finish cleanly instead of failing. (#367)
- **[Task]** **Run the automated admin tests regularly** — Our full suite of automated checks on the Admin area will run automatically after each update, catching problems before they reach users. (#376)
- **[Task]** **Keep test data from cluttering the practice environment** — Adding an automatic cleanup so leftover test records don't build up and interfere with future testing. (#377)
- **[Task]** **Overall review of the automated Admin tests** — A summary of improvements to make our automated Admin testing more reliable and trustworthy. (#379)

## Offers

- **[Bug]** **Saved offer settings not reaching the live experience** — Several offer options you set in the form (including some Modal-tab and display settings) currently don't carry through to what visitors see. This fixes the gap so your saved settings actually take effect. (#295)
- **[Feature]** **Predict how a new offer will perform** — Instead of a manual gut-check, you'll get an automatic performance estimate for a new offer based on your own historical offer data, helping you evaluate offers at intake. (#322)
- **[Bug]** **Auto-registered offers skipping duplicate and conflict checks** — Some automatic offers can fire even when they duplicate or conflict with another offer already shown. This fix applies the same eligibility rules used everywhere else, matching the old system. (#355)
- **[Bug]** **"Conflicting Offers" rule silently not working** — When you set conflicting offers in the current admin, the rule wasn't actually being enforced. This fix makes those mutual-exclusion settings work as expected. (#358)
- **[Feature]** **Decide the fate of the unused HubSpot List ID field** — This offer field currently does nothing because there's no HubSpot connection built. We'll either build the integration properly or remove the field so it's not misleading. (#362)
- **[Bug]** **Manually selected offers not carried over from the old system** — On manual-delivery placements, the list of chosen offers was coming across empty, so the wrong offers displayed. This fix preserves your selected offers and their order. (#370)
- **[Bug]** **Fix offer counts for campaigns with edited lists** — A data-reading issue could make campaign offer-group counts come back empty. This fixes the count so campaigns show the correct offers. (#372)

## Behind the Scenes / Data & Reliability

*(Grouped separately for clarity — these support Reports and the Dashboard.)*

## Reports & Dashboard

- **[Feature]** **See today's numbers on the Dashboard** — The Dashboard's "today" view will show live, up-to-the-hour impressions, clicks, leads, and revenue in the correct time zone. (#34)
- **[Feature]** **Faster, accurate historical report totals** — Daily numbers are rolled up behind the scenes so historical reports load quickly and stay consistent. (#35)
- **[Task]** **Make sure report numbers match the old system** — We're investigating why some Dashboard report figures differed from the legacy app, pinpointing the cause, and confirming the numbers line up. (#271)

## Data Clients

- **[Feature]** **Restore post-conversion delivery steps** — Certain after-success client behaviors from the old system are being brought over, so those clients continue receiving leads correctly. (#327)
- **[Feature]** **Bring over custom per-client lead pre-checks** — Hundreds of data clients rely on custom pre-checks that aren't running on the new platform yet. This restores that per-client validation at the right moment. (#338)
- **[Bug]** **Real lead validation for manually processed leads** — Leads sent through the manual/broker pipeline weren't being validated properly. This connects real validation so those leads reflect their true status. (#366)

## Placements

- **[Feature]** **Preview your unsaved changes** — On placement and offer edit pages, the Preview button will show your current in-progress edits instead of only the last saved version, so you can check changes before saving. (#292)
- **[Bug]** **Fix pixel placeholder codes so tracking works** — The placement pixel help text listed placeholder codes that didn't actually work, corrupting tracking data. We'll make the system accept the documented codes and fix the guidance so pixels fire correctly. (#384)

## Admin & Users

- **[Task]** **Compare the old and new Users areas** — A detailed review of the Users screen to identify which legacy features (like bulk actions, last-login, and 2FA status) are missing, so we can prioritize adding them. (#80)
- **[Feature]** **Remove admin controls that do nothing** — A few settings currently appear to control access or behavior but actually have no effect. We'll hide or remove them so the admin screens don't imply options that don't exist. (#296)

## Surveys

- **[Feature]** **Make every survey Design option actually take effect** — We're checking that each customization option on the Design tab is reflected in the live survey, and fixing any option that isn't fully connected. (#288)

## Modals

- **[Feature]** **Refreshed voucher-style visitor modal** — The visitor modal will match the richer legacy "voucher" look: a personalized header with a voucher number, a per-offer progress bar that recolors as offers are claimed, branded offer rows with clear Claim/No Thanks buttons, and a trusted footer. (#386)

## General / Across the App

- **[Task]** **Keep the new platform in step with the old one** — An ongoing effort that tracks every gap between the legacy system and the new platform in one place, so nothing is missed before the old system is retired. (#319)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
