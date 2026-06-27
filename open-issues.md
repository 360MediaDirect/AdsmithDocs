# Open Issues — Plain-Language Overview

_Last updated 2026-06-27 22:22:12 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a proper start- and end-date picker, so you can view dashboard numbers for any range you like instead of only the preset options. (#58)
- **[Task]** **Bring back missing Dashboard sections** — Restores the campaign stats, top offers, and watch list sections so the Dashboard shows full reporting again (not just the system overview), and the date range will actually update them. This is a high-priority fix. (#240)
- **[Feature]** **New "Other Dashboard" views plus an activity log** — Adds dedicated views for "Offers with Legs" and CLP offer performance (flagging offers converting under 30%), along with a searchable record of every offer change — pauses, cap edits, status updates — with who made them and when. (#256)
- **[Task]** **Consistent Dashboard colors** — Applies a defined color palette across the Dashboard so charts and sections are easier to read at a glance. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole admin between dark and light themes from your user menu, and your choice will be remembered next time you sign in. (#59)
- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link will show a clear error message in the Link Testing screen instead of quietly sending you back to the Dashboard. (#239)
- **[Task]** **Stronger brand guidelines for AI output** — Establishes a single, detailed brand-guidelines document used as the main input for AI-generated content, improving the quality and consistency of what the AI produces. (#264)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit it, others will see it's locked (with your name and when you started), and if someone changed it while you had it open, you'll be prompted to reload instead of accidentally wiping out their work. This applies across all editable screens — offers, flows, placements, advertisers, and more. (#267)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Fixes unstyled and misaligned parts of the Flow form (text boxes, color pickers, checkboxes, and paired fields) so it looks and behaves like the Placement and Modal forms. Some of this is done, with the rest being finished carefully to avoid breaking other tabs. (#152)
- **[Feature]** **Make the "Step order" setting understandable** — Adds a clearer label and inline help text explaining what the Step order setting controls and what its values do, so you no longer have to guess. (#226)

## Campaigns

- **[Feature]** **Bring the Campaigns module into New Adsmith Frontend** — Adds the ability to view, create, edit, and manage campaigns and offer groups — including titles, question text, CTA text, offer handling, order, and partners — matching what's available in the legacy admin. This is a high-priority gap. (#200)

## Placements

- **[Feature]** **Better control over selected offers** — Selected offers will default to manual order and can be reordered by dragging, with an "X" to remove each one and the ability to filter the offer list by taxonomy — making it much easier to organize offers on a placement. (#235)

## Pre-Pings

- **[Feature]** **Catch missing required fields before sending** — Pre-pings set to run before a data push will now check required fields first and stop a lead with missing information, rather than sending it on and relying on the advertiser to reject it. (#218)

## Users

- **[Task]** **Review of the Users screen against the legacy version** — A documented comparison identifying which Users features (such as bulk actions, last-login info, and 2FA status) are still missing in New Adsmith Frontend, to guide what gets built next. (#80)

## Behind the Scenes

- **[Feature]** **Up-to-date "today" numbers on the Dashboard** — Behind-the-scenes work so the Dashboard's "today" view reflects current-day impressions, clicks, leads, and revenue accurately in Eastern Time. (#34)
- **[Feature]** **Faster historical reporting** — Maintenance to roll up daily totals so historical stats load reliably over time. (#35)
- **[Task]** **Speed improvements for surveys** — Behind-the-scenes caching work to make survey-related screens respond faster. This is high priority. (#42)
- **[Task]** **Review of an older stats process** — Checking whether a legacy stats job is still needed or can be retired, with no change you'll notice. (#33)
- **[Task]** **Side-by-side testing of the new pre-ping system** — Running the new and old pre-ping systems together to confirm the new one behaves correctly before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each advertiser's pre-ping setup ahead of the switchover so leads continue to flow correctly. (#41)
- **[Task]** **Rolling out updated scheduled tasks** — Running the new automated background tasks alongside the existing ones to confirm they match before relying on them. (#43)
- **[Task]** **Careful switchover of background tasks (Group 3)** — Retiring the first batch of older scheduled jobs once the replacements prove stable, with close monitoring. (#44)
- **[Task]** **Careful switchover of background tasks (Group 2)** — Retiring the next batch of older scheduled jobs (various stats and reporting tasks) after the previous group is confirmed stable. (#45)
- **[Task]** **Careful switchover of the most critical background tasks (Group 1)** — Retiring the most important legacy jobs (lead processing and offer-cap resets) last, with close monitoring and the ability to roll back instantly. (#46)
- **[Task]** **Documented recovery steps** — Writing and testing clear rollback procedures for each major system so issues can be reversed quickly if needed. (#48)
- **[Task]** **Troubleshooting guides for the support team** — Creating step-by-step guides for handling common operational issues, helping problems get resolved faster. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
