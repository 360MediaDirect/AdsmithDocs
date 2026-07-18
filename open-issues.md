# Open Issues — Plain-Language Overview

_Last updated 2026-07-18 01:33:19 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels sometimes don't fire** — When an advertiser sets up conversion tracking pixels to fire after a successful lead, they currently never actually fire, which means conversions can go uncounted. This high-priority fix makes those pixels work reliably so you don't lose credit for results. (#297)
- **[Bug]** **Some offer settings never reach the live ad** — Several options you can fill in on an offer (including its Modal-tab fields, Display URL, and certain data delivery flags) are saved but quietly ignored when the ad runs. This work makes each saved setting either take effect or be removed so the form only shows options that truly do something. (#295)
- **[Task]** **Auto-register offers should respect targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting, so they can reach people they were meant to exclude. This makes them honor the same targeting rules as regular offers (or clearly document any intended exception). (#333)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This field on the offer Delivery tab is saved but has no effect when ads are served. The team is confirming what it should do before wiring it up, so it either works as intended or is cleaned up. (#351)
- **[Feature]** **Preview shows your unsaved edits** — On placement and offer edit pages, the Preview button will show the changes you're currently making instead of only the last saved version, so you can check your work before saving. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your own historical offer data, giving Kurt a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Surveys

- **[Feature]** **Make sure every survey design option actually works** — A full review across all entities to confirm that each customization you set on a design tab truly shows up in the live survey, with any options that lead nowhere fixed or removed. (#288)
- **[Feature]** **Finish connecting placement design settings** — Several placement Design-tab options (like survey height and display format) are saved but don't yet change the live widget. This finishes wiring them so your choices take effect. (#293)

## Data Clients

- **[Feature]** **Bring over post-success delivery behavior** — The legacy after-success steps (post-conversion delivery and redirects) that certain clients rely on are being rebuilt in New Adsmith Frontend so those behaviors keep working. This is nearly complete. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients used custom serve-time validation that isn't running on the new platform yet. This high-priority work brings those checks over so leads are validated as they were before. (#338)

## General / Across the App

- **[Feature]** **Remove buttons and settings that don't do anything** — Several admin controls (an Advertiser Web Presence tab, some user permission toggles, and a few data-client and pre-ping options) are shown but have no effect. Hiding or removing them prevents confusion and false expectations about what they control. (#296)
- **[Task]** **Compare the old and new Users areas** — A detailed review of the Users screens to spot anything the older system offered that the new one doesn't yet, such as bulk role changes and login/security details, so nothing important is missing. (#80)

## Behind the Scenes

- **[Task]** **Test environment using real-world data** — Setting up a safe, read-only copy of the app loaded with production-like data so the team can verify behavior without any risk of changing live information. (#270)
- **[Feature]** **Turn conversations into tracked to-dos automatically** — A helper that reads team chat discussions and files the resulting action items for the team, replacing today's manual copy-and-paste process. (#272)

## Reports

- **[Task]** **Investigate mismatched dashboard numbers** — Reviewers noticed some dashboard report figures didn't match the older system. This work pins down where the difference comes from and confirms the numbers you see can be trusted. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — The Modal Design tab's settings (header titles, colors, progress bar) currently have no effect on what visitors see. This makes them take effect or removes the tab so it isn't misleading. (#294)

## Properties

- **[Bug]** **Domain allowlist should actually block other sites** — When a publisher lists which website domains are allowed to serve their ads, that list isn't being enforced today, so any site can serve them. This fix honors the allowlist so ads only run where they're permitted. (#350)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned, with fields stacking oddly instead of sitting side by side. This gives the form the same polished, consistent look as the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
