# Open Issues — Plain-Language Overview

_Last updated 2026-07-13 01:33:35 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Task]** **Bring the Users area up to the level of the old system** — We're reviewing everything the previous Users screen could do (bulk role changes, select-all, last-login and two-factor status, and more) and closing the gaps so managing users in New Adsmith Frontend feels complete and familiar. (#80)
- **[Feature]** **Protection against two people overwriting each other's edits** — When someone opens a record you're already editing, you'll see a clear "locked by" note, and you'll be warned before accidentally saving over someone else's changes. This keeps records safe across Offers, Flows, Placements, Advertisers, and more. (#267)
- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every change to your entities (manual or automatic) with the time and the person or system responsible, so you can finally answer "who changed this and when." (#276)
- **[Feature]** **Cleaning up controls that don't do anything** — Some settings currently save but have no effect (certain Advertiser web-presence fields, a few user-permission and data-client options, and a pre-ping setting). We'll remove or hide them so the screens only show controls that actually work. (#296)
- **[Bug]** **Invalid links should show an error, not dump you on the Dashboard** — When you test a bad link, you'll get a clear failure message instead of being unexpectedly sent to the Dashboard. (#239)
- **[Task]** **Decide the future of the old file-share page** — We're confirming whether the legacy file-share feature is still needed and either giving it a home in the new admin or formally retiring it. (#328)

## Offers & Placements
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels you've set up on offers currently never fire, which means lost tracking. This fix makes sure a configured success pixel actually fires, so your attribution is accurate. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several offer options you fill in (including modal fields, display URL, and certain data-client flags) are being dropped before they reach visitors. We'll make sure each one either takes effect or is clearly removed. (#295)
- **[Task]** **Auto-register offers should respect visitor targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting and can fire for people they should exclude. We'll bring them in line with the rules applied to regular offers. (#333)
- **[Feature]** **Preview your unsaved offer and placement changes** — The Preview button will show your current edits before you save, so you can check how a change looks without having to save it first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, new offers could be scored against your historical performance data to estimate how they're likely to perform, giving Kurt a data-backed read at intake. (#322)

## Surveys
- **[Feature]** **Make sure every survey design option actually works** — We're checking that each customization in the Design tab truly shows up in the live survey, and fixing (or removing) any option that currently does nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Several placement Design-tab settings (like iFrame height and display format) don't yet affect the visitor experience. We'll wire them through or remove the ones that aren't needed. (#293)

## Data Clients
- **[Feature]** **Restore post-conversion delivery scripts** — The old "after success" delivery/redirect behavior for clients wasn't carried over. We're bringing it back as a configurable option so post-conversion handoffs work as before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients relied on custom serve-time validation that isn't running on the new platform. We're porting that logic so those checks apply again before offers are served. (#338)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — We're standing up a staging setup using production-like data for verification, locked to read-only so testing can't change real records. (#270)
- **[Feature]** **A Slack helper that turns conversations into tracked tasks** — A new assistant will read designated Slack channels, spot action items, and file them as tracked issues automatically, cutting out manual copy-paste. (#272)

## Modals
- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — The modal header and progress-bar settings currently have no effect on what visitors see. We'll either connect them to the live modal or remove the tab. (#294)

## Flows
- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned (plain textareas, unstyled color pickers, fields stacking instead of sitting side by side). This cleanup brings it in line with the Placement and Modal forms. (#152)

## Campaigns
- **[Feature]** **Bring the Campaigns module to the new platform** — Campaigns aren't available in New Adsmith Frontend yet. This high-priority work adds the ability to view, create, edit, and configure campaigns and their offer groups, matching the old system. (#200)

## Reports
- **[Task]** **Confirm report numbers match the old system** — Some dashboard report figures didn't line up with the legacy app during testing. We're comparing the two over a fixed date range to find any difference, explain it, and confirm the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
