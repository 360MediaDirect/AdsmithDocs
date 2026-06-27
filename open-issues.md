# Open Issues — Plain-Language Overview

_Last updated 2026-06-27 12:25:50 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Review an older stats job** — We're checking whether a legacy data-collection routine is still needed or can be retired, so reporting stays accurate without unnecessary duplication. (#33)
- **[Feature]** **Faster "today" numbers on the Dashboard** — Behind-the-scenes work to calculate the current day's impressions, clicks, leads, and revenue in real time (in Eastern Time) so the Dashboard's "today" view is fresh. (#34)
- **[Feature]** **Reliable historical reporting** — Maintenance to roll up daily totals automatically so longer-range reports stay complete and consistent. (#35)
- **[Task]** **Pre-ping safety check before go-live** — We'll run the new lead pre-check process alongside the old one and compare results before switching over, so accuracy and speed are confirmed first. (#40)
- **[Feature]** **Per-advertiser pre-ping verification** — Each advertiser's pre-ping setup will be tested individually to confirm the right information is sent and matched correctly before launch. (#41)
- **[Task]** **Speed improvements for the Survey Engine** — High-priority groundwork to cache survey and offer settings so surveys load and respond faster. (#42)
- **[Task]** **Run new and old scheduled jobs side by side** — Both systems will run together for a period so we can confirm the new one behaves identically before relying on it. (#43)
- **[Task]** **Switch over routine survey-stats jobs** — Part of a careful, staged move to the new background system, with close monitoring and the ability to revert. (#44)
- **[Task]** **Switch over the stats-reporting jobs** — Continuing the staged move of background data jobs, monitored over a week to ensure stability. (#45)
- **[Task]** **Switch over the most critical background jobs** — The final, most carefully watched step of moving lead-processing and offer-cap jobs, with instant rollback ready if needed. (#46)
- **[Task]** **Document how to roll back safely** — Clear, tested recovery steps for each major system so any issue can be reversed quickly. (#48)
- **[Task]** **Create troubleshooting guides** — Step-by-step guides for the support team to resolve common issues (like lead processing or offer-cap problems) faster. (#49)

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open a start/end date picker so you can view Dashboard data for any range you like, instead of only preset options like Today or This Month. (#58)
- **[Task]** **Bring back missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date-range selector will update them — restoring the full overview you had before. (#240)
- **[Feature]** **New monitoring views and an activity log** — Adds "Offers with Legs" and CLP performance views (highlighting offers converting under 30%) plus a searchable record of changes like pausing offers or adjusting caps, so you can spot issues and see who changed what. (#256)
- **[Task]** **Consistent Dashboard colors** — A defined color palette will be applied across Dashboard views for clearer, more readable charts and data. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole Admin between dark and light themes from your user menu, with your choice remembered next time you sign in. (#59)
- **[Task]** **Users area review** — A comparison of the old and new Users screens to identify missing capabilities (such as bulk actions and extra columns) and prioritize what to add next. (#80)
- **[Task]** **Brand guidelines as the main AI input** — A single, comprehensive brand-guidelines document will guide AI-generated output for more consistent, on-brand results. (#264)
- **[Feature]** **Prevent two people overwriting the same record** — When someone is editing an offer, flow, placement, or other record, others will see it's locked and by whom, and you'll be warned if a record changed while you had it open — so no one's edits get silently lost. (#267)

## Flows

- **[Task]** **Fix the Flow form's appearance** — Cleans up styling issues so text boxes, color pickers, checkboxes, and paired fields display correctly and match the look of other forms. (#152)
- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain-language label and inline help explaining what it controls, so it's no longer confusing. (#226)

## Placements

- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter offers by taxonomy — giving you full control over how offers are arranged. (#235)

## Pre-Pings

- **[Feature]** **Block leads missing required information** — When required fields are empty, the lead will be stopped before it's sent, rather than being passed along and only flagged in a log — keeping incomplete leads from slipping through. (#218)

## Link Testing

- **[Bug]** **Clear error for invalid links** — Testing a bad link will show a proper failure message instead of sending you to the Dashboard, so you know right away the link didn't work. (#239)

## Campaigns

- **[Feature]** **Add the Campaigns module** — Brings campaign management into New Adsmith Frontend so you can view, create, edit, and configure campaigns and offer groups — matching what's available in the legacy system. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
