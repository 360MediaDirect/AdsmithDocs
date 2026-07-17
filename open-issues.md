# Open Issues — Plain-Language Overview

_Last updated 2026-07-17 15:27:21 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on placements and offers** — When editing a placement or offer, the Preview will show your current, in-progress changes instead of only the last saved version, so you can check your work before committing it. (#292)
- **[Bug]** **Saved offer options now reach the live experience** — Several offer settings you fill in (including modal-related fields, "Force More Info Visible," and Display URL) are currently dropped before they reach visitors. This fix makes sure the options you set actually take effect. (#295)
- **[Bug]** **Success tracking pixels will fire correctly** — A high-priority fix: conversion pixels set up on offers currently never fire, meaning conversions go untracked with no error shown. Once resolved, configured success pixels will fire reliably so attribution and revenue signals aren't lost. (#297)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform, based on your own historical offer data, replacing the manual gut-check review. It would give the team a data-driven read on new offers at intake. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — A high-priority fix: auto-register offers currently ignore age, gender, state, zip, and device targeting and can fire for visitors who should be excluded. This work makes them honor the same targeting rules as regular offers (or documents the difference deliberately). (#333)

## Surveys

- **[Feature]** **Design settings that actually take effect everywhere** — A full check across all entities to make sure every option on the Design tab is reflected in the live survey, with no settings that quietly do nothing. You'll be able to trust that the customizations you choose really show up. (#288)
- **[Feature]** **Finish connecting Placement Design options to the survey** — Several placement Design-tab settings (like iFrame height and display format) are saved but don't yet affect the live survey. This wires them through so your choices display, or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior for clients** — Certain after-success delivery/redirect behaviors from the legacy system weren't carried over. This brings them back so affected clients continue working as before. (#327)
- **[Feature]** **Restore client-specific pre-ping checks** — A high-priority gap: custom serve-time validation used by 448 clients isn't running on the new platform. This work restores those checks so client-specific screening happens as expected before delivery. (#338)

## General / Across the App

- **[Task]** **Compare the old and new Users area to close gaps** — A review of the legacy Users management against the new one, identifying missing capabilities (like bulk actions, last-login and two-factor status, and role changes) so the new Users area can catch up. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Some settings across the app (Advertiser Web Presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no effect. These will be hidden or removed so the admin screens only show controls that actually work — or scheduled to be made functional. (#296)

## Behind the Scenes

- **[Task]** **Read-only test environment for safe verification** — Setting up a staging version of New Adsmith Frontend that mirrors real data but can't be changed, so the team can validate the product against realistic data without any risk to live information. (#270)
- **[Feature]** **Automatic issue capture from team chats** — A helper that reads designated chat conversations and turns action items into tracked to-do items automatically, reducing manual copy-paste and keeping work from slipping through the cracks. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — Every field on the Modal Design tab (header text, colors, progress bar) is currently saved but never shown to visitors. This work either makes those settings display in the visitor modal or removes the tab so it doesn't mislead. (#294)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly and plain-looking inputs. This cleanup brings the form's appearance in line with the Placement and Modal forms for a more polished, consistent experience. (#152)

## Dashboard / Reports

- **[Task]** **Confirm dashboard report numbers match the old system** — Reviewers noticed dashboard figures that didn't line up with the legacy app. This investigation pins down where any differences come from and confirms the numbers are accurate and trustworthy. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->
