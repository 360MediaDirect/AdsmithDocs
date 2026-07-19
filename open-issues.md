# Open Issues — Plain-Language Overview

_Last updated 2026-07-19 14:28:16 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes** — When editing a placement or offer, the Preview button will show exactly what you've typed so far, instead of only the last saved version — so you can check a change before committing to it. (#292)
- **[Bug]** **Saved offer options that never reached the live ad** — Several offer settings were being saved in the form but quietly dropped before they could appear on live ad units. This fix makes sure the options you configure actually take effect (or removes ones that were never meant to do anything). (#295)
- **[Bug]** **Success tracking pixels weren't firing** — A high-priority fix: conversion pixels set up on an offer's success step were silently never firing, meaning conversions weren't being tracked. Once fixed, the pixels you configure will reliably fire and record results. (#297)
- **[Feature]** **Automatic performance estimate for new offers** — An exploratory feature to predict how a new offer is likely to perform, based on your own past offers and their results — replacing the informal manual gut-check with a data-driven projection. (#322)
- **[Bug]** **Auto-register offers were ignoring audience targeting** — A high-priority fix: auto-register offers were firing for every visitor even when age, gender, state, ZIP, or device targeting should have excluded them. This ensures those offers respect the same targeting rules as regular offers. (#333)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This offer field is saved but has no effect on what visitors see. The team is confirming what it's meant to do so it can either be made to work or removed, avoiding confusion. (#351)

## Surveys

- **[Feature]** **Design settings fully connected to the live survey** — Every option on the Design tab will actually change what visitors see, and all entity forms will be checked so no setting is left disconnected. You'll be able to trust that the choices you make show up. (#288)
- **[Feature]** **Finish connecting Placement design settings** — A handful of Placement Design-tab settings (like display format and height) weren't reaching the live survey. This work wires them through so they take effect, or tidies up any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Bring back post-conversion delivery steps** — Certain "after success" delivery behaviors from the old system hadn't been carried over. This restores them as a reusable, configurable option so those clients keep working as before. (#327)
- **[Feature]** **Restore file-based pre-ping checks** — A high-priority effort to bring hundreds of clients' custom pre-ping validation rules onto New Adsmith Frontend, so serve-time checks that quietly stopped running are back in place. (#338)

## General / Across the App

- **[Feature]** **Clean up controls that do nothing** — Some admin settings (across Advertisers, user permissions, Data Clients, and Pre-Pings) were saved but had no real effect. Removing or hiding them prevents confusion about settings that appear to work but don't. (#296)
- **[Task]** **Users management review against the old system** — A documentation review comparing the old Users area with the new one to spot missing features (like bulk actions and last-login info) and plan what to add next. (#80)

## Behind the Scenes

- **[Task]** **A safe testing environment with real-like data** — Setting up a read-only copy of the app for testing and verification against production-like data, so changes can be checked without any risk to live information. (#270)
- **[Feature]** **Automatic issue creation from team chats** — A helper that turns action items from team conversations into tracked to-do items automatically, cutting out manual copy-and-paste. (#272)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or stack awkwardly compared with other forms. This is a careful cleanup so text boxes, color pickers, and paired fields display neatly. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab actually work** — The Modal Design tab's options (header text, colors, progress bar) don't currently change the visitor modal. This will either connect them so they take effect or remove them if the modal is meant to stay simple. (#294)

## Reports

- **[Task]** **Investigate Dashboard numbers that don't match the old system** — Some Dashboard report totals differed from the legacy app, making them hard to trust. This work pins down why and confirms the numbers line up. (#271)

## Properties

- **[Bug]** **Make the domain allowlist actually block other sites** — A property's allowed-domains list is saved but isn't currently enforced, so ads serve on any site. This fix ensures ads only serve on the domains you've approved, with no change for properties that leave the list empty. (#350)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
