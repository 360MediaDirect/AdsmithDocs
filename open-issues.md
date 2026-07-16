# Open Issues — Plain-Language Overview

_Last updated 2026-07-16 17:29:53 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success conversion pixels aren't firing** — This is a high-priority fix. Conversion tracking pixels set up on an offer's success step currently never fire, meaning completed conversions go unrecorded. Once fixed, the tracking you configure will actually run and your attribution data will be accurate. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several fields you fill in on an offer (including the Modal-tab fields, Force More Info Visible, Display URL, and certain data-client options) are saved but quietly dropped before they reach visitors. The fix ensures each option either takes effect as expected or is removed so nothing is misleading. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — High priority. Auto-register offers currently skip age, gender, state, zip, and device targeting, so they can fire for people they should exclude. This work makes their targeting behave consistently with regular offers (or confirms and documents the intended exception). (#333)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — You'll be able to click Preview and see your in-progress edits immediately, instead of having to save first to see how a change looks. (#292)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory feature to estimate how a new offer is likely to perform, based on your historical offer data, giving you a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Data Clients & Pre-Pings

- **[Feature]** **Restore per-client pre-ping checks from the old system** — High priority. Hundreds of data clients relied on custom serve-time validation that isn't running on New Adsmith Frontend yet. This work brings those checks back so the right leads are accepted or rejected as before. (#338)
- **[Feature]** **Restore after-success delivery behavior for data clients** — Post-conversion delivery and redirect steps from the legacy system are being carried over as a reusable, configurable option, so affected data clients behave as they did before. (#327)

## Surveys

- **[Feature]** **Design-tab settings will fully carry through to the live survey** — A thorough check across all screens to make sure every design and form option you set actually shows up in the survey, with any options that do nothing fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live survey** — Placement design options like iFrame Height, Display Format, and a few others will either take effect in the widget or be removed from the form, so what you set is what visitors see. (#293)

## Admin & User Management

- **[Feature]** **Clean up admin controls that don't do anything** — Several settings that are saved but have no effect (Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) will be removed or hidden, so you're not misled into thinking they change behavior. (#296)
- **[Task]** **Review of the Users area against the previous system** — A documentation exercise comparing the old Users management screen with the new one to identify missing features (like bulk actions and last-login info) and prioritize what to add. (#80)

## Reports & Dashboard

- **[Task]** **Investigate why Dashboard report numbers differ from the old system** — Reviewers noticed report figures didn't match the legacy app. This work compares the two over a fixed date range, finds where the difference comes from, and confirms the numbers can be trusted. (#271)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Some parts of the Flow form look unstyled or out of place, with fields stacking oddly instead of sitting side by side. This tidies up the layout to match other forms. Partly done, with the rest handled carefully to avoid disrupting other tabs. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — The six settings on the Modal Design tab currently have no effect on what visitors see. They'll either be wired up to actually control the modal's header and progress bar, or removed if the modal is meant to be header-less. (#294)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only testing environment** — A separate copy of the app running against realistic data, locked to read-only, so the team can verify behavior without any risk to live information. (#270)
- **[Feature]** **Automatically turn team conversations into tracked work items** — A helper that reads designated chat channels and files action items as tracked issues, reducing manual copy-paste when capturing follow-ups. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->
