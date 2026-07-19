# Open Issues — Plain-Language Overview

_Last updated 2026-07-19 16:19:11 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels you set up on an offer currently never fire, which means completed leads aren't being tracked and attribution is silently lost. This high-priority fix makes configured success pixels fire reliably. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers are firing for people they should exclude (by age, gender, state, ZIP, or device), unlike regular offers which respect those rules. This high-priority fix will bring auto-register offers in line so they only fire for the right visitors. (#333)
- **[Bug]** **Some saved offer settings never reach live ads** — Several options you fill in on the offer form (including Modal-tab fields, Display URL, and a few data-client flags) are being dropped before they reach visitors. This fix ensures each saved option either takes effect or is cleaned up if it isn't meant to be used. (#295)
- **[Bug]** **"Conflicting Referrals" field has no effect** — This field on the offer Delivery tab is saved but never actually excludes any offers. The work confirms what it's meant to do and either makes it work or removes it, so you're not relying on a setting that does nothing. (#351)
- **[Feature]** **Preview shows your unsaved changes** — On placement and offer edit pages, the Preview button will reflect the edits you've made but not yet saved, so you can check a change before committing it instead of having to save first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, giving Kurt a data-driven read at intake instead of relying on a manual review. (#322)

## Data Clients & Pre-Pings
- **[Feature]** **Restore custom pre-check rules for data clients** — Many data clients used custom serve-time validation in the old system that isn't running on the new platform yet. This high-priority work brings those checks back so the right leads are validated before delivery. (#338)
- **[Feature]** **Bring back after-success delivery behaviors** — The post-conversion delivery and redirect steps used by certain clients weren't carried over from the old system. This adds them back as a reusable setting so those clients behave as expected after a successful conversion. (#327)

## Surveys
- **[Feature]** **Design tab customizations that actually take effect** — A thorough check across all entity forms to make sure every design and display option you set is reflected in the live survey, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live widget** — Placement design options such as iFrame height and display format will actually apply to what visitors see, and any leftover unused options will be wired up or removed. (#293)

## Behind the Scenes
- **[Task]** **A safe, view-only test environment** — Setting up a staging copy of the product using production-like data for verification, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Automatic issue capture from team chat** — A helper that reads conversations and turns action items into tracked tasks automatically, reducing manual note-taking and follow-up. (#272)

## Admin / Users
- **[Task]** **Comparison of the Users screen against the old system** — A review that catalogs which capabilities from the legacy Users area (like bulk role changes, last-login, and two-factor status) are still missing in New Adsmith Frontend, to guide what gets built next. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings currently look active but have no effect (parts of the Advertiser Web Presence tab, a couple of user permission toggles, and a few data-client and pre-ping options). Hiding or removing them keeps the admin area trustworthy and avoids confusion. (#296)

## Reports & Dashboard
- **[Task]** **Investigate dashboard numbers that don't match the old system** — Looking into why some Dashboard report figures differ from the legacy app so we can pinpoint the cause and confirm the numbers you see are accurate. (#271)

## Modals
- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design settings (header text, colors, progress bar) currently have no effect on what visitors see. This work either makes those settings apply or removes the tab so it isn't misleading. (#294)

## Properties
- **[Bug]** **Enforce the allowed-domains list on Properties** — A property's list of allowed domains is currently ignored, so ads can serve on any site. This fix makes the allowlist actually block hostnames that aren't on it, while leaving properties without a list unaffected. (#350)

## Flows
- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form appear unstyled or misaligned, with some paired fields stacking awkwardly. This cleanup brings the Flow form's look in line with the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
