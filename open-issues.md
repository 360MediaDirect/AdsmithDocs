# Open Issues — Plain-Language Overview

_Last updated 2026-07-10 21:23:15 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record to edit it, others will see it's locked and by whom, and if a record was changed while you had it open, you'll be prompted to reload instead of accidentally wiping out someone else's work. This will apply to every editable screen (Offers, Flows, Placements, Advertisers, and more). (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when across the app — manual edits and automated changes alike — so you can finally answer "who changed this offer, and when?" with a filterable view and a history tab on each record. (#276)
- **[Feature]** **Remove admin settings that don't actually do anything** — Several controls quietly save but have no effect today (an Advertiser "Web Presence" tab, a couple of user-permission toggles, and some Data-Client and Pre-Ping options). These will be hidden or removed so the screens only show settings that truly work. (#296)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-sharing page has no equivalent yet; this is a check on whether anyone still needs it, then either rebuilding it or formally retiring it. (#328)
- **[Task]** **Bring the Users area up to par with the old system** — A review comparing the old and new Users screens to catch missing capabilities (bulk role changes, select-all, last-login and two-factor status columns, password entry on new users, and more) so the new Users area is complete. (#80)
- **[Bug]** **Invalid links should show a clear error** — When you test a link that isn't valid, you'll get a proper error message instead of being unexpectedly dropped onto the Dashboard. (#239)

## Offers & Placements

- **[Bug]** **Success tracking pixels now actually fire** — Conversion pixels set up on an offer currently never fire because of a format mismatch, silently losing attribution. This fix makes configured success pixels work end-to-end. (#297)
- **[Bug]** **Saved offer settings will reach the live experience** — A number of saved offer options (including modal settings, display URL, and several data-client flags) are dropped before they reach visitors. This ensures each saved option is either applied or cleaned up so nothing is quietly ignored. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — Offers that fire automatically currently ignore age, gender, state, zip, and device targeting, so they can reach people they should exclude. This work confirms the correct behavior and makes those offers honor the same targeting rules as everything else. (#333)
- **[Feature]** **Preview your unsaved changes** — On Placement and Offer edit pages, the Preview button will show your current edits rather than the last saved version, so you can check a change before saving. (#292)
- **[Feature]** **Performance projections for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical offer data, giving a data-driven read at intake instead of relying on a manual gut-check. (#322)

## Surveys

- **[Feature]** **Make sure every Design setting actually shows up** — A thorough check that each customization option on the design tabs is fully connected from the form through to what visitors see, with any dead or unwired options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Several Placement design settings (like survey height and display format) are saved but not yet reflected in the live survey widget. This wires the remaining ones through or removes any that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back after-success delivery behaviors** — Post-conversion delivery and redirect steps from the old system weren't carried over. This adds a flexible, configurable way to handle them so those clients behave as before. (#327)
- **[Feature]** **Restore per-client pre-ping validation** — Custom serve-time checks that hundreds of data clients relied on aren't running on the new platform yet. This work reconnects those validation rules so leads are checked the way they were before, with safe fallbacks. (#338)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — Every field on the Modal Design tab currently saves but has no effect on the visitor's modal. These will either be built into the modal (headers, progress bar, etc.) or removed so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or stack awkwardly compared to other forms. This is a careful visual cleanup so text boxes, color pickers, checkboxes, and paired fields look consistent and lined up. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — Campaign management (creating and editing campaigns, offer groups, CTA text, offer handling, and marketing partners) exists in the old admin but isn't in the new one yet. This is a high-priority build to restore that core capability. (#200)

## Dashboard & Reports

- **[Task]** **Confirm dashboard numbers match the old system** — Reviewers noticed report figures didn't line up with the legacy app. This investigation compares the two over a fixed date range, pinpoints where any difference comes from, and either fixes it or confirms the numbers are correct. (#271)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a copy of New Adsmith Frontend running against production-like data for testing, locked to read-only so no real data can be changed. (#270)
- **[Feature]** **Automatically turn discussions into tracked tasks** — An internal helper that reads team conversations and files the resulting to-dos as tracked items automatically, reducing manual note-taking and follow-up. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
