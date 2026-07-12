# Open Issues — Plain-Language Overview

_Last updated 2026-07-12 21:16:58 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Task]** **Bringing the Users area up to par with the old system** — A review of the Users screens found several familiar features from the previous system that aren't in New Adsmith Frontend yet (like bulk role changes, select-all checkboxes, last-login and two-factor details, and a password field when adding a user). Once addressed, managing user accounts will feel more complete and familiar. (#80)
- **[Feature]** **Warning when two people edit the same record** — If a colleague is already editing an offer, flow, placement, or other record, you'll see a clear "locked by" notice, and the app will stop two people from accidentally overwriting each other's changes. (#267)
- **[Feature]** **Searchable history of every change** — A new admin Audit Log will record who changed what and when — across offers, placements, advertisers, and more — including automated updates, so you can quickly answer "who changed this and when." (#276)
- **[Feature]** **Cleaning up controls that don't do anything** — Some settings (on Advertisers, Users, Data Clients, and Pre-Pings) currently save but have no effect. These will be removed, hidden, or properly wired up so what you see on screen actually works. (#296)
- **[Bug]** **Invalid links should show an error, not the dashboard** — When you test a link that isn't valid, you'll get a clear failure message right in the Link Testing tool instead of being dropped onto the dashboard. (#239)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-sharing page hasn't been rebuilt. This is a quick decision on whether anyone still needs it or it can be retired for good. (#328)

## Offers
- **[Bug]** **Success pixels that quietly never fire** — Conversion tracking pixels set up on offers currently don't fire at all due to a formatting mismatch, meaning lost attribution. This fix makes configured success pixels fire reliably. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of offer options (including Modal-tab fields, Display URL, and several data-client flags) are saved but dropped before they reach visitors. Each will be either properly delivered or cleaned up so what you configure is what runs. (#295)
- **[Task]** **Auto-register offers ignoring audience targeting** — Auto-register offers currently fire for every visitor, even ones they should exclude by age, gender, state, ZIP, or device. This work makes them respect the same targeting rules as regular offers (or documents the difference on purpose). (#333)
- **[Feature]** **Preview your unsaved changes on Offers and Placements** — The Preview button will show the edits you've just made rather than the last-saved version, so you can check a change before committing it. (#292)
- **[Feature]** **Predicting how a new offer will perform** — An exploratory tool to automatically estimate a new offer's likely performance based on your historical offer data, replacing today's manual gut-check review. (#322)

## Surveys & Widget Display
- **[Feature]** **Making sure design-tab settings actually show up** — A full check across all screens to confirm every look-and-feel option you set on the Design tab is genuinely reflected in the live survey, with any dead options fixed or removed. (#288)
- **[Feature]** **Finishing the Placement Design settings** — Several Placement Design options (like iframe height and display format) are saved but not yet shown to visitors. These will be wired through or removed so no setting is left doing nothing. (#293)
- **[Feature]** **Wiring up or removing the Modal Design tab** — The entire Modal Design tab currently has no effect on what visitors see. This work will either make those header and progress-bar settings work or remove the tab if it isn't needed. (#294)

## Data Clients & Pre-Pings
- **[Feature]** **Bringing back after-success delivery for data clients** — Post-conversion delivery and redirect behavior from the old system will be rebuilt as a reusable, configurable option, so affected data clients keep working as before. (#327)
- **[Feature]** **Restoring per-client pre-ping checks** — Custom serve-time validation used by hundreds of data clients isn't running on the new platform yet. This restores those checks so leads are validated the way they were before, with safe fallbacks if anything goes wrong. (#338)

## Reports
- **[Task]** **Confirming dashboard numbers match the old system** — Investigating why some dashboard report figures differed from the legacy system during testing, so you can trust that the numbers line up. (#271)

## Flows
- **[Task]** **Tidying up the look of the Flow form** — Parts of the Flow form appear unstyled or stacked awkwardly. This ongoing cleanup will make text boxes, color pickers, checkboxes, and paired fields look consistent with the other forms. (#152)

## Campaigns
- **[Feature]** **Bringing the Campaigns module to the new platform** — A high-priority rebuild of campaign management, letting you create, edit, and configure campaigns and offer groups just like in the old admin. (#200)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging version of New Adsmith Frontend using production-like data so features can be verified without any risk of changing real records. (#270)
- **[Feature]** **Turning conversations into tracked to-dos automatically** — A helper that reads team conversations and files the resulting action items for the team, reducing manual note-taking. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
