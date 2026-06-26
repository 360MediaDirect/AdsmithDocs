# Open Issues — Plain-Language Overview

_Last updated 2026-06-26 00:36:30 UTC · 15 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a proper start/end date picker, so you can view dashboard data for any specific period instead of only preset ranges like Today or This Month. (#58)
- **[Task]** **Restore missing Dashboard sections** — Campaign stats, top offers, and watch lists will be brought back to the Dashboard, and the date-range selector will update them. Right now only the system overview loads. (#240)
- **[Feature]** **"Other Dashboard" monitoring views and an activity log** — New views will help you watch long-running ("with legs") offers and flag low-converting CLP offers, plus a searchable record of key actions (pausing offers, daily cap changes, status updates) will show what changed, when, and by whom. (#256)
- **[Feature]** **Sub-ID Stats moving to the Dashboard** — Sub-ID Stats will be relocated from inside the placement form into the Dashboard reporting area, making them easier to find alongside your other reports. (#236)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will show activity in 15-minute increments, giving you the close, real-time view needed to spot offer or partner-server issues quickly. (#243)
- **[Feature]** **Dark and Light mode for the Admin** — A theme switch lets you choose a light or dark appearance to suit your environment and comfort, with your choice remembered between visits. (#59)
- **[Task]** **Consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for cleaner, more readable visuals. (#263)

## General / Across the App

- **[Feature]** **Campaigns module** — A high-priority addition that brings campaign management into New Adsmith Frontend, so you can view, create, edit, and configure campaigns (titles, question text, offer groups, CTAs, offer handling, and marketing partners) just as you could in the previous admin. (#200)
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record, New Adsmith Frontend will show a clear "locked by" notice and warn you if someone else has changed a record since you opened it, preventing accidental lost work across offers, flows, placements, advertisers, and other entities. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper failure message in the Link Testing screen instead of unexpectedly sending you to the Dashboard. (#239)

## Flows

- **[Task]** **Fix the look of the Flow form** — The Flow form will be cleaned up so text boxes, color pickers, checkboxes, and paired fields display correctly and sit side-by-side, matching the polished styling of the Placement and Modal forms. (#152)
- **[Feature]** **Clearer "step order" setting** — The step-order control on the Flow form will get plain labels and help text (or a redesign) so it's obvious what it controls and what each option means. (#226)

## Placements

- **[Feature]** **Easier offer ordering on Placements** — Selected offers will default to Manual Order with drag-and-drop reordering, an "X" to remove an offer (so clicking is reserved for dragging), and the ability to filter the offer list by taxonomy. (#235)

## Offers

- **[Bug]** **Enforce required fields before a data push** — When a pre-ping runs before a data push, required fields will be checked first so leads missing required information are stopped immediately rather than being passed along to the advertiser. (This change is pending confirmation that it's the desired behavior.) (#218)

## Behind the Scenes

- **[Task]** **Comprehensive brand guidelines for AI output** — The team will establish a thorough brand-guidelines document to use as the main reference for AI-generated content, improving the quality and consistency of results. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 2a56fd67f9291cb8ae4aad8782237f68a408d23759c09f54732863f026266184 -->
