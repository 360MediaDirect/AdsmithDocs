# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 21:21:13 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — A high-priority fix: conversion tracking pixels set up on offers currently never fire, which means completed conversions aren't being recorded. Once fixed, the pixels you configure will reliably fire so your attribution and revenue tracking stay accurate. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several options you fill in on an offer (including Modal-tab fields, Display URL, and various data-client flags) aren't being carried through to what visitors actually see. This work makes sure each setting either takes effect or is clearly removed so it isn't misleading. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — A high-priority fix: automatically-registered offers currently ignore age, gender, state, ZIP, and device targeting and can fire for visitors they should exclude. Once resolved, these offers will honor the same targeting rules as regular offers. (#333)
- **[Feature]** **Preview your unsaved changes on placements and offers** — Today the Preview button only shows the last saved version, so you have to save before you can check an edit. This lets Preview reflect your current, unsaved changes so you can review before committing. (#292)
- **[Feature]** **Predict how a new offer will perform** — An exploratory feature to automatically estimate a new offer's likely performance from your historical offer data, replacing today's manual gut-check review and giving a faster, data-grounded projection at intake. (#322)

## General / Across the App

- **[Feature]** **Protect records from being overwritten by two editors at once** — When someone is editing a record, others will see it's locked (with who has it and since when) and be prevented from accidentally saving over each other's changes. A safeguard also warns you if a record changed while you had it open. (#267)
- **[Feature]** **Remove controls that don't actually do anything** — Cleaning up admin options that look functional but have no effect (such as the Advertiser Web Presence fields, certain user-permission toggles, and some Data-Client and Pre-Ping settings) so screens only show controls that truly work. (#296)
- **[Task]** **Users management gap review** — A behind-the-scenes comparison of the older Users screens against New Adsmith Frontend to identify missing capabilities (like bulk role changes, 2FA status, and last-login info) and prioritize what to add. (#80)
- **[Task]** **Decide the future of the legacy File Share page** — Confirming whether the old file-sharing page is still needed and either giving it a home in the new admin or formally retiring it. (#328)

## Surveys

- **[Feature]** **Make survey design customizations actually apply** — Ensuring every option on the survey Design tab shows up in the live survey, plus a full check across all entity forms so no setting is a dead end. Your styling and display choices will reliably appear for visitors. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Settings like survey height and display format, plus a few others, aren't yet reflected in the live survey widget. This wires them through (or removes any that aren't needed) so what you set is what visitors get. (#293)

## Data Clients

- **[Feature]** **Restore after-success delivery behaviors** — Post-conversion delivery and redirect steps from the older system weren't carried over. This brings them back as a configurable option so conversions continue to hand off correctly for the clients that rely on it. (#327)
- **[Feature]** **Bring back custom pre-serve validation for data clients** — A high-priority gap: custom validation checks that used to run when serving many data clients aren't running on the new platform. This restores those checks so the affected clients are validated as expected. (#338)

## Dashboard & Reports

- **[Task]** **Investigate dashboard numbers that don't match the old system** — Reviewers noticed dashboard report figures differing from the legacy app. This traces down where the difference comes from and confirms the numbers can be trusted. (#271)
- **[Bug]** **Invalid links should show a clear error** — Testing an invalid link currently dumps you back on the Dashboard instead of telling you it failed. Once fixed, you'll get a clear error message right in the Link Testing screen. (#239)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The Modal Design tab's header, title, and progress-bar settings currently have no effect on the visitor-facing modal. This either wires them up so they display, or removes the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unpolished, with plain textareas, unstyled color pickers and checkboxes, and paired fields stacking instead of sitting side by side. This tidies the form so it matches the look of other screens. (#152)

## Behind the Scenes

- **[Task]** **Set up a read-only test environment** — Standing up a staging copy of New Adsmith Frontend against production-like data for safe verification, where no changes can accidentally be written. Not user-facing. (#270)
- **[Feature]** **Automatically turn Slack conversations into tracked tasks** — An internal tool that reads designated Slack channels and files the action items as tracked issues, reducing manual note-shuffling. Not user-facing. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d541cdec2d7ef7e80b16585fe689f12231c8b31406080f26d5421cd3a156890a -->
