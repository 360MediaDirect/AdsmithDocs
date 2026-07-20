# Open Issues — Plain-Language Overview

_Last updated 2026-07-20 17:38:31 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes on placements and offers** — When editing a placement or offer, the Preview button will show your in-progress edits instead of only the last-saved version, so you can check your work before committing to it. (#292)
- **[Bug]** **Success tracking pixels now fire correctly** — A high-priority fix: conversion pixels set up on offers were silently never firing, meaning completed conversions weren't being tracked. Once fixed, your success pixels will fire as configured and attribution will be recorded again. (#297)
- **[Bug]** **Auto-register offers will respect visitor targeting** — A high-priority fix: auto-register offers were being shown to everyone, ignoring your age, gender, state, ZIP, and device targeting rules. This corrects that so these offers only fire for the visitors they're meant for. (#333)
- **[Bug]** **Saved offer options will actually reach the live ad** — Several options you set on an offer weren't making it through to the live experience. This fix ensures the settings you save are the ones visitors actually see. (#295)
- **[Bug]** **"Conflicting Referrals" field will be honored (or removed)** — The Conflicting Referrals field on an offer's Delivery tab is currently saved but has no effect. We'll confirm how it should behave and either make it work or remove it to avoid confusion. (#351)
- **[Feature]** **Automatic performance estimate for new offers** — An exploratory feature to project how a new offer is likely to perform based on your historical offer data, giving you a data-driven gut-check at intake instead of relying on manual review. (#322)

## Data Clients & Pre-Pings

- **[Feature]** **Restore serve-time validation for data clients** — A high-priority effort to bring back the custom pre-ping checks that hundreds of data clients relied on in the older system, so their visitor-validation rules run correctly on New Adsmith Frontend. (#338)
- **[Feature]** **Restore post-conversion delivery steps** — The "after success" delivery and redirect steps used by certain data clients weren't carried over. This brings them back so those clients' post-conversion behavior works as before. (#327)

## Surveys

- **[Feature]** **Make sure every Design tab option actually works** — A full check across all entities to confirm that each customization option you set on the Design tab is truly reflected in the live survey, with any options that do nothing either fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Several Placement Design tab settings (like survey height and display format) weren't taking effect. This wires them through so your choices show up in the widget visitors see. (#293)

## General / Across the App

- **[Feature]** **Remove admin controls that don't do anything** — Some settings (such as the Advertiser Web Presence fields and certain user permission toggles) can be changed but have no real effect. We'll hide or remove them so the admin screens only show controls that actually work. (#296)
- **[Task]** **Close the gaps in Users management** — A review comparing the Users area against the older system to identify missing capabilities (like bulk actions, last-login info, and password setup on new users) so the new Users screens reach full functionality. (#80)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the product loaded with realistic data that can be reviewed without any risk of changing live information. (#270)
- **[Feature]** **Turn Slack discussions into tracked work automatically** — A helper that reads designated Slack conversations, spots action items, and files them as tracked issues automatically, reducing manual copy-and-paste. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The entire Modal Design tab currently saves its settings but none of them appear in the visitor-facing modal. We'll either wire these header and progress-bar options through or remove the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned compared to other forms, with some paired fields stacking awkwardly. This cleanup brings the Flow form's look in line with the rest of the app. (#152)

## Properties

- **[Bug]** **Enforce the domain allowlist on Properties** — Today a Property's allowed-domains list is saved but never enforced, so ads can be served from any website. This fix will block requests from sites that aren't on the list, while leaving Properties that haven't set a list unaffected. (#350)

## Reports & Dashboard

- **[Task]** **Investigate mismatched Dashboard report numbers** — During review, some Dashboard report figures didn't match the older system. This work compares the two over a fixed period to pinpoint why and confirm the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
