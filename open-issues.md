# Open Issues — Plain-Language Overview

_Last updated 2026-07-20 09:02:09 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **High priority: conversion pixels aren't firing on successful leads** — Success tracking pixels set up on offers are silently failing to fire, meaning completed conversions may not be recorded. This fix restores accurate attribution so you don't lose credit for the results you're driving. (#297)
- **[Task]** **Auto-register offers ignore visitor targeting rules** — Auto-register offers are currently served to everyone, even when age, gender, state, ZIP, or device targeting should exclude a visitor. This work ensures those offers respect the same targeting rules as your other offers. (#333)
- **[Bug]** **Saved offer options aren't reaching the live experience** — Several offer settings you fill in (including Modal-tab fields, Display URL, and some delivery flags) are saved but never actually applied when the offer runs. Each will be properly connected or removed so the form only shows options that truly do something. (#295)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This field on the offer Delivery tab is saved but has no effect on what gets served. It's being reviewed so the field either works as intended or is removed to avoid confusion. (#351)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — Today the Preview button shows the last-saved version of a placement or offer. Soon it will reflect the edits you're making right now, so you can check your changes before saving. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, giving you a fast, data-driven gut-check at intake. (#322)

## Surveys

- **[Feature]** **Make sure survey design choices actually show up** — A full review to confirm that every customization option across the app's forms is connected end-to-end, so the settings you pick in the Design tab reliably appear in the live survey. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live widget** — Some Placement design options (like survey height and display format) are saved but not yet shown to visitors. This work wires them through, or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **High priority: bring back custom pre-serve validation checks** — Certain client-specific validation steps that ran in the old system haven't carried over yet. This restores them so those clients get the same checks before an ad is served. (#338)
- **[Feature]** **Restore post-conversion delivery steps for clients** — After-success actions (like delivery and redirect steps that run once a lead converts) from the previous system are being added to New Adsmith Frontend so those client behaviors work again. (#327)

## General / Across the App

- **[Task]** **Bringing the Users area up to full feature parity** — A detailed comparison of the old and new Users screens to close gaps, such as bulk actions, role changes, and login/security columns, so managing users feels complete. (#80)
- **[Feature]** **Clean up admin controls that don't do anything** — Some settings across Advertisers, user permissions, and data clients are shown but have no effect. These will be hidden or removed so you can trust that every control on screen actually works. (#296)

## Behind the Scenes

- **[Task]** **A safe, read-only testing environment** — Setting up a practice copy of New Adsmith Frontend loaded with realistic data for review and verification, with changes disabled so nothing can be accidentally altered. (#270)
- **[Feature]** **Automatically turn team discussions into tracked work items** — A helper that reads team chat conversations and files the resulting to-dos automatically, reducing manual note-taking and follow-up. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab do what it promises** — The Modal Design tab's settings (header text, colors, progress bar) are saved but don't currently appear to visitors. They'll either be shown in the live modal or removed from the form. (#294)

## Reports & Dashboard

- **[Task]** **Confirming Dashboard report numbers match the previous system** — An investigation into why some Dashboard figures differed from the old platform, so you can trust that reporting is accurate and consistent. (#271)

## Properties

- **[Bug]** **Enforce the domain allowlist on Properties** — A property's list of approved domains is saved but not currently enforced, so ads can serve from any site. This fix ensures ads only serve on the domains you've approved. (#350)

## Flows

- **[Task]** **Fix visual styling issues on the Flow form** — Parts of the Flow form appear unstyled or misaligned compared to other forms. This cleanup restores proper layout, color pickers, and side-by-side fields for a consistent look. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
