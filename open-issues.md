# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 07:36:18 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes before saving** — On the Offers and Placements edit screens, the Preview button will show exactly what you're currently working on, including edits you haven't saved yet, so you no longer have to save first just to check how something looks. (#292)
- **[Bug]** **Offer options that never reached the live page** — Several saved offer settings (including Modal-tab options, Display URL, and certain data-client settings) weren't being carried through to what visitors actually see. This fix makes sure the options you set on an offer either take effect or are cleanly removed if unused. (#295)
- **[Bug]** **Success tracking pixels weren't firing** — Conversion pixels configured under "Pixels to Fire on Success" were silently not working, meaning some completed conversions went untracked. This fix restores that tracking so your attribution and reporting stay accurate. A high-priority fix. (#297)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check review, new offers could be scored automatically against your own historical offer data to estimate how they're likely to perform. An exploratory improvement to help at offer intake. (#322)
- **[Bug]** **Auto-register offers were ignoring visitor targeting** — Auto-register offers were firing for visitors they should have excluded (based on age, gender, state, zip, or device). This fix makes those offers respect the same targeting rules as regular offers. A high-priority fix. (#333)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When two users open the same record (an offer, flow, advertiser, and so on), you'll now be warned if someone else is editing it or has changed it since you opened it, so one person's work can no longer silently erase another's. (#267)
- **[Feature]** **Cleaning up controls that don't actually do anything** — Some admin settings (such as the Advertiser Web Presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping options) were saved but had no real effect. These will be removed or hidden so the screens only show controls that truly work. (#296)
- **[Bug]** **Invalid link tests should show a clear error** — When testing a link that isn't valid, you were unexpectedly dropped onto the dashboard. This fix will show a clear failure message instead, so you know the link didn't pass. (#239)
- **[Task]** **Decide the future of the file-share page** — The old file-share page hasn't been rebuilt in New Adsmith Frontend. This is a review to decide whether it's still needed or can be retired. (#328)

## Surveys

- **[Feature]** **Design settings that fully match the live survey** — Every customization option on the Design tab will be checked to make sure it actually shows up in the survey visitors see, with any options that don't do anything either fixed or removed across all screens. (#288)
- **[Feature]** **Finishing the Placement Design settings** — A handful of Placement Design-tab options (like survey height and display format) weren't yet affecting the live survey widget. This work makes each of those settings take effect or removes it if it's not needed. (#293)

## Data Clients

- **[Feature]** **Post-conversion delivery steps carried over from the old system** — The "after-success" delivery and redirect behavior used by some clients hadn't been rebuilt in New Adsmith Frontend. This restores that step so those clients keep working as before. Nearly complete. (#327)
- **[Feature]** **Rebuilding the older per-client pre-ping checks** — Many data clients relied on custom validation checks from the old system that don't currently run. This work restores those serve-time checks so those clients are validated the way they used to be. A high-priority, large effort. (#338)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a testing environment that mirrors live data but can't change anything, so the team can verify the product against realistic data without risk. (#270)
- **[Feature]** **Turning meeting discussions into tracked work automatically** — A helper that reads team conversations and files the resulting to-do items automatically, reducing manual copy-and-paste when logging new work. (#272)

## Modals

- **[Feature]** **Making the Modal Design tab do what it says** — The Modal Design tab's options (headers, colors, progress bar) currently don't appear in the modal visitors see. This work will either make those settings take effect or remove the tab if it isn't needed. (#294)

## Reports

- **[Task]** **Confirming report numbers match the old system** — Some dashboard report totals didn't line up with the legacy system during testing. This investigation will pinpoint why and either correct the numbers or confirm they're accurate. (#271)

## Users

- **[Task]** **Comparing the Users area to the old system** — A review of the Users screens against the previous version to spot anything missing (like bulk actions, last-login info, or two-factor status) and prioritize what to add. Well underway. (#80)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with some paired fields stacking awkwardly. This cleanup brings the form's appearance in line with the Placement and Modal forms. Partly done. (#152)

## Campaigns

- **[Feature]** **Bringing the Campaigns module to New Adsmith Frontend** — Campaign management from the old system isn't available yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups. A critical, high-priority feature. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f12be1691f4d05be7a51684fc6fe5ab6d4c4751d5a9de6a600395df673d554b3 -->
