# Open Issues — Plain-Language Overview

_Last updated 2026-07-18 18:17:55 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing on conversions** — Right now, the tracking pixels admins set up under "Pixels to Fire on Success" silently never fire, so conversions aren't being counted. This high-priority fix makes those pixels fire reliably so you keep accurate attribution. (#297)
- **[Task]** **Auto-register offers currently ignore audience targeting** — Auto-register offers are being served to visitors they should skip (wrong age, gender, state, zip, or device). This high-priority fix makes them respect the same targeting rules as regular offers so people only see offers meant for them. (#333)
- **[Bug]** **Some saved offer settings never reach live ads** — A number of offer options (including the Modal-tab settings, Force More Info, Display URL, and several data-client flags) are saved but dropped before the live ad is shown. This work makes those settings actually take effect or removes the ones that shouldn't be there. (#295)
- **[Bug]** **"Conflicting Referrals" field doesn't do anything yet** — The Conflicting Referrals box on the Offer Delivery tab saves your entry but has no effect on which offers are served. This clarifies the intended rule and either makes it work or removes it so the field isn't misleading. (#351)
- **[Feature]** **Preview your unsaved edits on placements and offers** — Today the Preview button only shows the last-saved version, so you have to save before you can check a change. Soon Preview will show your current, in-progress edits so you can review before committing. (#292)
- **[Feature]** **Automatic performance estimates for new offers** — An exploratory tool that projects how a new offer is likely to perform based on your historical offer data, giving Kurt a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Surveys

- **[Feature]** **Design settings that actually show up in the survey** — A full audit to make sure every option on the Design tab (across all entity screens) truly carries through to what visitors see, with any unused options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live widget** — A handful of Placement Design-tab settings (like survey height and display format) are saved but not yet applied. This makes each one take effect in the widget or removes it from the form. (#293)

## Data Clients

- **[Feature]** **Restore file-based pre-ping checks for data clients** — Custom, serve-time validation checks that many data clients relied on in the old system aren't running on New Adsmith Frontend yet. This high-priority work brings them back so those clients' rules are applied again. (#338)
- **[Feature]** **Bring back after-success delivery behaviors** — Post-conversion delivery and redirect steps from the legacy system are being ported over as a reusable, configurable option so data clients keep working the way they did before. (#327)

## Behind the Scenes

- **[Task]** **A safe test environment using real-world data** — Setting up a read-only staging copy so the team can verify New Adsmith Frontend against production-like data without any risk of changing live records. (#270)
- **[Feature]** **Automatic issue-logging from Slack conversations** — An internal helper that turns action items mentioned in Slack into tracked to-dos automatically, so nothing gets lost in note-taking. (#272)

## Dashboard

- **[Task]** **Look into report numbers not matching the old system** — During testing, some Dashboard report figures didn't line up with the legacy app. This investigation pins down why and confirms the numbers are correct and consistent. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The Modal Design tab's settings (header title, colors, progress bar, etc.) are saved but don't currently appear in the visitor modal. This either wires them up so they show, or removes the tab if it's not needed. (#294)

## Flows

- **[Task]** **Fix visual styling on the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other forms — plain textareas, unstyled color pickers, and fields stacking instead of sitting side-by-side. This tidies up the appearance so it matches the rest of the app. (#152)

## Properties

- **[Bug]** **Make the domain allowlist actually block other sites** — A property's "allowed domains" list is saved but not enforced, so ads currently serve on any site regardless of the list. This makes the allowlist work as expected, serving only on approved domains while leaving properties without a list unaffected. (#350)

## Users

- **[Task]** **Compare the Users area against the old system** — A review documenting which Users features from the legacy app are still missing in New Adsmith Frontend (like bulk actions, last-login, and 2FA status) so the gaps can be prioritized and closed. (#80)

## General / Across the App

- **[Feature]** **Remove admin controls that don't do anything** — Several settings across the app (Advertiser Web Presence fields, certain user-permission toggles, and some Data-Client and Pre-Ping options) are saved but have no effect. Hiding or removing them prevents confusion and false expectations about what they control. (#296)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
