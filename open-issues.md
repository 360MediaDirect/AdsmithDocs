# Open Issues — Plain-Language Overview

_Last updated 2026-07-19 00:25:14 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach live ads** — A number of options you set on an offer (such as the Modal-tab settings, Display URL, and "force more info" choices) are being dropped before the live ad is shown, so they have no effect today. This fix makes sure the settings you configure actually take hold on the visitor-facing ad. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — This is a high-priority fix. Conversion pixels set up under "Pixels to Fire on Success" are currently not firing at all, with no visible error, which means lost tracking and attribution. After this fix, configured success pixels will fire reliably. (#297)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your own historical offer data, replacing today's informal manual gut-check. It would give a data-driven read at intake — a decision aid, not a guarantee. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — This is a high-priority fix. Auto-register offers currently ignore age, gender, state, zip, and device targeting and can fire for visitors who should be excluded. This work makes them honor the same targeting rules as regular offers (or clearly document any intended difference). (#333)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — The Conflicting Referrals field on an offer's Delivery tab is saved but has no effect when ads are served. This work confirms what the field should do and either makes it work as intended or removes it, so nothing on the screen is misleading. (#351)

## Placements

- **[Feature]** **Preview will reflect your unsaved edits** — On placement and offer edit pages, the Preview button currently shows the last-saved version, so you have to save before you can see a change. This upgrade lets Preview show your current in-progress edits without forcing a save first. (#292)
- **[Feature]** **Placement Design-tab settings will actually apply** — Several Placement Design-tab options (like iFrame Height and Display Format) are saved but don't yet change what visitors see. This finishes connecting each option so your design choices take effect, and removes any option that's meant to be retired. (#293)

## Data Clients

- **[Feature]** **Post-conversion delivery behaviors restored** — Certain after-success actions from the previous system hadn't been carried over. This work brings those behaviors to New Adsmith Frontend so post-conversion delivery keeps working for the affected clients. (#327)
- **[Feature]** **Restore custom pre-serve checks for data clients** — This is a high-priority feature. Many data clients relied on custom validation from the old system that doesn't run on the new platform. This work brings those checks back and runs them at the right moment, so those clients behave as expected before an ad is served. (#338)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only testing environment** — A staging setup that mirrors real data for verification and review, locked so no changes can be made to it. This lets the team validate the product against realistic data without any risk to live information. (#270)
- **[Feature]** **Turn team conversations into tracked work items automatically** — An internal helper that reads designated chat conversations and files the resulting to-dos as tracked issues, replacing manual copy-and-paste. This keeps requests from slipping through the cracks. (#272)

## Surveys

- **[Feature]** **Make sure every design option truly takes effect** — A thorough review across all entity screens to confirm that each customization option on the design settings is actually reflected in the survey visitors see, with no "dead" options that appear to do something but don't. Anything not wired up will be fixed or removed. (#288)

## Modals

- **[Feature]** **Connect or remove the Modal Design tab** — Every field on the Modal Design tab currently has no effect on the modal visitors see. This work either makes those header and progress-bar settings actually display, or removes them so the screen only shows options that do something. (#294)

## Properties

- **[Bug]** **Domain allowlist will finally be enforced** — The allowed-domains list on a Property is saved and editable but currently doesn't block anyone — ads serve on any site regardless of the list. This fix makes ads serve only on the domains you've approved, while Properties with no list set stay unaffected. (#350)

## Flows

- **[Task]** **Tidy up the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other forms, with plain-looking text boxes, color pickers, and fields that stack instead of sitting side by side. This is a careful cleanup pass to make the Flow form look consistent with the rest of the app. (#152)

## Reports

- **[Task]** **Confirm dashboard report numbers match the previous system** — During review, some dashboard figures didn't line up with the old system, making it hard to trust the comparison. This investigation pins down where any difference comes from and confirms the numbers are consistent. (#271)

## Admin / Users

- **[Task]** **Review the Users area against the previous system** — A detailed comparison of the Users screens between the old and new products to spot any missing pieces (like bulk role changes, last-login and two-factor details, and password options) and prioritize what to bring over. This helps close gaps so the Users area feels complete. (#80)

## General / Across the App

- **[Feature]** **Remove admin controls that don't do anything** — Several settings across the app (such as an Advertiser's Web Presence fields, certain user-permission toggles, and a few data-client and pre-ping options) are saved but currently have no effect. A control that looks meaningful but does nothing erodes trust, so these will be hidden or removed — or properly implemented where the behavior is actually needed. (#296)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
