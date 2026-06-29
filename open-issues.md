# Open Issues — Plain-Language Overview

_Last updated 2026-06-29 15:09:36 UTC · 27 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Light mode option for the Admin** — You'll be able to switch the whole Admin between the current dark look and a new light theme, and your choice will be remembered next time you log in. Helpful for bright rooms or anyone who finds light backgrounds easier to read. (#59)
- **[Feature]** **Bring back the Campaigns area** — The Campaigns module from the older system isn't in New Adsmith Frontend yet. This high‑priority work adds it back so you can view, create, edit, and configure campaigns and their offer groups, just like before. (#200)
- **[Feature]** **Protection against two people overwriting the same record** — When someone else is already editing an offer, flow, placement, advertiser, or other record, you'll see a clear "locked by" notice, and the system will stop one person's save from silently wiping out another's changes. (#267)
- **[Bug]** **Clearer result when testing an invalid link** — Right now, entering a bad link in Link Testing quietly sends you to the dashboard. After this fix, you'll see a proper error message instead, so you know the link failed. (#239)
- **[Task]** **Comparing the old and new Users area** — A review documenting which Users features from the legacy system still need to be added (such as bulk role changes, last‑login info, and a password field on new users). This is the groundwork for closing those gaps. (#80)
- **[Task]** **Consistent brand guidelines for AI‑generated output** — A single, detailed brand‑guidelines document will be created and used as the main reference for AI‑assisted content, improving the quality and consistency of what's produced. (#264)

## Dashboard

- **[Task]** **Bring back the missing dashboard sections** — High priority: at the moment only the system overview loads. This restores the campaign stats, top offers, and watch‑list sections, and lets the date‑range filter update them. (#240)
- **[Feature]** **New "Other Dashboard" monitoring views** — Adds an "Offers with Legs" view for spotting steady, long‑running offers and a "CLP Performance" view that highlights offers converting under 30%, plus a searchable log of changes (like pausing offers or editing daily caps) so you can see who changed what and when. (#256)
- **[Task]** **Custom date range on the dashboard filter** — Choosing "Custom" will finally open a start/end date picker so you can view dashboard data for any period you like, not just the preset options. (#58)
- **[Task]** **A consistent dashboard color scheme** — A defined set of colors will be applied across the dashboard for better, more consistent readability. (#263)

## Offers

- **[Task]** **Quick action links under each offer** — Adds the familiar row actions (Edit, Quick Edit, Trash, View, Preview, Trends, Details) beneath each offer title, with Trends opening an Offer Activity page showing lead and revenue trends, date filtering, and a daily breakdown. (#252)
- **[Feature]** **Stop incomplete leads at pre‑ping push** — When a pre‑ping runs before sending data, leads missing required fields will be blocked right away instead of being sent on and relying on the advertiser to reject them. This matches how the "before offer displays" check already works. (#218)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain‑English label and inline help explaining what it controls and what the values mean, so you can use it without guessing. (#226)
- **[Task]** **Tidy up the Flow form's appearance** — Cleans up styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields look correct and consistent with the Placement and Modal forms. (#152)

## Placements

- **[Feature]** **Easier offer ordering on placements** — Selected offers will default to manual order, and you'll be able to drag them into the sequence you want, remove one with an "X" button, and filter the offer list by taxonomy to find offers faster. (#235)

## Behind the Scenes

These items are internal maintenance and reliability work with no direct change to what you see on screen.

- **[Feature]** **Live "today" stats** — Behind‑the‑scenes work so the dashboard's "today" view reflects up‑to‑date impressions, clicks, leads, and revenue in Eastern Time. (#34)
- **[Feature]** **Faster historical reporting** — A new automated process that rolls up daily totals so historical reports stay accurate and quick. (#35)
- **[Feature]** **Per‑advertiser pre‑ping checks** — Verifying each active advertiser's pre‑ping behaves correctly before the new system takes over. (#41)
- **[Task]** **Speed improvements for surveys** — Adding a caching layer so survey‑related lookups respond faster. (#42)
- **[Task]** **Side‑by‑side testing of the new pre‑ping system** — Running the new system alongside the old one to confirm results match before switching over. (#40)
- **[Task]** **Reviewing an older stats job** — Checking whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Rolling out new background jobs** — Deploying updated scheduled jobs to run in parallel with the existing ones while they're monitored. (#43)
- **[Task]** **Phased switch‑over of background jobs (lower risk)** — Carefully retiring lower‑priority legacy jobs once their replacements are proven stable. (#44)
- **[Task]** **Phased switch‑over of background jobs (mid‑tier)** — Retiring the next group of legacy stats jobs after a monitoring period. (#45)
- **[Task]** **Phased switch‑over of background jobs (critical)** — Carefully retiring the most important legacy jobs last, with close monitoring and a quick rollback plan. (#46)
- **[Task]** **Documented rollback steps** — Writing and testing recovery procedures for each system in case anything needs to be reverted. (#48)
- **[Task]** **Troubleshooting guides for the support team** — Creating reference guides so common issues can be resolved quickly. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 94900cccf9a7b3acb25443bbab588922c2cc2bff276c4d8ebadf6793ca8025fe -->
