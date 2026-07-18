# Open Issues — Plain-Language Overview

_Last updated 2026-07-18 08:33:36 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels you set up to fire when a lead succeeds are silently not running, so successful conversions aren't being counted. This high-priority fix makes configured success pixels fire reliably so you don't lose credit for conversions. (#297)
- **[Task]** **Auto-register offers ignore audience targeting** — Auto-register offers currently fire for every visitor even when you've set age, gender, state, ZIP, or device targeting. Once addressed, these offers will respect your targeting rules (or the difference will be clearly documented) so the right visitors are matched. (#333)
- **[Bug]** **Some saved offer settings never reach the live offer** — A number of offer options you can fill in (including Modal-tab fields, Display URL, and several delivery flags) are saved but don't currently affect what visitors see. This work makes each option either take effect or be removed so the form matches reality. (#295)
- **[Bug]** **"Conflicting Referrals" field has no effect** — The Conflicting Referrals box on the Offer Delivery tab is saved but never actually excludes any offers. This will confirm the intended rule with the business and either make it work or remove it, so nothing on the form is misleading. (#351)
- **[Feature]** **Preview unsaved edits on Placements and Offers** — Today the Preview button shows the last-saved version, so you must save before you can preview a change. This upgrade lets Preview reflect your current, unsaved edits so you can check your work as you go. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Replaces the informal manual gut-check with a data-driven estimate of how a new offer is likely to perform, based on your own historical offers. You'll get a helpful projection at intake to guide decisions. (#322)

## General / Across the App

- **[Feature]** **Remove admin controls that don't do anything** — Several settings (Advertiser Web Presence fields, certain user permission toggles, and some Data-Client and Pre-Ping options) are saved but have no effect. Cleaning these up means the controls you see actually do what they imply, reducing confusion. (#296)
- **[Task]** **Users area: catching the new experience up to the old one** — An in-progress review comparing the new Users screens to the legacy version, identifying missing pieces like bulk actions, last-login and two-factor details, and role-change tools. The result guides which Users features get restored or improved. (#80)

## Data Clients

- **[Feature]** **Restore post-conversion delivery for data clients** — The legacy "after-success" behaviors that run once a conversion completes weren't carried over to New Adsmith Frontend. This work ports them back as a reusable setting so affected data clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Legacy custom validation that ran at serve time for hundreds of data clients isn't currently running on the new platform. This high-priority effort re-establishes those checks so leads are validated and filtered as they were before. (#338)

## Placements

- **[Feature]** **Make Placement Design settings actually apply** — Several Placement Design-tab options (like survey height and display format) are saved but don't yet change what visitors see. This finishes connecting each setting so your design choices take effect, or removes any that aren't needed. (#293)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — All six fields on the Modal Design tab (header title, subtitle, colors, progress bar) are saved but currently have no effect on the visitor's modal. This will either bring those settings to life or remove the tab so it isn't misleading. (#294)

## Surveys

- **[Feature]** **Ensure every design option shows up in the live survey** — A full audit to confirm each customization you set on a design tab actually appears in the survey visitors see, across all entity types. The payoff is that no setting is left disconnected or ignored. (#288)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned, with paired fields stacking vertically instead of sitting side by side. This clean-up brings the Flow form's look in line with the Placement and Modal forms. (#152)

## Properties

- **[Bug]** **Domain allowlist isn't being enforced** — The allowed-domains list on a Property is saved but currently doesn't stop other websites from serving its ads. This fix makes the allowlist actually restrict serving to approved domains, while leaving properties that haven't set one unaffected. (#350)

## Dashboard / Reports

- **[Task]** **Investigate report numbers that don't match the old system** — During testing, some dashboard report figures didn't line up with the legacy app. This investigation pins down where the difference comes from and confirms the numbers you see are accurate. (#271)

## Behind the Scenes

- **[Task]** **Read-only staging environment for safe testing** — Setting up a test copy of the app connected to production-like data that can't be changed, so the team can verify behavior without any risk to live data. (#270)
- **[Feature]** **Automatic issue-logging from team chat** — A helper that turns action items from team conversations into tracked work items automatically, reducing manual note-keeping and helping requests get captured. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
