# Open Issues — Plain-Language Overview

_Last updated 2026-07-19 08:46:43 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on placements and offers** — When editing a placement or offer, the Preview button will show your current edits right away, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Some saved offer settings never reach the live ad** — Several options you set on an offer (including its Modal-tab settings, Display URL, and a few delivery flags) are saved but currently don't take effect on the live surface. This fix ensures the settings you enter are actually applied — or removes the ones that were never meant to do anything. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — This is a high-priority fix. Conversion pixels set up on an offer to fire on success are silently not firing, which means lost tracking of results. After the fix, a configured success pixel will fire as expected. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Another high-priority fix. Offers that register automatically are currently shown to every visitor, even ones outside the age, gender, state, ZIP, or device targeting you set. This work makes those offers respect your targeting rules so they only fire for the right audience. (#333)
- **[Bug]** **"Conflicting Referrals" field doesn't do anything yet** — The Conflicting Referrals box on an offer's Delivery tab is saved but has no effect on what gets served. This is being reviewed to confirm the intended behavior and then wire it up (or remove it) so the field does what it appears to do. (#351)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, replacing today's manual gut-check review. It would give a data-driven forecast at intake time. (#322)

## Surveys

- **[Feature]** **Design-tab customizations reflected in the live survey** — An end-to-end check so that every option on the Design tab actually shows up in the survey visitors see, across all entity screens, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting placement Design settings to the live widget** — Several placement Design-tab options (like iFrame height, display format, and a few display toggles) are saved but not yet reflected in the widget. This work wires them through so they take effect — or removes any that aren't needed. (#293)

## Admin

- **[Task]** **Users screen review against the previous system** — A documentation review comparing the old Users management with the new one to spot missing features (like bulk role changes, last-login and two-factor details) and plan what to add. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Some settings (such as the Advertiser Web Presence fields, certain user-permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no real effect. These will be hidden or removed so the admin area only shows controls that actually work. (#296)

## Data Clients

- **[Feature]** **Restore after-conversion delivery behavior for clients** — Post-conversion delivery and redirect steps from the previous system weren't carried over. This work brings those behaviors back for the clients that rely on them. (#327)
- **[Feature]** **Restore custom pre-check rules for data clients** — A high-priority parity item. Custom serve-time validation rules that hundreds of data clients depend on weren't carried over from the old system and currently don't run. This restores them so those checks work again on the new platform. (#338)

## Behind the Scenes

- **[Task]** **Read-only test environment for verification** — Setting up a safe, look-but-don't-touch environment loaded with production-like data so the team can verify the product against real-world numbers. (#270)
- **[Feature]** **Assistant to turn conversations into tracked work items** — An internal helper that reads team conversations and automatically logs the resulting to-dos, cutting out manual copy-paste. This is an internal workflow tool and has no direct effect on the product screens. (#272)

## Reports

- **[Task]** **Confirm report numbers match the previous system** — An investigation into why some Dashboard report figures didn't line up with the old platform, so the team can pinpoint the cause and confirm the numbers are trustworthy. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — The Modal Design tab's settings (header title, subtitle, colors, progress bar) are saved but don't currently show up in the modal visitors see. This work either wires them through so they take effect or removes the tab if it isn't needed. (#294)

## Properties

- **[Bug]** **Domain allowlist isn't being enforced** — The list of allowed domains on a Property is saved but currently doesn't block anyone — ads serve on any site. This fix makes the allowlist actually restrict serving to the domains you've approved, while properties without a list are unaffected. (#350)

## Flows

- **[Task]** **Fix unstyled areas of the Flow form** — Parts of the Flow form look broken or unstyled, with plain textareas, unstyled color pickers, and paired fields stacking instead of sitting side by side. This work brings the Flow form's appearance in line with the other forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
