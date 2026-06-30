# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 05:22:47 UTC · 14 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard** — Picking "Custom" in the date filter will open a proper start-and-end date picker, so you can view dashboard data for any time period you choose instead of only the preset options. (#58)
- **[Task]** **Bring back the missing Dashboard sections** — High priority. Right now only the system overview loads. We're restoring the campaign stats, top offers, and watch list sections, and making sure the date range actually updates them. (#240)
- **[Feature]** **New "Other Dashboard" views plus a change history log** — Adds dedicated views for "Offers with Legs" and CLP offer performance (with low-converting offers under 30% clearly flagged), plus a searchable record of every offer change — pauses, cap changes, and status updates — so admins can see who changed what and when. (#256)
- **[Feature]** **Pick report dates without editing the web address** — You'll get easy date controls right in the dashboard toolbar, so you can pull a specific day or range without hand-editing the address bar. Shareable links still update so you can bookmark and send them. (#268)

## Offers & Campaigns

- **[Feature]** **Campaigns are coming to the new Admin** — High priority. The Campaigns area from the old system is being rebuilt here, so you can create, edit, and manage campaigns and their offer groups — including titles, questions, CTAs, offer handling, and marketing partners — all in New Adsmith Frontend. (#200)
- **[Task]** **Quick action links under each offer** — Each offer will show familiar shortcuts beneath its title (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an offer activity page showing lead and revenue trends, date filtering, and a daily performance breakdown. (#252)

## General / Across the App

- **[Feature]** **Protection against two people overwriting the same record** — When someone is already editing a record, others will see a clear "Locked by {name}" notice and a read-only view, and if a record changes while you have it open you'll be prompted to reload — so edits no longer silently overwrite each other. (#267)
- **[Bug]** **Invalid link tests now show a real error** — A bug fix: testing a bad link currently dumps you on the dashboard with no explanation. After this, you'll get a clear failure message in Link Testing instead. (#239)

## Flows

- **[Task]** **Cleaner, more consistent Flow form styling** — Polishing the look of the Flow form so text boxes, color pickers, checkboxes, and paired fields display properly and match the styling of the Placement and Modal forms instead of appearing unstyled or stacked oddly. (#152)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on Placements** — Follow-up work so new placements can default to your manual offer order (rather than random), and so you can filter the available offers list by vertical/category to find the right offers faster. (#275)

## Behind the Scenes

- **[Task]** **Users area comparison review** — A documentation review comparing the old Users management screens against the new ones to spot any missing features and plan what to bring over. (#80)
- **[Task]** **A safe testing environment with May & June data** — Setting up a separate practice environment loaded with recent data so testing and report checks can happen without ever touching live information. (#270)
- **[Task]** **Confirming report numbers match the old system** — Investigating why some dashboard report figures differed from the legacy system, pinpointing the cause, and confirming the numbers line up. (#271)
- **[Feature]** **Turning Slack discussions into tracked work items** — An internal helper that reads team conversations and automatically logs action items, reducing manual copy-and-paste when capturing requests. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8829154e1612d904d34214ce9b90f4489589545ee2e2d3b48335d954aee90f97 -->
