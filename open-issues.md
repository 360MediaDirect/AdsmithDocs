# Open Issues — Plain-Language Overview

_Last updated 2026-07-12 11:25:15 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Warn when two people edit the same record at once** — When you open a record to edit, New Adsmith Frontend will hold your place and show a clear "someone else is editing this" message, so two people can no longer accidentally overwrite each other's changes. (#267)
- **[Feature]** **Searchable history of every change (Audit Log)** — A new Audit Log will record who changed what and when across offers, placements, advertisers, and more — including automatic system changes — so you can look up exactly what happened and when. This is a larger, high-value new feature. (#276)
- **[Feature]** **Clean up buttons and fields that don't do anything** — Several settings that look active but currently have no effect (an Advertiser "Web Presence" tab, certain user permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden, so what you see reflects what actually works. (#296)
- **[Bug]** **Invalid link now shows a proper error** — When you test a link that isn't valid, you'll see a clear error message instead of being unexpectedly sent to the dashboard. This fix is nearly complete. (#239)
- **[Task]** **Match the new user management to the old system** — A review comparing the older Users area with the new one, so missing capabilities (like bulk role changes and login/security details) can be planned and added. (#80)
- **[Task]** **Decide the future of the old file-sharing page** — A quick review to confirm whether the legacy file-share page is still needed, so it's either rebuilt in the new admin or formally retired. (#328)

## Offers

- **[Bug]** **Success tracking pixels now fire correctly** — Conversion pixels set up on offers currently never fire, meaning credit for successful conversions is being lost. This high-priority fix makes configured success pixels work as intended. (#297)
- **[Bug]** **Offer settings that weren't reaching the live experience** — Several saved offer options (including modal settings, a display URL, and various delivery flags) never actually reached visitors. This work makes sure each saved option either takes effect or is removed if unused. (#295)
- **[Task]** **Auto-register offers will respect audience targeting** — Auto-register offers currently ignore age, gender, state, zip, and device targeting and can fire for visitors who should be excluded. This high-priority fix brings them in line with your targeting rules. (#333)
- **[Feature]** **Preview offers and placements with your unsaved edits** — The Preview button will show your in-progress changes right away, so you no longer have to save first just to see how an edit looks. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, replacing today's manual gut-check review with a data-driven projection. (#322)

## Surveys

- **[Feature]** **Design settings will actually change the survey** — A thorough check to ensure every design and customization option you set is reflected in the live survey, with any settings that do nothing either wired up or removed. (#288)
- **[Feature]** **Finish connecting placement design options to the survey** — A handful of placement Design-tab settings (like survey height and display format) don't yet affect the live widget; this connects the remaining options or removes the ones that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore custom pre-lead checks for data clients** — Custom serve-time validation used by hundreds of data clients isn't running on the new platform yet. This high-priority work brings those checks back so leads are validated as they were before. (#338)
- **[Feature]** **Bring back post-conversion delivery for data clients** — The legacy after-success delivery/redirect behavior used by active data clients is being rebuilt as a configurable option, so post-conversion handoffs work again. This is nearly complete. (#327)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the product against production-like data for testing and verification, with safeguards so nothing can be changed by accident. (#270)
- **[Feature]** **Automatic issue creation from team conversations** — An internal helper that turns action items from team chats into tracked tasks automatically, reducing manual note-taking. No direct effect on the product screens. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — Every field on the modal's Design tab currently has no visible effect. This work either makes those header and progress-bar settings appear in the visitor modal or removes the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned (plain textareas, unstyled color pickers, fields stacking instead of sitting side by side). This tidies up the form's appearance to match other screens. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — Campaign management isn't available yet in New Adsmith Frontend. This high-priority work adds the ability to view, create, edit, and configure campaigns and offer groups, matching the older system. (#200)

## Dashboard

- **[Task]** **Confirm dashboard numbers match the old system** — An investigation into why some dashboard report figures differ from the legacy app, so any discrepancy can be explained and fixed and you can trust the numbers. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
