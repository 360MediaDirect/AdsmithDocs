# Open Issues — Plain-Language Overview

_Last updated 2026-07-13 14:58:56 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes on Offers and Placements** — When editing an offer or placement, the Preview button will show exactly what you've just changed, so you no longer have to save first to see how an edit looks. (#292)
- **[Bug]** **Some saved offer settings never reach the live experience** — A fix so that offer options you set (including modal-related and "more info" settings) actually show up for visitors instead of being quietly ignored. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — A high-priority fix so the conversion pixels you configure on an offer actually fire when a lead succeeds, protecting your attribution and revenue tracking. (#297)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your own historical data, replacing today's manual gut-check review. (#322)
- **[Task]** **Auto-register offers are ignoring visitor targeting** — A high-priority fix so auto-register offers respect age, gender, state, zip, and device targeting rules and don't fire for visitors they should exclude. (#333)

## General / Across the App

- **[Feature]** **Warn when two people edit the same record** — You'll see a clear "locked by someone else" notice and be protected from accidentally overwriting a colleague's changes when you both open the same record. (#267)
- **[Feature]** **Searchable activity history across the app** — A new admin log that records who changed what and when — manual edits and automated changes alike — so you can finally answer "who changed this and when." (#276)
- **[Feature]** **Clean up controls that don't do anything** — Removing or hiding admin settings (some Advertiser web-presence, user permission, Data-Client, and Pre-Ping fields) that currently look like they work but have no effect, reducing confusion. (#296)
- **[Task]** **Decide the future of the Users screen** — A review comparing the older Users area with the new one to confirm which features still need to be carried over. (#80)
- **[Task]** **Decide whether to keep the old file-share page** — A keep-or-retire decision on a legacy file-sharing page that has no equivalent in the new product yet. (#328)

## Surveys

- **[Feature]** **Make every Design tab option actually take effect** — A full check across all entities to ensure the customizations you set on Design tabs are reflected in the survey visitors see, with no dead settings. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey** — Remaining Placement design options (like survey height and display format) will properly show up in the live survey instead of being saved but ignored. (#293)
- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design settings (header text, colors, progress bar) will either display for visitors or be removed so they don't mislead. (#294)

## Data Clients & Pre-Pings

- **[Feature]** **Restore after-success delivery for data clients** — Bringing over the post-conversion delivery and redirect behavior from the older system so client hand-offs work as they did before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — A high-priority effort to bring back the per-client validation that runs before serving, so hundreds of data clients get the checks they had in the old system. (#338)

## Dashboard & Reports

- **[Task]** **Confirm report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy app, so you can trust the numbers you see. (#271)
- **[Bug]** **Invalid links should show an error, not the dashboard** — When you test a bad link, you'll get a clear failure message instead of being unexpectedly sent to the dashboard. (#239)

## Behind the Scenes

- **[Task]** **Set up a safe test environment** — Behind-the-scenes work to run the product against realistic data in a view-only mode for testing, with no risk of changing real records. (#270)
- **[Feature]** **Turn Slack conversations into tracked to-dos automatically** — A helper that reads designated Slack chats and files action items for the team, cutting out manual copy-and-paste. (#272)

## Flows

- **[Task]** **Tidy up the appearance of the Flow form** — Styling fixes so the Flow form's text boxes, color pickers, checkboxes, and paired fields look consistent and polished like the other forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — A critical, high-priority addition so you can view, create, edit, and configure campaigns and offer groups directly in New Adsmith Frontend, just like the older admin. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
