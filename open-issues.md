# Open Issues — Plain-Language Overview

_Last updated 2026-06-29 07:38:14 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

This is a large body of behind-the-scenes work to move the engine that powers New Adsmith Frontend onto a faster, more modern foundation. Most of it won't change what you see day to day, but it improves speed, reliability, and our ability to recover quickly if something goes wrong.

- **[Feature]** **Faster "today" numbers** — Today's impressions, clicks, leads, and revenue will be pulled from a quicker, near real-time source so the latest activity shows up sooner. (#34)
- **[Feature]** **Reliable historical totals** — Daily numbers will be rolled up automatically and accurately (in Eastern Time) so historical reports stay correct and consistent. (#35)
- **[Task]** **Tidy up duplicate stats tracking** — We're reviewing an older stats process to decide whether it's still needed, avoiding duplicate or redundant work in the background. (#33)
- **[Task]** **Safety check for lead pre-validation** — Before switching over, we'll run the new and old lead pre-check systems side by side and compare results to be sure the new one behaves correctly. (#40)
- **[Feature]** **Per-advertiser pre-check verification** — We'll confirm the new lead pre-check works correctly for every active advertiser, including their specific field requirements. (#41)
- **[Task]** **Speed boost for the Survey engine** — A new caching layer will make survey-related lookups (placements, offers, caps) faster, so live surveys respond more quickly. High priority. (#42)
- **[Task]** **Run new and old scheduled jobs together** — The new background jobs will run alongside the existing ones for a while so we can watch for any differences before relying on them. (#43)
- **[Task]** **Retire older scheduled jobs (first group)** — Once the new survey-stats job proves stable, the matching older job is switched off, with the ability to turn it back on if needed. (#44)
- **[Task]** **Retire scheduled jobs (second group)** — Several more older stats and reporting jobs are switched off after a monitoring period. (#45)
- **[Task]** **Retire the most critical scheduled jobs (final group)** — The most important jobs (lead processing and offer-cap resets) are switched over last, with close monitoring and instant rollback ready. (#46)
- **[Task]** **Documented rollback plans** — Clear, tested steps for reversing each major system if something goes wrong, so issues can be undone quickly and safely. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Step-by-step guides for handling things like lead-processing or stats hiccups, helping the team resolve problems faster. (#49)

## Dashboard

- **[Task]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will come back to the Dashboard, and the date range selector will properly update them. High priority. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — You'll get dedicated views for long-running ("Offers with Legs") and CLP offer performance, with under-30% converters flagged for quick action, plus a searchable record of changes like pausing offers or editing caps. (#256)
- **[Task]** **Custom date range on the date filter** — Choosing "Custom" will open a start/end date picker so you can view Dashboard data for any range you like, not just the preset options. (#58)
- **[Task]** **A polished, consistent color scheme** — The Dashboard will adopt a defined color palette for cleaner, easier-to-read visuals across all views. (#263)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain-language label and helpful inline explanation, so you can understand what it controls without outside help. (#226)
- **[Task]** **Fix the Flow form's appearance** — Parts of the Flow form currently look unstyled or misaligned compared to other forms; this cleans up the layout so it looks consistent and tidy. (#152)

## General / Across the App

- **[Feature]** **Dark/Light mode toggle** — You'll be able to switch the whole Admin between dark and light themes, with your choice remembered between sessions — handy for different lighting and personal preference. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — If two people open the same record, you'll be warned when someone else is editing it, and saves will be safeguarded so no one's changes get silently wiped out. (#267)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — A full Campaigns area will be added so you can create, edit, and manage campaigns and offer groups in New Adsmith Frontend, matching what the older system offered. Critical, high priority. (#200)

## Placements

- **[Feature]** **Easier offer ordering and filtering** — Selected offers will default to manual order with drag-and-drop reordering, a clear "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)

## Pre-Pings & Offers

- **[Feature]** **Catch missing required fields earlier** — When a pre-ping runs before pushing data, leads missing required fields will be stopped up front rather than sent out, preventing incomplete leads from slipping through. (#218)

## Link Testing

- **[Bug]** **Show a clear error for invalid links** — Testing a bad link will display a proper error message instead of unexpectedly sending you to the Dashboard. (#239)

## Users

- **[Task]** **Gap review of the Users area** — A review comparing the new Users screens to the older version, identifying missing features (like bulk actions and certain columns) so the team can prioritize bringing them back. (#80)

## Brand

- **[Task]** **Use brand guidelines to guide AI output** — A comprehensive brand-guidelines document will become the main reference for AI-generated content, improving the quality and consistency of results. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
