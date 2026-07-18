# Open Issues — Plain-Language Overview

_Last updated 2026-07-18 10:28:21 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on placements and offers** — When editing a placement or offer, the Preview button will show your current edits right away, so you can check how a change looks without having to save first. (#292)
- **[Bug]** **Some saved offer options don't reach live ads** — A number of offer settings (including modal fields, "Force More Info Visible," Display URL, and several data-client options) are saved but currently never make it to what visitors see. This fix makes sure the options you set actually take effect, or removes any that are no longer needed. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — High priority: conversion pixels set up on offers to fire on success currently never fire, which means lost tracking with no warning. This fix makes those pixels work as configured. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — High priority: auto-register offers currently fire for every visitor even when age, gender, state, zip, or device targeting should exclude them. This fix ensures these offers respect the same audience rules as regular offers. (#333)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This offer setting is saved but has no effect when serving ads. The work will confirm what it's meant to do and either make it work or remove it, so the form doesn't imply behavior that isn't there. (#351)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool to estimate a new offer's likely performance based on your historical offer data, replacing the current informal manual gut-check with a data-driven projection. (#322)

## General / Across the App

- **[Task]** **Match up the Users area with the older system** — A review comparing the new Users screens against the legacy version to spot missing capabilities (like bulk role changes, last-login and two-factor status, and password entry when adding a user) so the new area can catch up. (#80)
- **[Feature]** **Remove admin controls that do nothing** — Several settings that are saved but never actually applied (Advertiser Web Presence fields, certain user permission toggles, and some Data-Client and Pre-Ping options) will be hidden or removed so the admin area only shows controls that truly work. (#296)

## Surveys

- **[Feature]** **Make every design option actually take effect** — A full check across all entities to confirm each design and form option you set is reflected in the live survey, with any settings that don't do anything either wired up or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Several Placement design-tab options (like survey height and display format) are saved but aren't yet shown to visitors. This finishes hooking them up so your choices appear as intended. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring over post-success delivery steps from the old system** — Behaviors that ran after a successful conversion in the legacy system will be carried over so post-conversion delivery keeps working on New Adsmith Frontend. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — High priority: custom validation checks that ran before serving for hundreds of data clients aren't running on the new platform yet. This work reconnects those checks so those clients are validated as expected. (#338)

## Modals

- **[Feature]** **Make the Modal design settings work (or remove them)** — The Modal Design tab's header and progress-bar fields are saved but don't currently show up in the visitor modal. They'll either be displayed as intended or removed from the form. (#294)

## Reports & Dashboard

- **[Task]** **Confirm dashboard numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy app, to pin down the cause and make sure reporting numbers are accurate and trustworthy. (#271)

## Properties

- **[Bug]** **Make the domain allowlist actually block other sites** — A property's allowed-domains list is saved but not enforced, so ads can currently serve on any site. This fix ensures ads only serve on the domains you've approved. (#350)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with some paired fields stacking vertically instead of side by side. This tidies up the form so it looks consistent with the other screens. (#152)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of the app running against prod-like data for validation, locked to read-only so testing can't change real records. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels and automatically files action items as tracked issues, cutting out manual copy-paste when capturing follow-ups from meetings. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
