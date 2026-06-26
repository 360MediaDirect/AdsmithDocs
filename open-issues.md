# Open Issues — Plain-Language Overview

_Last updated 2026-06-26 15:45:56 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" on the Dashboard date filter will open a start/end date picker so you can view results for any specific stretch of time, not just the preset options. (#58)
- **[Task]** **Bring back missing Dashboard sections** — High priority. The campaign stats, top offers, and watch lists will return to the Dashboard, and your date-range selection will properly update them. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — You'll get dedicated views for "Offers with Legs" and CLP offer performance (flagging offers converting under 30%), plus a searchable record of changes like pausing offers or adjusting caps, with who made each change and when. (#256)
- **[Task]** **Consistent Dashboard colors** — The Dashboard will adopt a defined color palette so charts and sections are easier to read at a glance. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode** — You'll be able to switch the whole admin between dark and light themes from your user menu, and your choice will be remembered next time you sign in. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, you'll see who is currently editing it and be warned before you can accidentally overwrite someone else's changes, so updates no longer get lost. (#267)
- **[Task]** **Brand guidelines as the basis for AI output** — A clear, comprehensive brand-guidelines document will be used as the main reference for AI-generated content, improving the quality and consistency of results. (#264)

## Flows

- **[Task]** **Fix the styling on Flow forms** — Some Flow form fields (text boxes, color pickers, checkboxes, and paired fields) currently look unstyled or stack awkwardly; this cleans them up to match the polished look of the Placement and Modal forms. (#152)
- **[Feature]** **Make the "Step order" setting clear** — The Flow form's step-order setting will get a plain-language label and inline help explaining what it controls and what its values mean, so you no longer have to guess. (#226)

## Campaigns

- **[Feature]** **Add the Campaigns module** — Critical, high priority. The Campaigns area from the legacy system will be rebuilt here, letting you create, edit, and manage campaigns and their offer groups (titles, questions, CTAs, offer handling, order, limits, and marketing partners) without leaving New Adsmith Frontend. (#200)

## Placements

- **[Feature]** **Better control over offers on a Placement** — Selected offers will default to manual order, with drag-and-drop reordering, a clear "X" to remove an offer, and the ability to filter the offer list by taxonomy, making it much easier to arrange offers exactly how you want. (#235)

## Pre-Pings

- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping runs before pushing data, leads missing required fields will now be stopped up front instead of being sent anyway, preventing incomplete leads from slipping through. (#218)

## Link Testing

- **[Bug]** **Show a real error for invalid links** — Testing an invalid link currently dumps you back on the Dashboard; instead you'll see a clear failure message right in the Link Testing screen. (#239)

## Users

- **[Task]** **Review what's missing from the Users area** — A comparison of the old and new Users screens to identify gaps (such as bulk actions, last-login info, and other details) and prioritize what to add next. (#80)

## Behind the Scenes

- **[Feature]** **Faster, accurate "today" stats** — Behind-the-scenes work to power up-to-the-day numbers (impressions, clicks, leads, and revenue) for the Dashboard's "today" view, with correct time-zone handling. (#34)
- **[Feature]** **Reliable historical reporting totals** — Maintenance to roll up daily figures so your historical reports stay accurate over time. (#35)
- **[Task]** **Double-checking a stats job** — Reviewing whether an older stats process is still needed or can be retired, with no change to what you see. (#33)
- **[Task]** **Side-by-side testing of the new pre-ping system** — Running the new and old pre-ping processes together to confirm the new one matches before it takes over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each active advertiser's pre-ping behaves correctly before the switchover. (#41)
- **[Task]** **Speed improvements for the survey experience** — High priority. Adding a behind-the-scenes caching layer so surveys, offers, and limits load and respond faster. (#42)
- **[Task]** **Roll out the new background jobs alongside the old ones** — Running the new automated tasks in parallel with the existing ones and watching for any differences before relying on them. (#43)
- **[Task]** **Retire older background tasks (group 3)** — Switching off the first batch of legacy automated tasks once their replacements prove stable. (#44)
- **[Task]** **Retire more background tasks (group 2)** — Turning off the next batch of legacy stats tasks after the earlier ones run smoothly. (#45)
- **[Task]** **Retire the most critical background tasks (group 1)** — Carefully switching off the most important legacy tasks (lead processing and offer-cap reset) last, with close monitoring. (#46)
- **[Task]** **Document how to undo changes safely** — Writing step-by-step recovery procedures for each system so issues can be reversed quickly if needed. (#48)
- **[Task]** **Troubleshooting guides for the support team** — Creating reference guides for common issues so problems can be diagnosed and resolved faster. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
