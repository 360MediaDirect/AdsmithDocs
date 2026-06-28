# Open Issues — Plain-Language Overview

_Last updated 2026-06-28 18:23:57 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Task]** **Add a custom date range picker** — When you choose "Custom" on the Dashboard date filter, you'll get start and end date fields so you can view results for exactly the period you care about, with the chosen range shown right on the filter button. (#58)
- **[Task]** **Restore missing Dashboard sections** — High priority. The campaign stats, top offers, and watch list sections will return to the Dashboard, and changing the date range will update them. (#240)
- **[Feature]** **More Dashboard views and an activity log** — A new "Other Dashboard" area will help you track steady-performing offers ("Offers with Legs") and flag CLP offers converting under 30%, plus a searchable log of every offer change (pauses, cap edits, status updates) with who made them and when. (#256)
- **[Feature]** **Dark and light mode toggle** — You'll be able to switch the whole admin between dark and light themes from your user menu, and your choice will stick the next time you log in. (#59)
- **[Task]** **Consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for cleaner, easier-to-read screens. (#263)

## General / Across the App
- **[Feature]** **Protection against overwriting each other's edits** — If two people open the same record, you'll see a clear "being edited by…" notice and a warning if it changed while you had it open, so one person's save can't quietly wipe out another's work. Works across all entity screens (Offers, Flows, Placements, Advertisers, and more). (#267)
- **[Task]** **Users screen gap review** — A documentation review comparing the new Users area to the legacy one, highlighting missing pieces (like bulk role changes and last-login info) to guide upcoming improvements. (#80)
- **[Bug]** **Invalid links now show an error** — When you test a link that isn't valid, you'll get a clear failure message instead of being unexpectedly sent to the Dashboard. (#239)
- **[Task]** **Brand guidelines to improve AI output** — A single, comprehensive brand guide will be used as the main reference for AI-generated content, leading to more on-brand results. (#264)

## Flows
- **[Feature]** **Clearer "Step order" setting** — The Step order control on the Flow form will get a plain-language label and helpful inline text explaining what it does and what the values mean, so you don't have to guess. (#226)
- **[Task]** **Tidy up the Flow form's appearance** — Cleans up styling issues on the Flow form (plain-looking text boxes, color pickers, checkboxes, and fields that stack awkwardly) so it looks polished and consistent with the Placement and Modal forms. (#152)

## Campaigns
- **[Feature]** **Bring the Campaigns area to the new platform** — Critical, high priority. The Campaigns module from the old admin is being rebuilt here so you can view, create, edit, and configure campaigns and offer groups without going back to the legacy system. (#200)

## Placements
- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, an "X" to remove an offer (so clicking just moves it), and the ability to filter the offer list by taxonomy. (#235)

## Pre-Pings
- **[Feature]** **Enforce required fields before sending a lead** — When a pre-ping runs before a data push, leads missing required information will be stopped right away instead of being sent out and relying on the advertiser to reject them. (#218)

## Behind the Scenes
- **[Feature]** **Faster "today" numbers** — Behind-the-scenes work to show up-to-date impressions, clicks, leads, and revenue for the current day, with correct Eastern Time handling. (#34)
- **[Feature]** **Reliable historical reporting totals** — Maintenance to roll up daily figures so longer-term reports stay accurate. (#35)
- **[Task]** **Performance caching for surveys** — High priority groundwork to make survey-driven screens load faster. (#42)
- **[Task]** **Safety testing for pre-pings** — Running the new pre-ping process alongside the current one to confirm results match before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Verifying each active advertiser's pre-ping behaves correctly before the switch. (#41)
- **[Task]** **Review an older stats job** — Deciding whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Roll out updated scheduled jobs** — Deploying the new background jobs to run safely alongside the existing ones during the transition. (#43)
- **[Task]** **Switch over background jobs — first group** — Retiring the lowest-risk legacy scheduled jobs once their replacements prove stable. (#44)
- **[Task]** **Switch over background jobs — second group** — Retiring additional stats-related legacy jobs after the first group is confirmed stable. (#45)
- **[Task]** **Switch over background jobs — final group** — Critical. Carefully retiring the most important legacy jobs (lead processing and offer cap resets) with close monitoring and a quick fallback plan. (#46)
- **[Task]** **Document recovery steps** — Writing and testing rollback procedures for each core system in case something needs to be reversed. (#48)
- **[Task]** **Troubleshooting guides for the team** — Creating step-by-step guides for handling common issues like lead processing or cap reset failures. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
