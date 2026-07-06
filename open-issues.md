# Open Issues — Plain-Language Overview

_Last updated 2026-07-06 09:20:45 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record at once, New Adsmith Frontend will warn you and prevent one person's changes from silently wiping out the other's. Whoever isn't editing sees a clear "locked by…" notice. (#267)
- **[Feature]** **Searchable history of every change** — A new admin activity log will record who changed what (and when) across offers, placements, advertisers, and more — including automatic system changes — so you can answer "who edited this?" with confidence. (#276)
- **[Feature]** **Clean-up of settings that don't do anything** — Several admin fields (an advertiser's Web Presence links, some user-permission toggles, and a few data-client and pre-ping options) currently save but have no effect. They'll be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Bringing the Users area up to par with the old system** — A review comparing the new Users screens to the legacy version, identifying missing pieces (like bulk actions and last-login info) so nothing important is lost in the move. (#80)
- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link will now show a proper error message instead of quietly sending you back to the dashboard. (#239)

## Surveys

- **[Feature]** **Design choices that actually show up** — Making sure every customization on the Design tab is reflected in the live survey, plus a full check across all screens to catch any settings that currently do nothing. (#288)
- **[Bug]** **Survey styling settings that finally take effect** — Most of the survey appearance and behavior options (colors, buttons, header text, legal text, progress bar, and more) are saved today but don't change what visitors see. This work makes them work as expected. (#290)
- **[Bug]** **Missing voucher code and info links restored** — On the live survey page, the voucher code line and the privacy/terms/details links (which appear correctly in the old app) will show again — important for both the visitor experience and compliance. (#291)
- **[Feature]** **Finishing the remaining survey design settings** — A follow-up pass to wire up the last few Design-tab options (like survey height and display format) or remove any that aren't needed, so no setting is left doing nothing. (#293)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button lets you download the breakdown-by-day view for use in a spreadsheet. High priority. (#286)
- **[Task]** **Confirming dashboard numbers match the old system** — An investigation into why some dashboard report figures didn't line up with the legacy app, so you can trust that the new reports are accurate. (#271)

## Placements

- **[Feature]** **Smarter offer ordering and filtering** — Manually arranged offers will actually be served in that order by default, and you'll be able to filter the available-offers list by category instead of only searching by text. (#275)
- **[Feature]** **Preview your unsaved changes** — On placement and offer edit screens, Preview will show your current edits rather than the last-saved version, so you can check a change before committing it. (#292)

## Modals

- **[Feature]** **Modal Design tab wired up or removed** — The modal's header and design settings are saved today but don't affect what visitors see. They'll either be made to work or removed so the tab reflects reality. (#294)

## Offers

- **[Bug]** **Saved offer settings reaching the live widget** — Several offer options are saved in the admin but never make it to the live experience. This ensures each one either takes effect or is cleaned up so nothing is misleading. (#295)

## Campaigns

- **[Feature]** **Campaigns module coming to the new platform** — The Campaigns area from the old admin — creating and editing campaigns, offer groups, and offer settings — isn't yet available in New Adsmith Frontend. This adds it back so campaign management can happen here. High priority. (#200)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of New Adsmith Frontend using production-like data for verification, locked to read-only so testing can't change anything real. (#270)
- **[Feature]** **Turning conversations into tracked work items** — A helper that reads team discussions in Slack and files them as tracked issues automatically, reducing manual note-taking. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
