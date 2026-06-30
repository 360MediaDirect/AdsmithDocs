# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 20:37:13 UTC · 13 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard & Reports

- **[Task]** **Custom date range picker on the Dashboard** — When you choose "Custom" in the date filter, you'll now get start and end date pickers with Apply and Cancel buttons, so you can view dashboard data for any specific range you like. (#58)
- **[Feature]** **Pick report dates without editing the web address** — New date controls will live right in the dashboard toolbar, so you can pull a single day's report or any range with a click instead of changing the address bar by hand. Links will still stay shareable. (#268)
- **[Task]** **Confirming report numbers match the old system** — We're comparing dashboard report figures against the legacy system over the same date range to find and explain any differences, so you can trust that the numbers are accurate. (#271)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit, it will be reserved for you, and others will see a "currently being edited by…" notice. If someone changed it while you had it open, you'll be prompted to reload instead of accidentally wiping out their work. This applies across all editable screens. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when — across offers, placements, advertisers, flows, and more, including automated changes — so you can always answer "who changed this and when." You'll also be able to view a record's history right from its detail page. (#276)

## Behind the Scenes

- **[Task]** **A safe testing environment with May and June data** — We're setting up a separate testing area loaded with recent data so reviewers can validate reports without any risk to live information. (#270)
- **[Feature]** **Automatically turning meeting notes into tracked work** — We're building a helper that reads conversations and files the resulting to-dos automatically, so action items don't get lost and tracking stays up to date. (#272)

## Offers

- **[Task]** **Quick action links under each offer** — You'll get handy links beneath every offer title — Edit, Quick Edit, Trash, View, Preview, Trends, and Details — with Trends opening an activity page showing lead and revenue performance over time. (#252)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on placements** — We're following up on the offer reordering work so your manual order actually takes effect, and adding a way to filter the available offers list by category to make finding the right offers faster. (#275)

## Flows

- **[Task]** **Polishing the look of the Flow form** — We're fixing styling gaps so text boxes, color pickers, checkboxes, and paired fields display cleanly and consistently, matching the other forms in the app. (#152)

## Campaigns

- **[Feature]** **Bringing the Campaigns area to New Adsmith Frontend** — Campaign management isn't in the new platform yet. This high-priority work will let you view, create, edit, and configure campaigns — including offer groups, offer handling, and marketing partners — just like the legacy system. (#200)

## Users

- **[Task]** **Reviewing what the Users area still needs** — We're comparing the new Users screens against the old system to spot missing features — like bulk actions, last-login info, and password options — and prioritize what to add next. (#80)

## Link Testing

- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you back on the dashboard with no explanation. Once fixed, you'll see a proper failure message so you know the link didn't work. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d6062d17d4712f18c8e541a2714f6584c3d1d88f2c6a86112172a16bd86f7f7d -->
