# Open Issues — Plain-Language Overview

_Last updated 2026-07-20 00:26:34 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing on completed offers** — Conversion tracking pixels set up on offers currently never fire, meaning completed leads aren't being counted. This fix makes those pixels fire reliably so you don't lose credit for conversions. This is a high-priority fix. (#297)
- **[Bug]** **Some offer settings never reach the live ad** — Several options you can set on an offer (including Modal-tab settings, Display URL, Force More Info, and certain data-client options) are saved but quietly ignored when the offer runs. Each will either be made to work or removed so the form only shows settings that actually take effect. (#295)
- **[Task]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for every visitor even when age, gender, state, ZIP, or device targeting says they shouldn't. This work makes those offers respect the same targeting rules as regular offers so they only show to the right people. This is a high-priority fix. (#333)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This field on the offer Delivery tab is saved but has no effect on which offers show. We're confirming what it's meant to do and will either make it work or remove it, so the form doesn't imply a rule that isn't there. (#351)
- **[Feature]** **Preview edits before saving on placements and offers** — Today the Preview button shows the last saved version, so you have to save before you can see a change. This upgrade lets Preview reflect your current unsaved edits. (#292)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool that estimates a new offer's likely performance based on your historical offer data, replacing the old manual gut-check review. It would give a data-backed projection at intake time. (#322)

## Survey

- **[Feature]** **Make sure every design option actually changes the survey** — A full audit across all entities to confirm that each customization option you set really shows up in the live survey, with any dead options fixed or removed. You'll be able to trust that the settings you choose take effect. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Several Placement design-tab settings (like iFrame height and display format) are saved but not applied to the live survey. Each will either be wired up so it works or removed from the form. (#293)

## Data Clients

- **[Feature]** **Restore file-based pre-ping checks for data clients** — Custom serve-time validation that many data clients relied on in the old system isn't running on the new platform yet. This work brings those checks back so client-specific validation applies as expected. This is a high-priority parity gap affecting hundreds of clients. (#338)
- **[Feature]** **Bring back after-success delivery for data clients** — The old post-conversion delivery and redirect behavior for certain clients wasn't carried over. This restores it as a reusable setting so those clients get the follow-up actions they had before. This one is nearly complete. (#327)

## Admin & Users

- **[Task]** **Close the gaps between the old and new Users area** — A review comparing the legacy Users screen to the new one, so missing capabilities (like bulk actions, selecting multiple users, and extra columns) can be prioritized and added. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Some settings across Advertisers (Web Presence), user permissions, Data-Client, and Pre-Ping are shown but have no effect. Hiding or removing them prevents confusion and false expectations about what they control. (#296)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — Every field on the Modal Design tab is currently saved but never shown to visitors. Each field will either be built into the visitor modal or removed from the form so nothing is misleading. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or misaligned, with fields stacking instead of sitting side by side. This cleans up the layout so it matches the polished look of the Placement and Modal forms. (#152)

## Properties

- **[Bug]** **Enforce the domain allowlist on Properties** — The allowed-domains list is saved but not actually checked, so ads can currently be served from any website. This fix makes the allowlist block hostnames that aren't approved, while properties without a list keep working as before. (#350)

## Dashboard

- **[Task]** **Confirm dashboard report numbers match the old system** — During testing, some dashboard figures didn't line up with the legacy app. This investigation compares the two over a fixed period to find and explain any differences, so you can trust the reported numbers. (#271)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of New Adsmith Frontend, loaded with production-like data, where the team can verify behavior without any risk of changing real records. (#270)
- **[Feature]** **Turn meeting notes into tracked work automatically** — An internal helper that reads team conversations and files the resulting to-dos automatically, reducing manual tracking. No direct effect on the product screens you use. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
