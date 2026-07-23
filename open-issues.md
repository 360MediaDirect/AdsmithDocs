# Open Issues — Plain-Language Overview

_Last updated 2026-07-23 06:48:33 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach the live ad** — Several options you set on an offer (including the Modal tab settings, "Force More Info Visible," Display URL, and certain data-delivery flags) are saved but currently don't take effect when the ad is served. This work makes sure each setting either does what it says or is cleared away so it can't mislead you. (#295)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — Right now the Preview button shows the last saved version, so you have to save before you can see edits. Once done, Preview will reflect the changes you're currently making, so you can check your work before saving. (#292)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This Delivery-tab field on an offer is saved but has no effect on which offers get shown. This item confirms the intended behavior and either makes it work or removes the field so it isn't misleading. (#351)
- **[Feature]** **Automatic performance estimate for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your own past offers and their results, replacing today's informal manual gut-check. It would give you a helpful projection at intake. (#322)

## Surveys

- **[Feature]** **Make every design option actually change the survey** — A full review to confirm that each customization option across all screens truly carries through to what visitors see, with any options that quietly do nothing either fixed or removed. Your design choices will reliably show up in the live survey. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — A handful of Placement Design-tab settings (such as height and display format) don't yet affect the survey visitors see. This connects them so they work as expected, or removes ones that aren't needed. (#293)

## Data Clients

- **[Feature]** **Bring back post-conversion delivery steps for data clients** — Certain after-conversion behaviors from the older system weren't carried over yet. This restores them in a flexible, reusable way so affected data clients behave as they did before. This work is nearly complete. (#327)
- **[Feature]** **Restore custom pre-send checks for data clients** — A high-priority effort to bring over the custom validation that ran before sending leads for hundreds of data clients, which currently isn't running on the new platform. Once done, those checks will apply again at delivery time so leads are validated as expected. (#338)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design tab (header text, colors, progress bar, and more) is currently saved but never shown to visitors. This either wires those settings into the visitor's modal or removes the tab so it isn't misleading. (#294)

## Properties

- **[Bug]** **Enforce the allowed-domains list on Properties** — Today a Property's list of approved website addresses is saved but not actually enforced, so ads can be served on sites that were never approved. This high-priority fix makes the allowlist block unapproved sites as publishers expect. (#350)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or misaligned compared with the Placement and Modal forms (plain text boxes, unstyled color pickers, fields stacking instead of sitting side by side). This is a partly-done cleanup to make the Flow form look consistent and polished. (#152)

## Reports

- **[Task]** **Confirm dashboard report numbers match the previous system** — Reviewers noticed dashboard report figures didn't line up with the older system. This investigation compares the two over a fixed period, pinpoints any differences, and either corrects them or confirms the numbers are trustworthy. (#271)

## Admin / Users

- **[Task]** **Review the Users area against the previous system** — A documentation review comparing the new Users screens with the older version to spot missing capabilities (like bulk actions, last-login and two-factor status, and password setup) so gaps can be prioritized. This helps ensure the Users area is complete. (#80)

## General / Across the App

- **[Feature]** **Remove admin controls that don't do anything** — Several settings across the app are saved but have no effect (for example the Advertiser "Web Presence" fields, some user-permission toggles, and a few data-client and pre-ping options). Controls that imply access or behavior they don't actually deliver will be hidden or removed, or flagged for real implementation, so what you see is what you get. (#296)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of the product using production-like data, locked to view-only so testers can validate against realistic numbers without any risk of changing live data. (#270)
- **[Feature]** **Automatically turn team conversations into tracked work items** — An internal helper that reads designated chat channels, spots action items, and files them as tracked tasks automatically, reducing manual copy-and-paste when planning work. (#272)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
