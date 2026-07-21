# Open Issues — Plain-Language Overview

_Last updated 2026-07-21 07:47:53 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — A high-priority fix. Right now, conversion tracking pixels set up on an offer's success step silently never fire, so successful conversions aren't being counted. Once fixed, the pixels you configure will actually trigger and your attribution will be accurate. (#297)
- **[Task]** **Auto-register offers ignore audience targeting** — A high-priority fix. Auto-register offers are currently shown to every visitor even when age, gender, state, ZIP, or device targeting should exclude them. This work makes those offers respect the same targeting rules as regular offers (or documents it as intended). (#333)
- **[Bug]** **Some saved offer settings never reach live ads** — Several offer options you can set today (including Modal-tab fields, Display URL, and certain delivery flags) aren't making it through to what visitors actually see. This audit ensures each setting either works end-to-end or is removed so nothing is misleading. (#295)
- **[Bug]** **"Conflicting Referrals" field does nothing yet** — The Conflicting Referrals box on an offer's Delivery tab saves your input but has no effect on which offers get served. This clarifies the intended rule and either makes it work or removes the field. (#351)
- **[Feature]** **Preview unsaved changes on placements and offers** — You'll be able to click Preview and see your in-progress edits right away, instead of having to save first before previewing. (#292)
- **[Feature]** **Automatic performance estimate for new offers** — An exploratory feature to project how a new offer is likely to perform based on your historical offer data, replacing today's manual gut-check review. (#322)

## Surveys

- **[Feature]** **Make sure design options actually change the survey** — A review to confirm that every customization you set on the Design tab is reflected in the live survey, with any settings that currently do nothing getting fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Several Placement Design-tab settings (like survey height and display format) aren't yet applied to the live survey widget. This finishes wiring them so your choices take effect. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back file-based pre-ping checks** — A high-priority parity item. Custom validation checks that hundreds of data clients relied on in the old system aren't running on New Adsmith Frontend yet. This restores that pre-serve validation. (#338)
- **[Feature]** **Restore after-success delivery behaviors** — Post-conversion delivery and redirect steps from the legacy system are being carried over so affected clients keep working as before. Nearly complete. (#327)

## Admin Area

- **[Task]** **Users screen comparison with the old system** — A review comparing the Users area to the legacy version to spot missing capabilities (like bulk actions and last-login info) and plan what to add. Mostly complete. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings across Advertisers, Users, Data Clients, and Pre-Pings currently save but have no real effect. These will be hidden or removed so the admin screens only show controls that truly work. (#296)

## Behind the Scenes

- **[Task]** **Safe testing environment using real-like data** — Setting up a read-only environment mirroring live data so the team can verify the product against realistic information without any risk of changing it. (#270)
- **[Feature]** **Automatically turn conversations into tracked work items** — A helper that reads team conversations and files the resulting to-dos automatically, reducing manual note-keeping. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — The Modal Design tab settings (header text, colors, progress bar) currently don't appear on the visitor's modal. This will either make them show up or remove the tab if a header isn't wanted. (#294)

## Properties

- **[Bug]** **Enforce the domain allowlist** — A property's allowed-domains list is saved but not actually enforced, so ads can currently be served from any website. This will honor the allowlist so ads only serve on approved domains. (#350)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other forms. This tidies up the layout so text boxes, color pickers, and paired fields display properly. (#152)

## Reports

- **[Task]** **Investigate mismatched dashboard report numbers** — Report totals on the dashboard didn't match the old system during testing. This traces where the difference comes from and confirms the numbers are correct. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
