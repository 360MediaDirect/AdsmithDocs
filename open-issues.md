# Open Issues — Plain-Language Overview

_Last updated 2026-06-27 18:24:14 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a real date picker so you can set your own start and end dates, with the selected range shown right on the filter button. Today the Custom option doesn't actually let you pick dates. (#58)
- **[Feature]** **Light mode option for the Admin UI** — You'll be able to switch between the current dark theme and a new light theme from your user menu, with your choice remembered next time you sign in. Helpful for bright rooms or anyone who prefers a lighter look. (#59)
- **[Task]** **Bring back missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date range selector will update them. Right now only the system overview loads. This is high priority. (#240)
- **[Feature]** **New "Other Dashboard" views plus an activity log** — Adds dedicated views for "Offers with Legs" and CLP offer performance (flagging offers converting under 30%), along with a searchable record of every offer change—pausing, cap edits, and status updates—showing who made each change and when. (#256)
- **[Task]** **Consistent Dashboard colors** — The Dashboard will adopt a defined color palette so charts and sections are easier to read at a glance. (#263)

## General / Across the App

- **[Feature]** **Protection against two people overwriting the same record** — When you open a record to edit (offers, flows, placements, advertisers, and more), others will see it's being edited and by whom, and you'll be warned before saving if someone changed it while you had it open. This prevents one person's edits from silently erasing another's. (#267)
- **[Task]** **Users area gap review** — A side-by-side review of the old Users screens versus the new ones, identifying what's still missing (like bulk actions and last-login info) so the new Users area can catch up. Behind-the-scenes analysis with no immediate visible change. (#80)
- **[Task]** **Brand guidelines to guide AI output** — A complete brand-guidelines document will be created and used as the main reference for AI-generated content, improving the quality and consistency of what the AI produces. (#264)
- **[Bug]** **Link testing should show errors, not bounce to the Dashboard** — Testing an invalid link will return a clear error message instead of quietly sending you to the Dashboard. (#239)

## Flows

- **[Task]** **Polish the Flow form's appearance** — Cleans up styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields look right and line up properly, matching the Placement and Modal forms. (#152)
- **[Feature]** **Make "Step order" understandable** — The Step order setting will get a clear label and inline help explaining what it controls and what its values do, so you no longer have to guess. (#226)

## Campaigns

- **[Feature]** **Add the missing Campaigns module** — Brings campaign management into New Adsmith Frontend, letting you view, create, edit, and configure campaigns and offer groups just like the old admin. This is critical and high priority, since campaigns currently can't be managed in the new platform. (#200)

## Placements

- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, a clear "X" to remove an offer, and the ability to filter the offer list by category. (#235)

## Pre-Pings

- **[Feature]** **Enforce required fields before sending a pre-ping** — When a pre-ping runs before pushing data, leads missing required fields will be stopped right away instead of being sent out and relying on the advertiser to reject them. This keeps incomplete leads from slipping through. (#218)

## Behind the Scenes

- **[Feature]** **Up-to-date "today" stats** — Behind-the-scenes work to power accurate same-day impressions, clicks, leads, and revenue on the Dashboard's "today" view. (#34)
- **[Feature]** **Reliable historical stats** — A scheduled process will roll up daily totals so longer-term reports stay accurate. (#35)
- **[Feature]** **Per-advertiser pre-ping checks** — Validating each active advertiser's pre-ping setup so leads are handled correctly once the new system goes live. (#41)
- **[Task]** **Faster surveys** — Adding a caching layer to speed up survey, offer, and targeting lookups. High priority. (#42)
- **[Task]** **Review an old stats job** — Checking whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Side-by-side pre-ping testing** — Running the new pre-ping system alongside the old one to confirm results match before switching over. (#40)
- **[Task]** **Run new scheduled jobs alongside the old ones** — Deploying the new background jobs to run in parallel for safe comparison. (#43)
- **[Task]** **Retire older background jobs (group 3)** — Turning off lower-risk legacy jobs once their replacements prove stable. (#44)
- **[Task]** **Retire mid-tier background jobs (group 2)** — Switching off the next set of legacy stats jobs after monitoring. (#45)
- **[Task]** **Retire critical background jobs (group 1)** — Carefully switching off the most important legacy jobs last, with a quick path to revert if needed. (#46)
- **[Task]** **Safety nets for switching systems** — Documenting and testing how to roll back each system if a problem comes up. (#48)
- **[Task]** **Troubleshooting guides** — Creating step-by-step guides for handling common operational issues quickly. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
