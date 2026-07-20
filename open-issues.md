# Open Issues — Plain-Language Overview

_Last updated 2026-07-20 21:25:05 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Configured success pixels aren't firing** — When you set up conversion pixels to fire on a successful lead, they're currently being ignored, meaning some conversions go untracked. This fix makes those pixels fire reliably so your attribution and revenue tracking stay accurate. High priority. (#297)
- **[Bug]** **Some saved offer options never reach the live ad** — Several offer settings (including Modal-tab fields, "Force More Info Visible," Display URL, and various data-client flags) are saved but dropped before they take effect. This work makes each one either work as expected or be cleanly removed so nothing misleads you. (#295)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This field on the offer Delivery tab can be filled in but has no effect on which offers are shown. This work confirms the intended behavior and either makes it work or removes it so it isn't misleading. (#351)
- **[Task]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for every visitor, even when age, gender, state, ZIP, or device targeting says they shouldn't. This work makes them respect the same targeting rules as normal offers (or documents it as intended) so leads only fire for the right visitors. High priority. (#333)
- **[Feature]** **Preview unsaved changes on placements and offers** — Today the Preview button only shows the last-saved version, so you have to save before checking your edits. This upgrade lets Preview reflect your current, unsaved changes right away. (#292)
- **[Feature]** **Predict how a new offer will perform** — Instead of relying on a manual gut-check, this explores an automated projection of a new offer's likely performance based on your historical offer data, giving you a helpful estimate at intake time. (#322)

## Surveys

- **[Feature]** **Design settings will match what visitors actually see** — This makes sure every customization option on the design tab is truly reflected in the live survey, and audits all entity forms so no setting is left doing nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live widget** — Some placement design options (like iFrame height, display format, and skip/more-info controls) are saved but not yet applied. This wires the remaining ones through—or removes any that aren't needed—so what you set is what appears. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients rely on custom serve-time validation that hasn't yet been carried over to New Adsmith Frontend. This work ports those checks so the right leads are accepted or rejected as they were before. High priority. (#338)
- **[Feature]** **Bring back after-success delivery steps** — Post-conversion delivery and redirect steps from the older system weren't yet available here. This adds a flexible, configurable version so those clients keep working after a successful conversion. (#327)

## Admin & Users

- **[Feature]** **Remove controls that don't actually do anything** — Several admin settings (Advertiser Web Presence fields, certain user-permission toggles, and a few data-client and pre-ping options) currently look active but have no effect. Cleaning these up prevents confusion and false expectations about access control. (#296)
- **[Task]** **Compare the old and new Users areas** — A review of the older Users management screen against the new one, identifying which features still need to come across (like bulk actions and last-login info) so nothing important is missed. (#80)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of New Adsmith Frontend using production-like data that can't be changed, so the team can verify behavior without risk to live information. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads team discussions and files the resulting to-dos automatically, reducing manual note-taking and making sure requests don't slip through the cracks. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab count** — The entire Modal Design tab (header text, colors, progress bar, and more) is currently saved but never shown to visitors. This work either brings those settings to life in the visitor modal or removes them so the tab isn't misleading. (#294)

## Properties

- **[Bug]** **Domain allowlist will actually block other sites** — A property's list of allowed domains is currently ignored, so ads can be served from any site. This fix enforces the allowlist so ads only appear on the domains you've approved. (#350)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned—plain text boxes, unstyled color pickers, and fields that stack instead of sitting side by side. This work polishes the form so it matches the look of the other screens. (#152)

## Reports

- **[Task]** **Confirm dashboard numbers match the old system** — Reviewers noticed report figures differing from the legacy app. This investigation pins down where the difference comes from and confirms the numbers you see are accurate. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
