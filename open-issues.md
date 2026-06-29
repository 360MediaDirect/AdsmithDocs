# Open Issues — Plain-Language Overview

_Last updated 2026-06-29 21:31:31 UTC · 33 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Task]** **Custom date range on the Dashboard filter** — The date filter's "Custom" option will actually open a start- and end-date picker, so you can view Dashboard data for any range you choose instead of only the preset options. (#58)
- **[Task]** **Bring back the missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date range selector will update them. Right now only the system overview loads. (#240)
- **[Feature]** **New "Other Dashboard" monitoring views and activity log** — You'll get dedicated views for "Offers with Legs" and CLP offer performance (flagging anything converting under 30%), plus a searchable log of changes like pausing offers or editing caps, with who made each change and when. (#256)
- **[Task]** **A consistent Dashboard color scheme** — A defined set of colors will be applied across Dashboard views for cleaner, easier-to-read screens. (#263)
- **[Feature]** **Pick report dates without editing the address bar** — Date and range controls will live right in the Dashboard toolbar, so you can pull daily or custom reports through the interface. Links will still update so you can share them. (#268)
- **[Feature]** **Dashboard links open in a new tab** — Clicking a link on the Dashboard will open it in a new browser tab so you don't lose your place or your current view. (#269)

## Behind the Scenes
- **[Feature]** **Faster "today" numbers** — Work to power up-to-the-hour totals for impressions, clicks, leads, and revenue on the "today" view. (#34)
- **[Feature]** **Reliable historical reporting** — Behind-the-scenes work to roll up daily totals so past performance reports stay accurate. (#35)
- **[Task]** **Speed improvements for survey serving** — Caching of placement and offer settings to make surveys load and respond faster. (#42)
- **[Task]** **Safety checks before switching to new pre-ping handling** — Running the new and old pre-ping systems side by side, and validating each advertiser, to confirm results match before any switch. (#40, #41)
- **[Task]** **Smooth transition of scheduled background jobs** — A careful, monitored rollout that moves automated routines (like stats processing and offer cap resets) to the new platform, with the ability to roll back instantly if anything looks off. (#43, #44, #45, #46)
- **[Task]** **Tidying up an old stats routine** — Reviewing whether an older statistics process is still needed or can be retired. (#33)
- **[Task]** **Recovery and troubleshooting guides** — Written procedures for safely reverting changes and resolving common issues quickly if they arise. (#48, #49)
- **[Task]** **A safe testing environment with real sample data** — Setting up a staging area loaded with May and June data so reports can be verified without touching live information. (#270)
- **[Task]** **Confirming report numbers match the old system** — Comparing reports between the legacy and new platforms to find and explain any differences and confirm the data lines up. (#271)
- **[Task]** **Brand guidelines as the foundation for AI output** — Establishing a single, thorough brand-guidelines document to improve the quality of AI-generated content. (#264)
- **[Feature]** **A helper that turns conversations into tracked work items** — A tool to capture action items from team chats and log them automatically, reducing manual follow-up. (#272)

## Offers
- **[Task]** **Quick actions under each offer** — Familiar links such as Edit, Quick Edit, Trash, View, Preview, Trends, and Details will appear beneath each offer title, with Trends opening an offer activity page showing lead and revenue trends by date. (#252)
- **[Feature]** **Required fields checked before a lead is pushed** — When a pre-ping is set to run before pushing data, missing required fields will stop the lead right away instead of relying on the advertiser to catch it. (#218)
- **[Bug]** **Closing a gap where hidden offers still recorded leads** — Fixes a case where an offer hidden by a pre-ping could still auto-submit a lead and record a successful transaction. (#274)

## General / Across the App
- **[Feature]** **Light and dark mode** — You'll be able to switch the entire Admin between dark and light themes from your user menu, and your choice will be remembered next time you log in. (#59)
- **[Feature]** **Protection against overwriting each other's edits** — If two people open the same record, the second person will see it's being edited and by whom, and saves will be checked so no one silently overwrites someone else's changes. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Entering an invalid link in Link Testing will show a proper failure message instead of quietly sending you to the Dashboard. (#239)
- **[Task]** **Users area feature review** — A documented comparison of the Users screens against the legacy system to identify what's still missing (such as bulk actions and certain columns) and prioritize the gaps. (#80)

## Flows
- **[Feature]** **A clearer "Step order" setting** — The Step order field on the Flow form will get a plain-language label and inline help explaining what it controls and what its values mean, so it's no longer a mystery. (#226)
- **[Task]** **Polish for the Flow form's appearance** — Cleanup of styling on the Flow form so text boxes, color pickers, checkboxes, and side-by-side fields look consistent with the Placement and Modal forms. (#152)

## Campaigns
- **[Feature]** **Bring the Campaigns module to the new platform** — A high-priority effort to add Campaigns to New Adsmith Frontend, letting you view, create, edit, and configure campaigns and their offer groups just like the legacy admin. (#200)

## Placements
- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to manual order with drag-and-drop reordering, a clear "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f4270bdd0b31f8e2616cac8fcf7e170b6cc49a2bf509514aac88ea987a3291d0 -->
