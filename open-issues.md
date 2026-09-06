# Open Issues — Plain-Language Overview

_Last updated 2026-09-06 06:06:32 UTC · 36 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Retire an old stats job if it's no longer needed** — A review of whether an older background process for sub-ID stats is still required or can be safely switched off. (#33)
- **[Feature]** **Groundwork for faster historical reporting** — Rolls up hourly activity into daily totals behind the scenes so historical report numbers are ready and accurate. (#35)
- **[Task]** **Run new and old background jobs side by side** — New background processing runs alongside the old system so results can be compared before fully switching over, reducing the risk of disruption. (#43)
- **[Task]** **Switch over low-risk background jobs** — Retires a low-risk older background job once its replacement is proven stable, with the ability to switch back if needed. (#44)
- **[Task]** **Switch over mid-tier background jobs** — Retires several stats-related background jobs after monitoring their replacements for stability. (#45)
- **[Task]** **Switch over the most critical background jobs** — Carefully retires the most important jobs (lead processing and offer cap resets) with close monitoring and instant rollback ready. High priority. (#46)
- **[Task]** **Document how to undo a change if something goes wrong** — Clear written rollback steps for each major system so the team can recover quickly. (#48)
- **[Task]** **Troubleshooting guides for common problems** — Step-by-step guides that help the team resolve issues faster. (#49)
- **[Feature]** **Turn Slack conversations into tracked tasks** — A helper that reads chat discussions and files them as work items so action items don't get lost. (#272)
- **[Task]** **One place to track progress toward matching the old system** — An overarching tracker that rolls up all the work needed to bring New Adsmith Frontend fully in line with the legacy app. High priority. (#319)
- **[Task]** **Weekly progress report on matching the old system** — An automatically updated weekly scorecard showing how close the new platform is to full parity. (#323)
- **[Task]** **Run automated checks before changes go live** — Automated tests will run after each update so problems in the admin screens are caught early. High priority. (#376)
- **[Task]** **Keep automated test data clean** — Housekeeping so leftover test records get cleaned up and tests don't interfere with one another. (#377)
- **[Task]** **Review of the automated testing setup** — A review of the automated test suite, with the remaining follow-up items being tracked. (#379)

## Offers

- **[Bug]** **Some saved offer settings never reached the live ad** — Fixes cases where options you set on an offer weren't actually being used when the offer was shown, so what you configure matches what visitors see. High priority. (#295)
- **[Feature]** **Automatic performance predictions for new offers** — When a new offer comes in, you'll get a data-based estimate of how it's likely to perform, drawn from past offers, in place of a manual gut-check. (#322)
- **[Bug]** **Auto-registered offers now follow the same eligibility rules** — Auto-fire offers will properly respect duplicate, conflict, and address-matching checks, so offers that should be blocked no longer slip through. High priority. (#355)
- **[Bug]** **"Conflicting Offers" setting works again after editing** — Fixes a problem where the rule keeping conflicting offers apart was silently ignored for offers edited in the current admin. High priority. (#358)
- **[Feature]** **Decide the future of the unused HubSpot List ID field** — The HubSpot List ID field currently does nothing; this decides whether to build a real HubSpot connection or remove the field. (#362)

## Data Clients

- **[Feature]** **Bring back post-conversion delivery steps** — Restores the "after success" client handling from the old system so leads are delivered and redirected as before. Nearly complete. (#327)
- **[Feature]** **Restore custom pre-check validation for data clients** — Ports the older per-client pre-checks that validate leads before they're sent, so those custom rules run again on the new platform. High priority. (#338)
- **[Bug]** **Consistent lead validation across all lead paths** — Makes the UserTrue lead-validation result real for leads processed through the manual/broker path, so validation status is trustworthy everywhere. (#366)

## Surveys

- **[Feature]** **Make sure every survey design option actually works** — Confirms that each customization on the design tab is reflected in the live survey and cleans up any settings that don't do anything. (#288)
- **[Task]** **Speed up surveys** — Adds a caching layer so surveys load and respond faster for visitors. High priority. (#42)
- **[Bug]** **Prevent survey submissions from timing out** — Reworks how outside checks are run during a submission so slow third parties can't cause a hard failure. High priority. (#367)

## Dashboard & Reports

- **[Feature]** **Live "today" numbers on the dashboard** — Adds up-to-the-hour totals for impressions, clicks, leads, and revenue so today's activity is visible right away. (#34)
- **[Task]** **Investigate report numbers not matching the old system** — Compares report totals between the old and new platforms to find and fix any differences, so you can trust the figures. High priority. (#271)

## Advertisers

- **[Task]** **Safely test the new pre-ping before switching** — Runs the new pre-ping alongside the old one to confirm results match before it goes fully live. High priority. (#40)
- **[Feature]** **Check pre-ping for each advertiser** — Verifies pre-ping works correctly for every active advertiser, so lead qualification behaves as expected once switched over. High priority. (#41)

## Admin / Users

- **[Task]** **Gap review of the Users area** — A side-by-side comparison of the old and new Users screens to identify missing features (like bulk actions and role changes) and prioritize what to add. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Hides or removes settings that appear to work but have no effect, so the admin area is clearer and more trustworthy. (#296)

## Modals

- **[Feature]** **Refreshed voucher-style visitor modal** — Rebuilds the visitor pop-up to match the legacy voucher look, with a personalized header, a progress bar that updates as offers are claimed, branded offer rows, and a secure footer. (#386)

## Campaigns

- **[Bug]** **Campaign offer groups display reliably** — Fixes a data-reading issue so campaign offer groups always load correctly, even after entries were removed in the old system. High priority. (#372)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
