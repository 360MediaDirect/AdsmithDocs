# Open Issues — Plain-Language Overview

_Last updated 2026-07-20 23:21:13 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Conversion tracking pixels aren't firing on successful leads** — A high-priority fix so that the success pixels you set up on an offer actually fire when a conversion happens, restoring accurate attribution and revenue tracking that's silently being missed today. (#297)
- **[Bug]** **Auto-register offers ignore audience targeting** — We're making sure automatically-registered offers respect the same age, gender, state, ZIP, and device rules as regular offers, so they no longer count leads for visitors who should have been excluded. (#333)
- **[Bug]** **Some saved offer settings never reach the live ad** — Several offer options you can fill in today (including Modal-tab fields, Display URL, and certain delivery flags) aren't actually being applied where visitors see them. We'll wire each one through or clearly retire the ones that aren't needed. (#295)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This offer setting is saved but has no effect when ads are served. We're confirming what it's meant to do and then making it work as expected (or removing it so it isn't misleading). (#351)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool that estimates a new offer's likely performance based on your own historical offer data, giving Kurt a fast, data-driven gut-check at intake instead of relying on a manual review. (#322)

## Placements

- **[Feature]** **Preview your unsaved changes on Placements and Offers** — The Preview button will show the edits you're currently making before you save, so you can check how a change looks without having to save first. (#292)
- **[Feature]** **Make all Placement Design-tab settings take effect** — We're finishing the connection between the Placement Design tab and what visitors actually see, so options like iFrame height and display format are applied (and any unused ones are cleaned up). (#293)

## General / Across the App

- **[Task]** **Bring new user management in line with the old system** — A review comparing the old and new user administration screens to spot what's missing, so features like bulk role changes, login/2FA visibility, and other user-list tools can be added to the new experience. (#80)
- **[Feature]** **Remove admin settings that don't do anything** — Several controls (such as the Advertiser Web Presence tab, some user permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no real effect. We'll hide or remove them so the admin area only shows settings that truly work. (#296)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior for data clients** — The after-success delivery and redirect steps from the old system are being carried over, so clients that rely on them keep working on the new platform. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — A high-priority effort to bring over the older custom validation that runs when ads are served for hundreds of data clients, so their pass/reject rules are honored again on the new platform. (#338)

## Surveys

- **[Feature]** **Make every design customization actually appear in surveys** — A full review across all entity screens to confirm each design and form option you can set is truly reflected in the live survey, with any dead options fixed or removed. (#288)

## Modals

- **[Feature]** **Make the Modal Design tab settings work (or remove them)** — Right now the Modal Design tab's header, colors, and progress-bar options are saved but never shown to visitors. We'll either build them into the visitor modal or remove the tab so it isn't misleading. (#294)

## Properties

- **[Bug]** **Enforce the domain allowlist on Properties** — When a property lists approved domains, ads will only be served on those domains as intended, instead of serving everywhere regardless of the list. (#350)

## Reports

- **[Task]** **Confirm Dashboard report numbers match the old system** — We're investigating why some dashboard figures differed from the legacy app during testing, so you can trust the reported numbers are consistent and accurate. (#271)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Cleaning up the Flow form's appearance so text boxes, color pickers, checkboxes, and paired fields look consistent and properly laid out like the other forms. (#152)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of the product loaded with production-like data for verification and testing, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Automatically turn team conversations into tracked work items** — A helper that reads designated chat channels and files the requested changes for the team automatically, reducing manual note-taking and making sure requests aren't lost. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
