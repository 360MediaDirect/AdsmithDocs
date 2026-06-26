# Open Issues — Plain-Language Overview

_Last updated 2026-06-26 23:26:00 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Review of an older stats job** — We're checking whether an older background process that tracks certain stats is still needed or can be retired, to keep reporting clean and efficient. (#33)
- **[Feature]** **Faster historical reporting totals** — Behind-the-scenes work to roll up daily numbers so that historical reports load reliably and accurately over time. (#35)
- **[Task]** **Side-by-side testing of the new pre-ping system** — Before switching over, we'll run the new lead pre-check alongside the current one to confirm it produces the same results. No visible change yet; this protects accuracy. (#40)
- **[Task]** **Speed improvements for the Survey engine** — Adding a caching layer so surveys, offers, and caps load faster during live traffic. (#42)
- **[Task]** **Rolling out new scheduled jobs in parallel** — The new automated background jobs will run alongside the existing ones so we can compare them safely before relying on them. (#43)
- **[Task]** **Gradual switchover of background jobs (first wave)** — Retiring the lowest-risk old scheduled jobs once their replacements are proven stable, with the ability to switch back if needed. (#44)
- **[Task]** **Gradual switchover of background jobs (second wave)** — Retiring the next group of older stats and reporting jobs after the first wave runs cleanly. (#45)
- **[Task]** **Gradual switchover of the most critical background jobs (final wave)** — Carefully retiring the most important jobs (lead processing and offer cap resets) last, with close monitoring and instant rollback. (#46)
- **[Task]** **Documented recovery steps** — Writing clear rollback procedures for each major system so we can restore normal operation quickly if anything goes wrong. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Creating step-by-step guides for the support team to resolve issues like lead processing or stats problems faster. (#49)

## Dashboard

- **[Feature]** **Live "today" numbers on the Dashboard** — The Dashboard's "today" view will show up-to-the-hour impressions, clicks, leads, and revenue in your local (Eastern) time. (#34)
- **[Task]** **Custom date range on the Dashboard** — Choosing "Custom" in the date filter will open a start/end date picker so you can view Dashboard data for any range you want. (#58)
- **[Task]** **Restore missing Dashboard sections** — Bringing back the campaign stats, top offers, and watch list sections so the full Dashboard loads and updates with your selected date range. This is high priority. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds dedicated views for long-running offers and CLP offer performance (flagging those converting under 30%), plus a searchable log of offer and system changes for easy auditing. (#256)
- **[Task]** **Consistent Dashboard colors** — Applying a defined color palette across the Dashboard to make charts and data easier to read. (#263)

## General / Across the App

- **[Feature]** **Dark and light mode** — A new theme switch lets you choose light or dark mode across the whole Admin area, with your choice remembered between visits. (#59)
- **[Task]** **Users screen comparison review** — A documentation review comparing the new Users area to the older one, so missing options (like bulk actions and extra columns) can be planned and added. (#80)
- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link will show a clear error message instead of unexpectedly sending you to the Dashboard. (#239)
- **[Task]** **Brand guidelines as the main AI input** — Establishing a single, detailed brand-guidelines document to feed AI-generated content, improving the quality and consistency of results. (#264)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit, others will see it's being edited and you'll be warned if someone changed it since you opened it — protecting your work across offers, flows, placements, advertisers, and more. (#267)

## Pre-Pings

- **[Feature]** **Per-advertiser pre-ping checks** — Confirming each active advertiser's pre-ping works correctly, with the right field mapping and pass/fail rules, before the new system goes live. (#41)
- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping is set to run before pushing data, leads missing required fields will be stopped right away instead of being sent on, preventing incomplete leads from slipping through. (#218)

## Flows

- **[Task]** **Cleaner, consistent Flow form styling** — Fixing unstyled areas of the Flow form (text boxes, color pickers, checkboxes, and side-by-side fields) so it looks and behaves like the Placement and Modal forms. (#152)
- **[Feature]** **Clearer "Step order" setting on Flows** — Adding a plain-language label and helpful explanation so you can tell exactly what the step order controls and what its values mean. (#226)

## Placements

- **[Feature]** **Better offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer, and the ability to filter the offer list by category. (#235)

## Campaigns

- **[Feature]** **Campaigns module added to the new platform** — Bringing the Campaigns feature into New Adsmith Frontend so you can create, edit, and manage campaigns and offer groups just as in the legacy system. This is high priority. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
