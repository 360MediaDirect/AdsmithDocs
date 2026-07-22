# Open Issues — Plain-Language Overview

_Last updated 2026-07-22 06:49:31 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview offers and placements with your unsaved edits** — When you click Preview while editing an offer or placement, you'll see your latest changes right away instead of having to save first. This makes it much easier to check how a change looks before committing to it. (#292)
- **[Bug]** **Some saved offer settings weren't reaching the live ad** — A number of offer options (including certain modal settings, Display URL, and several delivery-related flags) were being saved but never actually applied when the offer went live. This fix makes sure the options you set on an offer take effect. (#295)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, replacing the current manual gut-check review. This would give you a quick, data-driven read on a new offer at intake. (#322)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — The Conflicting Referrals box on an offer's Delivery tab is saved but has no effect on which offers get served. This is being reviewed to confirm the intended rule and then make the field actually work (or be removed) so it's not misleading. (#351)

## Surveys

- **[Feature]** **Make sure every survey design option actually works** — A full review across all entity screens to confirm that each customization option you set on a design tab genuinely shows up in the live survey. Any options that don't do anything will be fixed or removed, so what you configure is what visitors see. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Several Placement design options (like survey height and display format) are saved but aren't yet reflected in the survey visitors see. This work wires them up so those settings take effect. (#293)

## Data Clients

- **[Feature]** **Bring over post-conversion delivery behavior from the old system** — Certain after-success actions (such as follow-up redirects and delivery scripts) from the legacy platform hadn't been carried over yet. This restores that behavior so affected data clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients relied on custom serve-time validation in the old system that isn't running on the new platform yet. High priority. This brings those checks back so leads are validated the way they were before. (#338)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — The entire Modal Design tab (header text, colors, progress bar, and more) is currently saved but never shown to visitors. This work will either make those settings appear in the visitor modal or remove the tab so it isn't misleading. (#294)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned compared to other forms, with fields stacking oddly and plain-looking text boxes and color pickers. A careful cleanup will bring the Flow form in line with the polished look of the Placement and Modal forms. (#152)

## Properties

- **[Bug]** **Domain allowlist wasn't actually blocking other sites** — The allowed-domains list on a Property is saved but currently isn't enforced, so ads could serve from any website. High priority. This fix ensures that when you set an allowlist, only the listed sites can serve the ads. (#350)

## Dashboard & Reports

- **[Task]** **Confirm report numbers match the old system** — Reviewers noticed dashboard report figures didn't line up with the legacy app. This investigation compares the two over a fixed date range to find any differences, explain the cause, and confirm the numbers can be trusted. (#271)

## Admin & Users

- **[Task]** **Review of the Users area against the old system** — A detailed comparison of the Users screens in New Adsmith Frontend versus the legacy app, identifying missing capabilities (like bulk role changes and last-login info) so the team can prioritize what to add. (#80)

## General / Across the App

- **[Feature]** **Remove admin controls that don't do anything** — Several settings across the app (such as the Advertiser Web Presence fields, certain user permission toggles, and some data-client and pre-ping options) are saved but have no real effect. These will be hidden or removed so the admin screens only show controls that actually work. (#296)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A separate environment loaded with production-like data for verification and testing, locked down so no changes can be made to it. This lets the team validate the product against realistic data without any risk to live information. (#270)
- **[Feature]** **Turn team conversations into tracked work items automatically** — An internal helper that reads designated chat channels and files follow-up tasks automatically, reducing manual copy-and-paste. No direct effect on the product screens you use. (#272)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
