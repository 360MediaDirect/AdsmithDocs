# Open Issues — Plain-Language Overview

_Last updated 2026-09-02 06:07:54 UTC · 37 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Bug]** **Saved offer settings not reaching live offers** — Several options you set on an offer (including the Modal-tab fields, Display URL, and certain delivery flags) currently don't carry through to what visitors actually see. This work makes sure the settings you save either take effect or are removed so nothing misleads you. (#295)
- **[Bug]** **Conflicting-offers rule will be enforced again** — When you list conflicting offers on an offer today, that mutual-exclusion rule is being silently ignored. Once fixed, offers you mark as conflicting will correctly be kept from showing together. (#358)
- **[Bug]** **Auto-registering offers will respect the same eligibility checks** — These offers can currently fire even when they duplicate or conflict with an offer already shown, or repeat a postal address an advertiser would reject. This brings them in line with the checks every other offer follows. (#355)
- **[Feature]** **Decision on the HubSpot List ID field** — This offer field currently does nothing behind the scenes. The team will either build a real HubSpot connection or remove the field so it no longer implies something that isn't happening. (#362)
- **[Feature]** **Preview unsaved changes on placements and offers** — The Preview button will show your current, in-progress edits instead of only the last saved version, so you can check a change before saving it. (#292)
- **[Feature]** **Automatic performance projection for new offers** — Instead of a manual gut-check, new offers could get a data-driven estimate of how they're likely to perform, based on your own historical offer results. (#322)

## Surveys
- **[Feature]** **Design-tab options fully reflected in the live survey** — Every customization you make on the Design tab will actually appear in the survey visitors see, plus a review to catch any settings that currently have no effect. (#288)
- **[Task]** **Faster survey loading for visitors** — A behind-the-scenes speed improvement so surveys, offers, and their rules load more quickly. (#42)
- **[Bug]** **Prevent lead submissions from timing out** — When several outside checks run during a submission, they can together take too long and fail. This keeps submissions within safe time limits so they finish cleanly. (#367)

## Dashboard & Reports
- **[Task]** **Report numbers that match the legacy system** — Some dashboard figures don't line up with the old system. This investigation pins down where the difference comes from and corrects it so you can trust the totals. (#271)
- **[Feature]** **Today's live numbers on the Dashboard** — You'll see up-to-the-hour impressions, clicks, leads, and revenue for the current day. (#34)
- **[Feature]** **Faster, more reliable historical report data** — A behind-the-scenes rollup of daily totals so past-date reports load quickly and consistently. (#35)

## Pre-Pings
- **[Feature]** **Bring over custom pre-ping checks** — Custom, client-specific validation that ran in the old system will be recreated so those checks keep working on the new platform. (#338)
- **[Task]** **Safely test the new pre-ping system** — The new system will run side by side with the old one to confirm it produces the same results before any switch-over. (#40)
- **[Feature]** **Verify pre-ping for every advertiser** — Each active advertiser's pre-ping will be checked for correct field mapping and success handling before cutover. (#41)

## Admin & Users
- **[Task]** **Legacy-to-new parity tracking** — An overarching effort to make sure every screen and behavior from the old system is matched (or has a tracked gap) in New Adsmith Frontend. (#319)
- **[Task]** **Users screen gap review** — A comparison of the old Users area against the new one, highlighting missing pieces like bulk actions, last-login and two-factor status, so they can be prioritized. (#80)
- **[Feature]** **Remove admin controls that do nothing** — Some settings (certain user permissions, data-client, and pre-ping options) are saved but never used. They'll be hidden or removed so the admin area only shows controls that actually do something. (#296)

## Placements
- **[Bug]** **Manually selected offers now carry over correctly** — On Manual-delivery placements, the specific offers you'd chosen weren't coming across, so the wrong offers displayed. Your selected offers and their order will now match what you set. (#370)
- **[Bug]** **Pixel tracking codes use the correct placeholder format** — The pixel example shown in the form didn't match what the system actually recognizes, which could corrupt tracking values. This makes the documented format and the real behavior line up. (#384)

## Data Clients
- **[Feature]** **Post-conversion delivery scripts restored** — After-success delivery and redirect behaviors from the old system will be recreated so those client hand-offs keep working. (#327)
- **[Bug]** **Accurate lead validation on manually processed leads** — Leads handled through the manual/broker path will run real validation instead of always reporting a placeholder "true," so the outcome you see is genuine. (#366)

## Modals
- **[Feature]** **New voucher-style visitor modal** — The visitor modal will match the richer legacy design: a personalized header with a voucher number, a color-coded progress bar that updates as offers are claimed, branded offer rows with clear "Claim Offer" and "No Thanks" options, and a trust footer. (#386)

## Flows
- **[Task]** **Fix Flow form styling** — Parts of the Flow form currently look unstyled or misaligned, with fields stacking oddly. This tidies up the layout so it matches the polished look of the other forms. (#152)

## Behind the Scenes
- **[Bug]** **Fix a data-reading glitch in Campaign records** — Corrects a rare case where a saved list of items could be read as empty, so campaign offer-group counts and details stay accurate. (#372)
- **[Task]** **Run new scheduled jobs alongside the old ones** — The new automated jobs will operate in parallel with the existing ones and be watched daily to confirm they match before anything is switched off. (#43)
- **[Task]** **Retire the low-risk scheduled jobs** — Safely turning off the least critical old background jobs once their replacements are proven stable. (#44)
- **[Task]** **Retire the mid-tier scheduled jobs** — Turning off the next set of old background jobs after the low-risk ones are confirmed steady. (#45)
- **[Task]** **Retire the most critical scheduled jobs** — Carefully switching off the highest-stakes old jobs last, with close monitoring and a quick way to revert. (#46)
- **[Task]** **Review an old stats job** — Deciding whether an older statistics job is still needed or can be retired. (#33)
- **[Task]** **Document rollback procedures** — Written, tested steps for safely reverting each production system if something goes wrong. (#48)
- **[Task]** **Create troubleshooting runbooks** — Quick-reference guides for resolving common issues like lead-processing or stats hiccups. (#49)
- **[Task]** **Add automated testing to the release process** — The full automated test suite will run after each update so problems are caught before they reach users. (#376)
- **[Task]** **Make automated testing safer and cleaner** — Prevent leftover test data and timing conflicts so automated tests stay reliable. (#377)
- **[Task]** **Testing-suite audit follow-ups** — Acting on findings from a review of the automated tests to close coverage gaps. (#379)
- **[Task]** **Weekly parity scorecard** — A recurring, automatically updated report that tracks how closely the new platform matches the old one. (#323)
- **[Feature]** **Slack helper that files issues automatically** — A Slack assistant that turns action items from conversations into tracked issues, saving manual copy-paste. (#272)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
