# Open Issues — Plain-Language Overview

_Last updated 2026-07-01 14:58:38 UTC · 11 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker on the Dashboard** — Choosing "Custom" from the date filter will open a proper start-and-end date picker, so you can view Dashboard data for any range you like instead of just the preset options. (#58)
- **[Feature]** **Pick report dates right from the Dashboard toolbar** — You'll be able to pull daily or custom-range reports using controls built into the Dashboard, with no need to hand-edit the web address. Links you share will still reflect the range you picked. (#268)
- **[Task]** **Make Dashboard report numbers match the legacy system** — We're investigating why some Dashboard report figures don't line up with the older system so we can pin down the cause and confirm the numbers you see are accurate. (#271)

## Behind the Scenes

- **[Task]** **A safe testing environment with May & June data** — We're setting up a separate practice environment loaded with recent data so reports can be checked thoroughly without any risk to your live information. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper will read designated Slack channels and automatically log follow-up tasks, so needs raised in conversation get captured without manual copying. (#272)

## Users

- **[Task]** **Filling gaps between the old and new Users area** — We've compared the current Users screens against the legacy version and are prioritizing the missing pieces (like bulk actions, extra columns, and password options) so the new Users area matches what you're used to. (#80)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — We're correcting styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields display neatly and consistently, matching the polished look of other forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns area to the new platform** — A high-priority addition that lets you view, create, edit, and manage campaigns and their offer groups directly in New Adsmith Frontend, just as you can in the legacy admin. (#200)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on Placements** — We're looking at defaulting new placements to your manual offer order (so the order you set is actually used) and adding a way to filter the available offers list by category, making it faster to find the right offers. (#275)

## Link Testing

- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper failure message instead of quietly sending you to the Dashboard, so you'll immediately know the link didn't work. (#239)

## Audit Log

- **[Feature]** **A searchable history of who changed what** — We're introducing an Audit Log that records every change to offers, placements, advertisers, and more — including automated ones — with a timestamp and who made it, so administrators can easily trace and troubleshoot changes. (#276)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 18c895dd2d51d67625ab25b86c398b76285d058485c5365f84641d856758854b -->
