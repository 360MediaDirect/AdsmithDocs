# Open Issues — Plain-Language Overview

_Last updated 2026-07-17 21:16:31 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers & Placements

- **[Bug]** **Success tracking pixels weren't firing** — This is a high-priority fix. Conversion pixels set up on offers were silently failing to fire, meaning completed conversions went unrecorded. Once fixed, configured success pixels will fire reliably so you don't lose attribution or revenue signal. (#297)
- **[Bug]** **Auto-register offers ignored visitor targeting** — Another high-priority fix. Auto-register offers were being served to visitors who should have been excluded by age, gender, state, zip, or device rules. This ensures those offers respect the same targeting as every other offer. (#333)
- **[Bug]** **Some offer settings never reached the live ad** — A number of saved offer options (including several Modal-tab fields and Display URL) weren't actually making it to the visitor-facing widget. Each will be made to work or cleaned up so what you configure is what visitors see. (#295)
- **[Bug]** **The "Conflicting Referrals" field currently does nothing** — This offer setting saves but has no effect when ads are served. It's being reviewed so it either works as intended or is removed to avoid confusion. (#351)
- **[Feature]** **Preview will show your unsaved changes** — On placement and offer edit pages, the Preview button will reflect the edits you're currently making instead of only the last saved version — so you can check changes before saving. (#292)
- **[Feature]** **Placement design settings will actually take effect** — Several placement Design-tab options (like iframe height and display format) weren't being applied in the live survey. This finishes wiring them up so your design choices show as expected. (#293)
- **[Feature]** **Automatic performance projection for new offers** — A new, data-driven way to estimate how a new offer is likely to perform based on your historical offer data, replacing today's manual review step. (#322)

## Admin / Users

- **[Task]** **Review of the Users area against the old system** — A thorough comparison to make sure the new Users management screens don't miss features people relied on before (like bulk role changes, last-login info, and 2FA status). (#80)
- **[Feature]** **Removing admin controls that don't do anything** — Some settings (such as the Advertiser Web Presence tab, certain user-permission toggles, and a few data-client options) currently save but have no real effect. They'll be removed or hidden so the admin screens only show controls that actually work. (#296)

## Data Clients & Pre-Pings

- **[Feature]** **Custom pre-conversion checks brought over from the old system** — This is a high-priority gap. Many data clients relied on custom serve-time validation checks that don't yet run on New Adsmith Frontend. Porting them ensures those clients' rules are applied again. (#338)
- **[Feature]** **Post-conversion delivery steps restored** — Legacy "after success" behaviors (delivery and redirect steps that run once a conversion completes) are being carried over so affected data clients keep working as before. (#327)

## Surveys

- **[Feature]** **Making every survey design option work** — A full check to confirm each customization on the Design tab is actually reflected in the live survey, with any settings that do nothing either fixed or removed. (#288)

## Modals

- **[Feature]** **Modal Design tab settings wired up or removed** — The Modal Design tab's options (header title, colors, progress bar, and more) currently save but don't appear to visitors. They'll either be made functional or removed so the tab reflects reality. (#294)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Some parts of the Flow form look unstyled or don't line up correctly. This cleans up the layout so it matches the polished look of the other forms. (#152)

## Properties

- **[Bug]** **Approved-domains list will actually be enforced** — A property's allowed-domains list wasn't blocking anything, so ads could serve on any website. This fix ensures ads only appear on the domains you've approved, while properties without a list are unaffected. (#350)

## Dashboard / Reports

- **[Task]** **Investigating report figures that didn't match the old system** — Some dashboard report numbers differed from the legacy app during testing. This work compares the two over a fixed date range to find the cause and confirm the figures are accurate. (#271)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging version of the product using realistic data for verification, with safeguards so nothing can be changed by accident. (#270)
- **[Feature]** **Turning conversation notes into tracked work automatically** — An internal helper that reads discussion notes and files them as tracked tasks, reducing manual copy-and-paste. This is a behind-the-scenes convenience for the team. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
