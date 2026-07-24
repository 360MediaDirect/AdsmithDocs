# Open Issues — Plain-Language Overview

_Last updated 2026-07-24 06:48:11 UTC · 15 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes before saving** — On the placement and offer edit pages, the Preview button will show your current in-progress edits instead of the last saved version, so you can check your work without saving first. (#292)
- **[Bug]** **Saved offer options not reaching live pages** — Several offer settings you fill in (including modal-tab options, Display URL, and a few delivery flags) are saved but never actually appear on the live experience. This fix ensures each option either works as expected or is cleared out if it isn't needed. (#295)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — The Conflicting Referrals box on the offer Delivery tab is saved but has no effect on which offers show. This work will make the field actually exclude offers as intended (pending confirmation of the exact rule). (#351)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, new offers could be scored against your historical offer data to estimate likely performance. This is an early, exploratory idea to give a data-driven read at intake time. (#322)

## Survey

- **[Feature]** **Design options fully connected to the live survey** — Every customization on the Design tab will reliably show up in the actual survey, and all entity form options will be reviewed to remove or fix any settings that currently don't do anything. (#288)
- **[Feature]** **Finish connecting Placement design settings** — A handful of Placement Design-tab settings (like survey height and display format) are saved but not yet reflected in the live widget. This work wires them through or removes the ones that aren't used. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — Certain after-conversion redirect and delivery steps from the old system weren't carried over yet. This brings that behavior back for the clients that still rely on it. (#327)
- **[Feature]** **Restore custom pre-delivery validation checks** — A large group of data clients (about 448) relied on custom checks in the old system that don't currently run on New Adsmith Frontend. This high-priority work re-enables those checks so leads are validated as before. (#338)

## Admin & Users

- **[Task]** **Review of Users features vs. the old system** — A detailed comparison of the old Users area against the new one, identifying missing capabilities (like bulk role changes, last-login and two-factor status, and password/notification options on new-user setup) so the new Users area can catch up. (#80)
- **[Feature]** **Remove controls that don't do anything** — Several admin settings (Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) are saved but currently have no effect. Hiding or removing them prevents confusion about access and behavior that doesn't actually exist. (#296)

## Behind the Scenes

- **[Task]** **Safe testing environment against production-like data** — Setting up a view-only staging version of the product wired to a copy of real data, so the team can verify behavior without any risk of changing live records. (#270)
- **[Feature]** **Automatic issue tracking from team conversations** — A helper that reads designated chat channels and turns action items into tracked work items automatically, cutting out manual copy-paste. (#272)

## Reports & Dashboard

- **[Task]** **Confirm Dashboard report numbers match the old system** — Investigating why some Dashboard report figures differed from the legacy system, pinpointing the cause, and confirming the numbers line up so you can trust the reports. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The Modal Design tab's header and progress-bar settings are saved but don't currently show up in the visitor modal. This work either brings them to life or removes them so the tab only shows options that actually apply. (#294)

## Flows

- **[Task]** **Fix visual layout issues on the Flow form** — Some parts of the Flow form appear unstyled or awkwardly stacked compared to other forms. This tidies up the appearance so text areas, color pickers, checkboxes, and paired fields look consistent and polished. (#152)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
