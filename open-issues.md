# Open Issues — Plain-Language Overview

_Last updated 2026-07-07 05:19:29 UTC · 23 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record at once, the app will warn you if someone else changed it and stop your save from quietly wiping out their work. You'll see a clear "locked by" note or a prompt to reload. (#267)
- **[Feature]** **Searchable history of who changed what** — A new Audit Log will record every manual and automatic change across the app — offers, placements, advertisers, flows and more — with the time and the person or system responsible, so you can always see who changed something and when. (#276)
- **[Feature]** **Clean up settings that don't actually do anything** — Several admin controls (like the Advertiser Web Presence fields, some user permission toggles, and a few Data Client and Pre-Ping options) are currently saved but have no real effect. They'll be removed or hidden so the screens only show settings that truly work. (#296)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent in New Adsmith Frontend. This is a quick decision on whether it's still needed or can be retired for good. (#328)
- **[Task]** **Review the Users area against the old system** — A documentation review comparing the old Users management screen with the new one, to spot missing pieces (like bulk role changes and login details) and plan what to add. (#80)
- **[Bug]** **Invalid links should show an error, not the Dashboard** — When you test a link that isn't valid, you'll now get a clear failure message instead of being dropped back on the Dashboard with no explanation. (#239)

## Surveys

- **[Feature]** **Make every survey design option actually work** — A full check to make sure each customization you set in the design tab truly shows up in the live survey, with no "dead" settings that look active but do nothing. (#288)
- **[Bug]** **Design tab settings that don't reach the live survey** — Most of the ~30 survey styling and behavior options (colors, buttons, header, legal text and more) are currently saved but ignored on the visitor-facing survey. This wires them up so what you set is what visitors see. (#290)
- **[Bug]** **Voucher code and info links missing on the live survey** — A configured voucher code line and the privacy/terms/details links are set up correctly in the admin but aren't showing on the new survey page. This fixes their display so they appear as they did before — important for compliance and passing leads. (#291)
- **[Feature]** **Finish the last few survey design settings** — Wraps up the remaining design-tab options that were left incomplete, so settings like survey height and display format take effect (or are removed if not needed). (#293)

## Offers

- **[Bug]** **Some saved offer settings never reach the live page** — A number of offer options (including the Modal-tab fields and "Force More Info Visible") are saved but dropped before they reach visitors. Each will be either made to work or clearly removed, so what you configure is what runs. (#295)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool that estimates a new offer's likely performance based on your historical offer data, giving a data-driven gut-check at intake instead of relying on a manual review. (#322)
- **[Task]** **Auto-register offers should respect visitor targeting** — Auto-register offers currently fire for everyone, ignoring age, gender, state, zip and device targeting. This confirms the correct behavior and makes sure these offers only fire for the right visitors. (#333)

## Placements

- **[Feature]** **Preview your unsaved changes before saving** — The Preview button on placement and offer edit screens will show your current in-progress edits, so you can check how a change looks without having to save it first. (#292)
- **[Feature]** **Bring back banner placements** — The old banner placement template isn't yet available in New Adsmith Frontend. This confirms whether banners are still used and, if so, restores them. (#326)

## Behind the Scenes

- **[Task]** **Set up a safe test environment with real-like data** — A read-only staging setup so the team can verify the product against production-like data without any risk of changing live records. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels and automatically files action items as tracked issues, reducing manual copy-and-paste. (#272)

## Dashboard & Reports

- **[Task]** **Confirm report numbers match the old system** — An investigation into why some Dashboard report figures didn't line up with the legacy app, so you can trust the numbers you see. (#271)

## Modals

- **[Feature]** **Make the Modal design settings work — or remove them** — Every field on the Modal Design tab is currently saved but has no effect on the visitor-facing modal. Each will be wired up to actually change the modal, or removed if it isn't needed. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or awkwardly laid out (plain text boxes, misaligned paired fields). This tidies up the appearance to match the other forms. (#152)

## Data Clients

- **[Feature]** **Restore after-success delivery for certain clients** — The old "after-success" delivery and redirect behavior for specific clients hasn't been carried over yet. This confirms what's still needed and brings it back. (#327)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — Campaign management (creating and editing campaigns, offer groups, CTAs and marketing partners) doesn't exist yet in New Adsmith Frontend. This high-priority work adds it so campaigns can be managed here like in the old admin. (#200)

## Pre-Pings

- **[Feature]** **Restore the older per-client pre-ping** — A legacy pre-ping method isn't available in the new platform, which could affect offers that still rely on it. This confirms which offers need it and brings the missing behavior across. (#330)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 0f0dc75345ae083c3f2607503afd91bf3b9663925bf97592fab1f9e589c4ec62 -->
