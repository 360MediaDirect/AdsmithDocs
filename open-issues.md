# Open Issues — Plain-Language Overview

_Last updated 2026-07-01 12:55:32 UTC · 11 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker for the dashboard** — Choosing "Custom" on the dashboard date filter will now open a proper start-and-end date picker, so you can view results for any specific stretch of time instead of only the preset options like Today or This Month. (#58)
- **[Feature]** **Pick report dates right from the dashboard** — You'll be able to change the reporting date range using controls built into the dashboard itself, with no need to edit the web address by hand. Your chosen range is still saved in the link so you can share or bookmark it. (#268)
- **[Task]** **Making sure dashboard numbers match the old system** — We're comparing report figures between the previous system and New Adsmith Frontend to track down and explain any differences, so you can trust that the numbers you see are accurate. (#271)

## Behind the Scenes

- **[Task]** **A safe testing environment with recent data** — We're setting up a separate practice environment loaded with May and June data so the team can validate reports and features without ever touching your live information. (#270)
- **[Feature]** **Turning chat discussions into tracked work automatically** — A new helper will read designated team conversations and automatically log action items as tracked tasks, so requests raised in meetings are captured without manual copying. (#272)

## Flows

- **[Task]** **Polishing the look of the Flow form** — We're cleaning up the styling on the Flow form so text boxes, color pickers, checkboxes, and paired fields display neatly and consistently, instead of looking plain or stacking awkwardly. Part of this is done, with a careful final pass still to come. (#152)

## Placements

- **[Feature]** **Better control over offer order and filtering in Placements** — Building on recent improvements, we're looking at making new placements respect your manual offer order by default and adding a way to filter the available offers list by category, so it's faster to find and arrange the offers you want. (#275)

## Campaigns

- **[Feature]** **Bringing the Campaigns area to New Adsmith Frontend** — The Campaigns module from the older admin system isn't available yet. We're building it so you can view, create, edit, and configure campaigns and their offer groups directly in New Adsmith Frontend. This is a high-priority, core feature. (#200)

## Link Testing

- **[Bug]** **Clear error when testing an invalid link** — Right now, testing a bad link quietly sends you to the dashboard. This fix makes the Link Testing screen show a clear failure message instead, so you know the link didn't work. (#239)

## Users

- **[Task]** **Reviewing what's missing from the Users area** — We're comparing the Users screens against the older system to spot gaps like bulk actions, additional columns, and extra filters, so we can prioritize bringing back the tools you rely on. This is a review-and-planning effort. (#80)

## Audit

- **[Feature]** **A searchable history of every change** — We're building an audit log that records who changed what and when across the app — offers, placements, advertisers, and more — including automated changes. Administrators will get a searchable page and per-record history, making it easy to answer "who changed this?" (#276)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 18c895dd2d51d67625ab25b86c398b76285d058485c5365f84641d856758854b -->
