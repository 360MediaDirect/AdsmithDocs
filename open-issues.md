# Open Issues — Plain-Language Overview

_Last updated 2026-07-20 15:36:10 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved edits on placements and offers** — When editing a placement or offer, the Preview will show your current in-progress changes instead of only the last saved version, so you no longer have to save first just to see how something looks. (#292)
- **[Bug]** **Some saved offer options never reach live ads** — A number of offer settings are saved but don't currently make it through to what visitors actually see. This work makes sure each option either works end-to-end or is cleaned up so nothing is misleading. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — High priority. Conversion pixels set on offers currently never fire, so conversions go unrecorded with no visible error. This fix restores accurate conversion tracking. (#297)
- **[Feature]** **Automatic performance projection for new offers** — New offers will get a data-driven estimate of how they're likely to perform, based on your own historical offer data, replacing the manual gut-check review. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — High priority. Auto-register offers currently fire for everyone, ignoring age, gender, state, zip, and device targeting. This ensures they follow the same audience rules as regular offers. (#333)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This offer field can be filled in but has no effect on which offers are shown. This work confirms what it's meant to do and then makes it work or removes it. (#351)

## Surveys

- **[Feature]** **Design options fully connected to the survey** — Every customization on the Design tab will actually appear in the live survey, with a thorough check across all screens to fix or remove any option that currently does nothing. (#288)
- **[Feature]** **Placement design settings applied to the live widget** — Placement Design-tab settings (like survey height and display format) will properly affect the survey as visitors see it. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore after-success delivery steps** — Post-conversion delivery and redirect behavior from the old system will be carried over so those client flows work as they used to. (#327)
- **[Feature]** **Restore custom pre-conversion checks** — High priority. Custom serve-time validation used by hundreds of data clients in the legacy system isn't running on the new platform yet; this brings that validation back. (#338)

## Admin / Users

- **[Task]** **Users screen feature review** — A side-by-side comparison of the new Users area against the old system to spot and close missing capabilities, such as bulk actions and extra columns. (#80)
- **[Feature]** **Remove controls that don't do anything** — Several admin controls that look editable but have no effect (for example the Advertiser Web Presence fields and certain user permission toggles) will be hidden or removed to avoid confusion. (#296)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a testing space that mirrors real production data so changes can be verified without any risk to live data. (#270)
- **[Feature]** **Turn conversations into tracked tasks automatically** — A helper that reads team conversations and creates or updates tracked work items, cutting out manual copy-and-paste. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work** — The Modal Design tab settings currently have no effect on what visitors see. They'll either be wired up so they apply, or removed if the modal is meant to have no header. (#294)

## Reports & Dashboard

- **[Task]** **Investigate mismatched report numbers** — Looking into why some Dashboard report figures don't match the legacy system, to pin down the cause and confirm the numbers are accurate. (#271)

## Properties

- **[Bug]** **Allowed-domains list isn't being enforced** — The allowed-domains setting on Properties is currently ignored, so ads can be served on any site. This fix makes the list actually block sites that aren't approved, while leaving properties that haven't set a list unaffected. (#350)

## Flows

- **[Task]** **Tidy up the Flow form layout** — Parts of the Flow form currently look unstyled or misaligned, with fields stacking oddly. This cleans up the layout so it matches the other forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
