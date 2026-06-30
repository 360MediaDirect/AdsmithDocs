# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 15:50:07 UTC · 13 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker on the dashboard** — Choosing "Custom" on the date filter will open a proper start- and end-date picker so you can look at any specific stretch of time, not just preset options like Today or This Month. (#58)
- **[Task]** **Bring back the full dashboard with richer reporting** — The dashboard will show all of its sections again — campaign stats (impressions, clicks, leads, revenue), top offers, a placements watch list, recent notes, and a view that flags offers converting under 30%. A searchable history of changes (who paused an offer, adjusted caps, etc.) is also planned. High priority. (#240)
- **[Feature]** **Pick report dates without editing the web address** — Today you have to hand-edit the address bar to change a report's date range. New date controls in the dashboard toolbar will let you pull daily or custom-range reports directly, while still keeping shareable links. (#268)

## Behind the Scenes

- **[Task]** **A safe testing environment with May & June data** — Sets up a separate staging space loaded with real-looking data so reports and new features can be checked without touching live information. (#270)
- **[Task]** **Confirming report numbers match the old system** — An investigation into why some dashboard figures differed from the legacy app, to find and fix any gaps and confirm the new platform processes data consistently. (#271)
- **[Feature]** **Automatic issue-logging from team chats** — A behind-the-scenes helper that turns action items from team conversations into tracked tasks automatically, reducing manual copy-and-paste. (#272)

## Offers

- **[Task]** **Quick action links under each offer** — Each offer will gain handy shortcuts (Edit, Quick Edit, Trash, View, Preview, Trends, Details) right beneath its title. "Trends" will open an activity page with lead and revenue trends, date filtering, and a daily performance breakdown. (#252)

## Campaigns

- **[Feature]** **Campaigns module added to the new platform** — The Campaigns area, currently missing in New Adsmith Frontend, will be rebuilt so you can create, edit, and manage campaigns and their offer groups just like in the old system. Critical, high priority. (#200)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Fixes styling problems on the Flow form so textareas, color pickers, checkboxes, and paired fields display cleanly and line up side by side, matching the polish of other forms. (#152)

## Link Testing

- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you back on the dashboard with no explanation. This fix shows a clear failure message instead, so you know the link didn't work. (#239)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on Placements** — Builds on recent drag-to-reorder work: new placements would default to your manual offer order (so your arrangement is actually used), and you'll be able to filter the available-offers list by category to find offers faster. (#275)

## Users

- **[Task]** **Review of what the Users area still needs** — A documentation review comparing the old Users management screens with the new ones, highlighting features still to be added (like bulk actions, last-login info, and password setup) to guide upcoming work. (#80)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — A new safeguard across all editable records (offers, flows, placements, advertisers, and more). When someone is editing a record, others will see a "locked by" banner, and a check at save time prevents accidentally wiping out a colleague's changes. (#267)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: bf396deeef75f72cc4ba41ede731d1ed1113c7dcc3b9038d97660e349109ef22 -->
