# Open Issues — Plain-Language Overview

_Last updated 2026-06-27 16:24:15 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Light mode option for the Admin** — You'll be able to switch between the current dark theme and a new light theme from your account menu, and your choice will stick the next time you log in. Helpful for bright rooms and easier on the eyes. (#59)
- **[Feature]** **Protection against two people overwriting the same record** — When you open a record (an offer, flow, placement, advertiser, and so on) that someone else is already editing, you'll see a clear note about who has it open, and you'll be warned before your save could erase their changes. This prevents quiet, accidental loss of edits across the app. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Testing a broken or invalid link will show a proper error message instead of unexpectedly sending you back to the Dashboard. (#239)
- **[Task]** **Review of the Users area against the old system** — A documentation review comparing the new Users screens to the legacy version to confirm what's already covered and what still needs to be added (such as bulk actions and extra columns). (#80)
- **[Task]** **Brand guidelines as the foundation for AI output** — Establishing a single, detailed brand-guidelines document to feed the AI, so generated content stays consistently on-brand. (#264)

## Dashboard

- **[Task]** **Bring back the missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date-range selector will update them. Right now only the system overview loads. High priority. (#240)
- **[Feature]** **New "Other Dashboard" views plus a change history** — Adds an "Offers with Legs" view and a CLP performance view that flags offers converting under 30%, along with a searchable log of changes (like pausing offers or adjusting daily caps) showing who changed what and when. (#256)
- **[Task]** **Custom date range on the Dashboard** — Choosing "Custom" in the date filter will open a start/end date picker so you can view data for any range you need, not just preset options. (#58)
- **[Task]** **Consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for cleaner, more readable visuals. (#263)

## Flows

- **[Feature]** **Make "Step order" easy to understand** — The Step order setting will get a clearer label and inline help explaining what it controls and what the values mean, so you don't have to guess. (#226)
- **[Task]** **Fix the look of the Flow form** — Cleans up styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields display properly and match the other forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns area into the new platform** — Adds the Campaigns module so you can view, create, edit, and configure campaigns and offer groups, matching what's available in the legacy admin. This is a core capability that's currently missing. High priority. (#200)

## Placements

- **[Feature]** **Better control over offer ordering on Placements** — Selected offers will default to manual order, with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)

## Pre-Pings

- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping runs before a data push, leads missing required fields will be stopped up front rather than sent out and judged only by the advertiser's response, helping keep incomplete leads from slipping through. (#218)

## Behind the Scenes

- **[Feature]** **Accurate "today" numbers on the Dashboard** — Behind-the-scenes work to read up-to-the-hour activity (impressions, clicks, leads, revenue) so today's figures display correctly in Eastern Time. (#34)
- **[Feature]** **Faster, more reliable historical reporting** — Maintenance to roll up activity into daily totals so historical reports stay quick and accurate. (#35)
- **[Task]** **Speed improvements for the Survey Engine** — Adding a caching layer so surveys, offers, targeting, and caps load and check faster. High priority. (#42)
- **[Task]** **Check whether an old stats job is still needed** — Reviewing a legacy background job to decide if it can be retired without affecting your reports. (#33)
- **[Task]** **Side-by-side testing of the new pre-ping system** — Running the new and old systems together to confirm results match before the switch, with no impact to you. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each active advertiser's pre-ping behaves correctly before the changeover. (#41)
- **[Task]** **Roll out new background jobs alongside the old ones** — Running the new automated jobs in parallel with the existing ones and monitoring for any differences. (#43)
- **[Task]** **Carefully retire older background jobs (group 3)** — Turning off a lower-risk batch of legacy jobs once the replacements prove stable. (#44)
- **[Task]** **Carefully retire more background jobs (group 2)** — Turning off the next batch of legacy jobs after the first group is confirmed stable. (#45)
- **[Task]** **Carefully retire the most critical background jobs (group 1)** — Switching over the most sensitive jobs last, with close monitoring and the ability to revert quickly. (#46)
- **[Task]** **Document how to undo changes safely** — Writing step-by-step rollback procedures for each system so issues can be reversed quickly if they arise. (#48)
- **[Task]** **Troubleshooting guides for support staff** — Creating reference guides for common operational issues to keep things running smoothly. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
