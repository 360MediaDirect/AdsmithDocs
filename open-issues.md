# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 03:05:07 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard
- **[Task]** **Custom date range on the dashboard filter** — Choosing "Custom" in the date filter will open a proper start/end date picker, so you can view dashboard data for any specific range instead of only the preset options like Today or This Month. (#58)
- **[Task]** **Bring back missing dashboard sections** — The dashboard will once again show campaign stats, top offers, and watch lists (not just the system overview), and the date range selector will update them. This is a high-priority fix. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — You'll get dedicated views for offers with sustained performance ("Offers with Legs") and for CLP offer performance, with low-converting offers highlighted. A searchable log will also record changes like pausing offers or editing caps, with who made the change and when. (#256)
- **[Feature]** **Pick report dates without touching the web address** — You'll be able to choose a day or range directly from the dashboard toolbar, rather than manually editing the address bar. The link still updates so you can bookmark or share it. (#268)
- **[Feature]** **Dashboard links open in a new tab** — Clicking a link on the dashboard will open it in a new browser tab, so you keep your current dashboard view instead of being navigated away. (#269)

## Offers
- **[Feature]** **Enforce required fields before sending leads** — When an offer check runs before a data push, leads missing required information will be stopped up front instead of being passed through, preventing incomplete or malformed leads from slipping by. (#218)
- **[Task]** **Quick action links under each offer** — Each offer will show handy links beneath its title (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an activity page showing lead and revenue performance over time. (#252)
- **[Bug]** **Close a gap that let hidden offers still submit leads** — In certain auto-register setups, an offer could be correctly hidden yet still record a successful lead. This fix makes sure a hidden offer never submits, keeping your reporting and revenue accurate. (#274)

## General / Across the App
- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit it, others will see it's locked and by whom, and the system will warn you if someone changed it since you opened it. This protects your work from being silently overwritten across offers, flows, placements, advertisers, and more. (#267)

## Flows
- **[Task]** **Tidy up the Flow form's appearance** — Remaining styling issues on the Flow form will be cleaned up so text boxes, color pickers, checkboxes, and paired fields look consistent with the rest of the app instead of appearing plain or stacked awkwardly. (#152)

## Placements
- **[Feature]** **Better control over the offer selection list** — Building on recent drag-to-reorder work, placements will be able to default to manual offer ordering (so your arrangement actually takes effect) and let you filter the available offers list by category. (#275)

## Campaigns
- **[Feature]** **Bring the Campaigns area into the new platform** — A Campaigns module will be added so you can view, create, edit, and configure campaigns and their offer groups, matching what's available in the current system. This is a critical, high-priority addition. (#200)

## Users
- **[Task]** **Review of what's missing in the Users area** — A documentation review comparing the new Users screens to the older system, flagging gaps like bulk actions, login/2FA details, and a few form fields so the team can prioritize what to add next. (#80)

## Link Testing
- **[Bug]** **Show a clear error for invalid links** — Testing a bad link will now return a proper failure message instead of quietly sending you to the dashboard, so you immediately know the link didn't work. (#239)

## Behind the Scenes
- **[Task]** **Dedicated testing environment with May and June data** — Setting up a separate, safe space loaded with recent data so testing and report checks can happen without touching live information. (#270)
- **[Task]** **Checking report numbers against the old system** — An investigation into why some dashboard figures differed from the legacy system, to pin down the cause and confirm the numbers line up. (#271)
- **[Feature]** **Turn Slack conversations into tracked tasks automatically** — A helper that reads team chats and files them as work items, reducing manual copy-and-paste when capturing requests and follow-ups. (#272)
- **[Task]** **Stronger brand guidelines to guide AI output** — Establishing a single, thorough brand-guidelines document to use as the main reference for AI-generated content, improving the quality and consistency of results. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 3a22b4ee69d23ae5129a56cac1ade559584b388a1abb27033c1ca95602512225 -->
