# Open Issues — Plain-Language Overview

_Last updated 2026-07-19 18:17:45 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — When an offer is set up to fire a pixel after a successful conversion, those pixels currently never actually fire, so conversions can go unrecorded. This high-priority fix makes configured success pixels fire reliably so you don't lose credit for conversions. (#297)
- **[Task]** **Auto-register offers now respect visitor targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting, so they can show to visitors who should be excluded. This fix brings them in line with regular offers so targeting rules are honored everywhere. (#333)
- **[Bug]** **Saved offer settings that never reached the live ad** — A number of offer options you can fill in (including Modal-tab fields, Display URL, and several data-client settings) were being dropped before the offer went live. Each will be properly connected or removed, so what you save is what visitors actually get. (#295)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This offer Delivery-tab field can be filled in but has no effect on which offers are shown. It will either be made to work as intended (once the business rule is confirmed) or removed so it doesn't imply behavior that isn't there. (#351)
- **[Feature]** **Preview shows your unsaved edits** — On placement and offer edit pages, Preview will reflect the changes you're currently making instead of only the last saved version, so you can check your work without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical offer data, replacing the informal manual gut-check and giving a data-driven read at intake. (#322)

## Surveys

- **[Feature]** **Design-tab options that actually change the survey** — A full audit to make sure every customization option on the Design tab (across all entity screens) truly shows up in the survey visitors see, with any dead options fixed or removed. (#288)
- **[Feature]** **Finishing the Placement survey design settings** — Several Placement Design-tab settings (such as survey height and display format) aren't yet reflected in the live survey widget. This work connects them so your choices take effect, or removes the ones that shouldn't be there. (#293)

## Data Clients / Pre-Pings

- **[Feature]** **Custom pre-ping checks carried over from the old system** — Hundreds of data clients rely on custom serve-time validation rules that haven't been brought into New Adsmith Frontend yet. This high-priority work reconnects those checks so those clients keep validating as they did before. (#338)
- **[Feature]** **Restoring after-success delivery behavior** — Post-conversion delivery and redirect steps from the legacy system are being rebuilt as a reusable option, so clients that depend on them keep working after a successful lead. (#327)

## Admin

- **[Feature]** **Cleaning up controls that don't do anything** — Several admin settings (Advertiser Web Presence fields, certain user permission toggles, and some Data-Client and Pre-Ping options) currently save but have no effect. They'll be hidden or removed so the admin screens only show controls that actually work. (#296)
- **[Task]** **Review of the Users area against the old system** — A detailed comparison of the Users screens in New Adsmith Frontend versus the legacy app, identifying missing capabilities (like bulk role changes and last-login info) to guide what gets built next. (#80)

## Modals

- **[Feature]** **Making the Modal Design tab work — or removing it** — The Modal Design tab's settings (header text, colors, progress bar) currently have no effect on the modal visitors see. This work will either wire them up so they take effect or remove the tab if the modal is meant to be header-less. (#294)

## Properties

- **[Bug]** **Domain allowlist will finally be enforced** — Properties let you list allowed domains, but ads are currently served to any site regardless of that list. This fix makes the allowlist actually block unlisted domains, while properties that leave it empty keep working exactly as before. (#350)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned, with paired fields stacking instead of sitting side by side. This cleanup brings the Flow form's look in line with the Placement and Modal forms. (#152)

## Dashboard / Reports

- **[Task]** **Making sure Dashboard numbers match the old system** — Reviewers noticed Dashboard report figures didn't line up with the legacy app. This investigation pins down where the difference comes from and confirms the reports are accurate. (#271)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a testing copy of the product loaded with realistic data that can't be accidentally changed, so the team can verify behavior against production-like information. (#270)
- **[Feature]** **Turning team conversations into tracked work items** — An internal helper that reads team chat and automatically logs identified tasks, reducing manual copying and keeping the to-do list up to date. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
