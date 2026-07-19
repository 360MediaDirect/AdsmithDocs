# Open Issues — Plain-Language Overview

_Last updated 2026-07-19 03:02:40 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing on completed offers** — This is a high-priority fix. Right now, the tracking pixels you set up to fire when an offer is successfully completed are silently doing nothing, so conversions aren't being recorded. Once fixed, your configured success pixels will fire reliably and your attribution/revenue tracking will be accurate again. (#297)
- **[Task]** **Auto-register offers will respect visitor targeting rules** — Another high-priority fix. Auto-register offers currently ignore your age, gender, state, ZIP, and device targeting, so they can fire for visitors who should have been excluded. This work makes them honor the same targeting rules as your other offers (or clearly document any intended exception). (#333)
- **[Bug]** **Saved offer options that never reached the live experience** — A number of offer settings you fill in on the form (including Modal-tab options, Display URL, and several data-client flags) were being dropped before they reached visitors. Each will be properly wired up so it takes effect, or cleanly removed from the form so you're not configuring things that do nothing. (#295)
- **[Bug]** **"Conflicting Referrals" field currently has no effect** — The Conflicting Referrals box on the offer Delivery tab is saved but doesn't actually influence which offers show. This work confirms the intended business rule and either makes the field work as expected or removes it so it's not misleading. (#351)
- **[Feature]** **Preview edits before saving on Placements and Offers** — Today the Preview button shows the last saved version, so you have to save before you can see a change. This upgrade lets Preview reflect your current, unsaved edits, so you can check your work as you go. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, replacing an informal manual gut-check. If it lands, you'd see a projected performance tier or a comparison to similar past offers right at intake. (#322)

## Surveys

- **[Feature]** **Design-tab options that actually change the survey** — A full audit to make sure every customization option on the Design tab is reflected in what visitors actually see, across all entities. Any setting that doesn't do anything will be fixed or removed, so what you configure is what you get. (#288)
- **[Feature]** **Finishing the Placement survey design settings** — Several Placement Design-tab settings (like iFrame height, display format, skip options, and more-info visibility) aren't yet fully connected to the live survey widget. This finishes wiring them up, or removes the ones that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restoring custom serve-time checks for data clients** — Legacy per-client pre-ping validations (used by hundreds of active data clients) aren't running on New Adsmith Frontend yet. This high-priority work brings that custom validation back so those clients' pass/reject rules apply as they should. (#338)
- **[Feature]** **Bringing back after-success delivery behavior** — Legacy post-conversion delivery and redirect steps for certain clients weren't carried over. This work ports them as a reusable, configurable option so those clients' after-success actions work again. (#327)

## Admin & Users

- **[Feature]** **Cleaning up admin controls that don't do anything** — Several settings (Advertiser Web Presence fields, some user permission toggles, and a few data-client and pre-ping options) are saved but read by nothing, which is confusing and misleading. Each will be removed/hidden or properly implemented, so every control you see actually does something. (#296)
- **[Task]** **Comparing the old and new Users areas** — A documentation review lining up the legacy Users module against the new one to spot missing pieces (like bulk actions, 2FA status, and last-login details). The result is a prioritized list guiding which Users features get built next. (#80)

## Flows

- **[Task]** **Fixing the appearance of the Flow form** — Parts of the Flow form currently look unstyled or misaligned, with plain text boxes, unstyled color pickers, and paired fields stacking vertically instead of sitting side by side. This tidies up the form so it matches the polished look of the Placement and Modal forms. (#152)

## Modals

- **[Feature]** **Making the Modal Design tab do something** — Every field on the Modal Design tab (header title, subtitle, colors, progress bar, and more) is currently saved but never shown to visitors. This work either connects those fields so they change the visitor modal, or removes the tab if the modal is meant to be header-free. (#294)

## Properties

- **[Bug]** **Enforcing the domain allowlist for publishers** — The allowed-domains list on a Property is saved but never actually restricts anything, so ads serve on any website regardless of the list. This fix makes the allowlist work: requests from hostnames you haven't approved will be blocked, while properties without a list stay unaffected. (#350)

## Dashboard & Reports

- **[Task]** **Confirming dashboard numbers match the legacy system** — During testing, some dashboard report figures didn't line up with the old system, making them hard to trust. This investigation pins down where the difference comes from and either corrects it or confirms the numbers are right. (#271)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a copy of the product loaded with production-like data for verification and testing, locked to read-only so nothing can be accidentally changed. No visible change to your day-to-day use. (#270)
- **[Feature]** **Turning conversations into tracked work items automatically** — A helper that reads designated team chat channels, spots action items, and files them as tracked issues (avoiding manual copy-paste). This is an internal workflow tool with no direct impact on the product screens you use. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
