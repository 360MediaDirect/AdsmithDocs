# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 22:20:17 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview offers and placements with your unsaved changes** — When editing an offer or placement, the Preview will show exactly what you're working on right now, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Some saved offer settings don't reach the live experience** — A number of options you set on an offer (including modal settings and display details) currently get lost before reaching visitors. This fix makes sure every saved setting is actually used or clearly removed if it isn't needed. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — A high-priority fix: conversion pixels set up on offers currently never fire, meaning credit for those conversions goes unrecorded. Once fixed, configured success pixels will fire reliably. (#297)
- **[Task]** **Auto-register offers are ignoring visitor targeting** — A high-priority fix so that automatically-registered offers respect the same age, gender, state, ZIP, and device rules as regular offers, instead of firing for people who should be excluded. (#333)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, giving Kurt a data-driven read at intake instead of relying on a manual gut-check. (#322)

## General / Across the App

- **[Feature]** **Protection against two people overwriting the same record** — When someone opens a record to edit it, others will see it's being edited and be warned before they can accidentally overwrite each other's changes. Works across offers, flows, placements, advertisers, and more. (#267)
- **[Feature]** **Remove controls that don't actually do anything** — Several settings across Advertisers, Users, Data Clients, and Pre-Pings currently save but have no effect. These will be hidden or removed so the screens only show controls that genuinely work. (#296)
- **[Bug]** **Invalid link tests now show a clear error** — When you test a link that isn't valid, you'll get a proper error message instead of being unexpectedly sent to the Dashboard. (#239)
- **[Task]** **Decide the future of the file-share page** — The old file-share page has no equivalent yet. This is a quick review to confirm whether anyone still needs it or it can be retired. (#328)

## Surveys

- **[Feature]** **Design-tab options fully reflected in the survey** — A thorough pass to make sure every customization you set on the Design tab actually shows up in the live survey, with a wider check across all screens to catch any options that currently do nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey widget** — Several placement Design-tab settings (like survey height and display format) aren't yet reflected in the live widget. This wires them up or removes the ones that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back after-success delivery steps** — Post-conversion delivery and redirect behavior from the old system will be carried over so it keeps working for the clients that rely on it. (#327)
- **[Feature]** **Restore custom pre-ping validation checks** — A high-priority effort to carry over the custom serve-time checks used by hundreds of data clients, which currently don't run on the new platform. (#338)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging version of New Adsmith Frontend that runs against production-like data for verification, with writing disabled so nothing can be changed by accident. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads discussion notes and files them as tracked items, cutting out manual copy-and-paste when logging follow-ups. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — Every field on the Modal Design tab currently saves but has no effect on what visitors see. These will either be wired up to display properly or removed to avoid confusion. (#294)

## Reports

- **[Task]** **Investigate why dashboard numbers don't match the old system** — A review to compare report figures between the old and new platforms, find where any differences come from, and confirm the numbers can be trusted. (#271)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned, with paired fields stacking awkwardly instead of sitting side by side. This tidies up the form to match the rest of the app. (#152)

## Campaigns

- **[Feature]** **Add the missing Campaigns area** — A high-priority build to bring campaign management into New Adsmith Frontend, letting you view, create, edit, and configure campaigns and their offer groups just like the old system. (#200)

## Users

- **[Task]** **Compare the Users area to the old version** — A review of what the old Users screens could do versus the new one, so any missing pieces (like bulk actions or extra columns) can be planned and prioritized. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f12be1691f4d05be7a51684fc6fe5ab6d4c4751d5a9de6a600395df673d554b3 -->
