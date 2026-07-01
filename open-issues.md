# Open Issues — Plain-Language Overview

_Last updated 2026-07-01 05:31:52 UTC · 11 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker for the dashboard filter** — Choosing "Custom" on the date filter will finally open a proper start-and-end date picker, so you can view dashboard data for any specific range instead of only the preset options like Today or This Month. (#58)
- **[Feature]** **Pick report dates right from the dashboard** — You'll be able to change the reporting range using controls built into the dashboard toolbar, with no need to hand-edit the web address. Daily and custom ranges become easy to pull, and links stay shareable. (#268)
- **[Task]** **Confirming dashboard report numbers match the previous system** — We're reviewing why some dashboard report totals differed from the old platform, tracking down the cause, and making sure the numbers you see are accurate and consistent. (#271)

## Behind the Scenes

- **[Task]** **A safe testing environment with recent data** — We're setting up a separate practice environment loaded with May and June data so reports and new features can be checked thoroughly without ever touching your live information. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — An internal helper will capture action items from team chats and log them as work items, so requests are recorded consistently and nothing gets lost. (#272)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — We're fixing styling gaps so the Flow form's text boxes, color pickers, checkboxes, and paired fields display cleanly and line up side by side, matching the polished look of the Placement and Modal forms. (#152)

## Placements

- **[Feature]** **Better control over the offers in a placement** — New placements will default to your manually arranged offer order (so the order you set actually sticks), and you'll be able to filter the available offers list by category to find the right ones faster. (#275)

## Campaigns

- **[Feature]** **Bringing the Campaigns module to the new platform** — Campaign management isn't available yet in New Adsmith Frontend. This adds it back, letting you view, create, edit, and configure campaigns and their offer groups just like in the older system. This is a high-priority, core piece of functionality. (#200)

## Users

- **[Task]** **Reviewing what the Users area still needs** — We're comparing the new Users screens against the older version to spot missing pieces — like bulk actions, extra columns, and login-related details — so we can prioritize bringing them over. (#80)

## General / Across the App

- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when across offers, placements, advertisers, and more (including automated updates), so administrators can easily answer "who changed this and when." (#276)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently sends you to the dashboard with no explanation. This fix shows a clear failure message instead, so you know right away that the link didn't work. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 18c895dd2d51d67625ab25b86c398b76285d058485c5365f84641d856758854b -->
