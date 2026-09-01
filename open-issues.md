# Open Issues — Plain-Language Overview

_Last updated 2026-09-01 06:08:01 UTC · 38 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Saved offer options don't reach the live ad** — Several options you fill in on an offer (certain Modal-tab fields, Display URL, and some data-client flags) are being dropped before they reach the live widget, so they never take effect. This ensures each saved setting is either honored on live offers or cleanly removed. (#295)
- **[Bug]** **Auto-register offers skip duplicate and conflict checks** — Auto-register offers can currently fire even when they duplicate or conflict with an offer already shown to a visitor. This applies the same eligibility and de-duplication rules used for regular offers, so you won't get unwanted duplicates. (#355)
- **[Bug]** **"Conflicting Offers" setting quietly stops working** — When you set conflicting offers in the current admin, the rule silently does nothing when offers are served. This makes that mutual-exclusion setting take effect again. (#358)
- **[Feature]** **Decision on the HubSpot List ID field** — The HubSpot List ID on offers currently does nothing because there's no HubSpot connection behind it. This decides whether to build that integration or remove the unused field so the form only shows controls that work. (#362)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, you'll get a data-driven estimate of how a new offer is likely to perform, grounded in your own historical offer data. (#322)

## Data Clients & Pre-Pings

- **[Feature]** **Restore custom serve-time validation (pre-ping)** — Custom validation used by hundreds of data clients isn't running on the new platform yet, so those checks silently don't happen. This brings that validation over so leads are checked as they were before. High priority. (#338)
- **[Feature]** **Bring back after-success delivery steps** — Post-conversion delivery and redirect behavior for certain clients hasn't been carried over. This rebuilds it so those clients keep working after a lead succeeds. (#327)
- **[Bug]** **Real lead validation in the manual/broker lead path** — The manual lead path currently reports a validation result that's always "true." This wires in genuine validation so the reported outcome is accurate. (#366)
- **[Feature]** **Verify each advertiser's pre-ping before switch-over** — Every active advertiser's pre-ping will be tested and its field mapping confirmed before going live, so nothing breaks at cutover. High priority. (#41)
- **[Task]** **Side-by-side pre-ping testing** — The new pre-ping runs alongside the old one and results are compared, to confirm they match before the switch. High priority. (#40)

## Dashboard / Reports

- **[Feature]** **Live "today" numbers on the Dashboard** — You'll see up-to-date impressions, clicks, leads, and revenue for the current day, in the correct time zone. (#34)
- **[Task]** **Investigate report numbers that don't match the old system** — Confirm why some dashboard report figures differ from the legacy app on the same data, pin down the cause, and fix it so you can trust the numbers. High priority. (#271)
- **[Feature]** **Notes on Placement, Advertiser, and Offer dashboards** — You'll be able to add short, categorized notes to these records and see a recent-notes roll-up on the main Dashboard. (#382)

## Placements

- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show your current edits without forcing you to save first. (#292)
- **[Bug]** **Manually selected offers now carry over** — Manual-delivery placements were showing the wrong or no offers because the hand-picked offer list wasn't migrated. This restores the correct selected offers and their order. (#370)
- **[Bug]** **Pixel example matches what actually works** — The in-app pixel example used a macro format the system didn't recognize, which corrupted tracking values. This aligns the help text and the system so pixels fire cleanly. (#384)

## General / Across the App

- **[Task]** **Parity tracking with the legacy app** — An overarching effort to make sure the new platform matches everything the old app could do, tracked in one place so nothing slips through. High priority. (#319)
- **[Task]** **Users screen gap analysis** — A review documenting what the old Users area could do that the new one can't yet (bulk actions, extra filters, last-login, and more) so the gaps can be prioritized. (#80)
- **[Feature]** **Remove admin controls that do nothing** — Some settings look like they control access or behavior but currently have no effect. These will be hidden or removed so the admin only shows controls that actually work. (#296)

## Surveys

- **[Feature]** **Design tab settings actually apply to the live survey** — Every customization on the Design tab will be reflected in what visitors see, plus an audit across all entities to catch any options that aren't fully connected. (#288)

## Flows

- **[Task]** **Fix Flow form styling** — Parts of the Flow form look unstyled or broken (plain text boxes, unstyled color pickers, fields stacking oddly). This gives the form the same polished look as the Placement and Modal forms. (#152)

## Modals

- **[Feature]** **Voucher-style visitor modal redesign** — The visitor modal will be redesigned to match the polished legacy "voucher" style: a personalized header with a voucher number, a progress bar that recolors as offers are claimed, branded offer rows with clear Claim/No Thanks options, and a trust footer. (#386)

## Behind the Scenes

- **[Task]** **Speed up surveys with caching** — Behind-the-scenes caching to make survey responses faster. High priority. (#42)
- **[Bug]** **Prevent lead-submission timeouts** — Rework how lead submissions call outside services so slow third parties can't cause a submission to time out and fail. High priority. (#367)
- **[Bug]** **Fix Campaign offer-group data reading** — Correct a data-reading issue so campaign offer groups always load properly. (#372)
- **[Task]** **Run automated UI tests automatically** — Turn on the automated end-to-end tests in the release process so UI problems are caught before reaching users. High priority. (#376)
- **[Task]** **Tidy up automated test data** — Add automatic cleanup and better isolation so leftover test records don't clutter shared data. (#377)
- **[Task]** **Automated test suite review** — A review of the automated testing setup, with follow-up fixes tracked. (#379)
- **[Feature]** **Historical stats roll-up** — Automatically summarize daily activity for faster historical reporting. (#35)
- **[Task]** **Review an old stats job** — Check whether an older stats process is still needed or can be retired. (#33)
- **[Task]** **Run new scheduled jobs alongside the old ones** — Deploy the new scheduled jobs to run in parallel so results can be compared safely. High priority. (#43)
- **[Task]** **Retire old scheduled jobs (first batch)** — Turn off a low-risk group of legacy scheduled jobs once their replacements prove stable. (#44)
- **[Task]** **Retire old scheduled jobs (second batch)** — Turn off the next group of legacy scheduled jobs and monitor for a week. (#45)
- **[Task]** **Retire the most critical scheduled jobs last** — Carefully switch off the most important legacy jobs, with close monitoring and instant rollback ready. High priority. (#46)
- **[Task]** **Document rollback procedures** — Write clear steps to safely revert each major system if something goes wrong. (#48)
- **[Task]** **Create troubleshooting runbooks** — Step-by-step guides for quickly resolving common operational issues. (#49)
- **[Task]** **Weekly parity scorecard** — An automated weekly snapshot showing how close the new platform is to matching the legacy app. (#323)
- **[Feature]** **Slackbot to file issues from conversations** — A helper that turns action items from Slack chats into tracked issues automatically, saving manual copy-paste. (#272)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
