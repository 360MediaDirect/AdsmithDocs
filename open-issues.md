# Open Issues — Plain-Language Overview

_Last updated 2026-07-18 04:57:26 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — When an offer is set up to fire a pixel after a successful conversion, those pixels are currently being skipped without any warning, which means conversions can go uncounted. This high-priority fix makes sure configured success pixels actually fire, so attribution and revenue tracking are accurate. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting rules** — Certain always-on offers are being shown to everyone, even when they're meant to be limited by age, gender, state, ZIP, or device. This high-priority fix confirms and corrects the behavior so these offers respect the same audience rules as everything else. (#333)
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of options you can set on an offer (including several Modal-tab settings and display details) are saved but silently dropped before visitors ever see them. This work makes sure each option either takes effect or is removed so nothing is misleading. (#295)
- **[Bug]** **"Conflicting Referrals" field has no effect yet** — This field on the offer Delivery tab is saved but doesn't currently change what visitors are shown. The team is confirming the intended business rule before wiring it up, so it will either work as expected or be cleaned up. (#351)
- **[Feature]** **Preview unsaved changes on placements and offers** — Today the Preview button shows the last saved version, so you have to save before checking your edits. This update lets Preview reflect your current, in-progress changes right away. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your own historical offer data, replacing the current informal manual gut-check. It would give a data-driven read on expected performance at intake. (#322)

## Surveys

- **[Feature]** **Design-tab customizations fully connected to the live survey** — An audit across all entities to make sure every design and form option you set actually shows up in the visitor-facing survey, with any options that don't do anything either fixed or removed. (#288)
- **[Feature]** **Finish connecting placement Design settings to the survey widget** — Several placement design options (like display height and format) are saved but not yet applied. This work wires them through so they take effect, and cleans up any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore file-based pre-ping checks for data clients** — Custom validation checks that ran in the old system for hundreds of data clients haven't been carried over yet, so that logic isn't running today. This high-priority work brings those checks to New Adsmith Frontend or documents any that are intentionally retired. (#338)
- **[Feature]** **Bring back after-success delivery behaviors** — Post-conversion delivery and redirect steps from the legacy system are being ported over as a reusable setting, so affected data clients keep working the way they did before. This work is nearly complete. (#327)

## General / Across the App

- **[Feature]** **Clean up controls that don't do anything** — Several admin settings (Advertiser Web Presence fields, some user permission toggles, and a few Data-Client and Pre-Ping options) are currently shown but have no effect. They'll be removed or hidden so the interface only offers controls that actually work. (#296)
- **[Task]** **Review of the Users area against the old system** — A detailed comparison of the Users management screens in New Adsmith Frontend versus the legacy app, identifying missing capabilities (like bulk actions and extra columns) to guide future improvements. (#80)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A separate staging copy of the product, loaded with production-like data and locked so nothing can be changed, so the team can verify behavior without any risk to live data. (#270)
- **[Feature]** **Automated issue-logging from team chats** — A helper that turns action items mentioned in Slack conversations into tracked work items automatically, reducing manual copying and keeping requests from slipping through the cracks. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — Every field on the Modal Design tab currently saves but has no effect on what visitors see. This work either wires those header and progress-bar settings into the live modal or removes the tab so it's no longer misleading. (#294)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form currently look unstyled or misaligned, with fields stacking awkwardly instead of sitting side by side. This is a careful visual cleanup to bring the form in line with the Placement and Modal forms. (#152)

## Properties

- **[Bug]** **Enforce the domain allowlist on properties** — Today a property's list of approved domains is saved but never actually checked, so ads can serve on any website. This fix makes the allowlist do its job: only approved domains serve, while properties without a list are unaffected. (#350)

## Dashboard

- **[Task]** **Confirm dashboard report numbers match the legacy system** — During testing, some dashboard figures didn't line up with the old system. This investigation compares the two over a fixed date range to find any differences, explain them, and confirm the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
