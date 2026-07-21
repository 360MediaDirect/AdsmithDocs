# Open Issues — Plain-Language Overview

_Last updated 2026-07-21 15:33:16 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved edits** — On placement and offer edit pages, the Preview button will show the changes you're currently making instead of the last saved version, so you can check your work before saving. (#292)
- **[Bug]** **Some offer settings never reach live ads** — Several saved offer options (including Modal-tab settings, Display URL, and certain data-client flags) are currently dropped and never appear where visitors see them. Each option will either be made to work or removed. (#295)
- **[Bug]** **Success tracking pixels not firing** — A high-priority fix. Conversion pixels configured on offers currently never fire, so conversions can go unrecorded with no visible error. This ensures configured success pixels fire reliably. (#297)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, new offers will get a data-driven estimate of likely performance based on your own historical offer data. (#322)
- **[Task]** **Auto-register offers will respect targeting** — A high-priority fix. Auto-register offers currently fire for every visitor regardless of age, gender, state, zip, or device targeting. This makes them honor the same targeting rules as other offers. (#333)
- **[Bug]** **"Conflicting Referrals" field will actually do something** — This field on the offer Delivery tab is saved today but has no effect. Work will make it exclude offers as intended (once the exact rule is confirmed) or clarify its purpose. (#351)

## Data Clients

- **[Feature]** **Restore after-success delivery steps** — Post-conversion delivery and redirect behavior from the old system will be brought over so affected clients keep delivering leads correctly after a successful conversion. (#327)
- **[Feature]** **Restore custom pre-ping checks** — A high-priority item. Custom serve-time validation used by hundreds of data clients in the old system isn't running on the new platform yet. This ports those checks so they apply again. (#338)

## Surveys

- **[Feature]** **Design options that actually take effect** — A thorough audit so every design and customization option across the product genuinely changes what appears in the survey view, with no settings that quietly do nothing. (#288)
- **[Feature]** **Placement Design settings applied to the widget** — Placement design options like display format and iFrame height (plus a few others) will actually change what visitors see, or be removed if they aren't used. (#293)

## General / Across the App

- **[Task]** **Users screen catch-up review** — A documentation and analysis effort comparing the old Users management with the new one, so gaps like bulk actions, extra filters, and additional columns can be closed. (#80)
- **[Feature]** **Clean up controls that do nothing** — Settings that currently save but have no effect (Advertiser Web Presence fields, certain user permission toggles, and some Data-Client and Pre-Ping options) will be removed or hidden to avoid confusion. (#296)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a test environment that mirrors real data so the team can verify behavior against realistic data without any risk of changing it. (#270)
- **[Feature]** **Automatic capture of action items** — A helper that turns team discussion into tracked work items automatically, reducing manual copying and follow-up. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work** — The modal's Design tab (header title and subtext, colors, and progress bar) currently has no effect on what visitors see. These will be wired up to display properly, or removed if the modal is meant to be header-less. (#294)

## Flows

- **[Task]** **Fix Flow form styling** — A styling fix. Parts of the Flow form currently look unstyled or misaligned, and paired fields stack awkwardly. This restores proper styling and side-by-side layouts to match the other forms. (#152)

## Reports

- **[Task]** **Investigate dashboard report mismatches** — Confirm why some dashboard report numbers differ from the legacy system and correct any discrepancies, so the figures can be trusted during review. (#271)

## Properties

- **[Bug]** **Enforce a property's allowed-domains list** — A property's allowed-domains list is currently ignored, meaning ads can serve on any website. This makes the allowlist actually block requests from domains you haven't approved, while leaving properties without a list unaffected. (#350)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
