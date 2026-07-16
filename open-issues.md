# Open Issues — Plain-Language Overview

_Last updated 2026-07-16 23:18:18 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on Placements and Offers** — Right now the Preview button shows the last saved version of a placement or offer. Once this is done, Preview will reflect the edits you're making on screen, so you can check your work before saving. (#292)
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of options you set on an offer (including modal fields, display URL, and several delivery flags) are being dropped and never take effect. This fix makes sure each saved option is actually used, or is cleared out if it isn't needed. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — A high-priority fix. Conversion pixels set up on an offer are silently failing to fire, which means lost tracking and attribution. Once fixed, the pixels you configure will reliably fire on a successful conversion. (#297)
- **[Feature]** **Automatic performance estimates for new offers** — Instead of relying on a manual gut-check review, new offers will get a data-driven projection of how they're likely to perform, based on your existing offers and their history. This is an exploratory decision aid to help judge new offers faster. (#322)
- **[Bug]** **Auto-register offers ignore visitor targeting** — A high-priority fix. Auto-register offers currently fire for every visitor, even ones who should be excluded by age, gender, state, zip, or device. This corrects them so they respect the same targeting rules as regular offers. (#333)

## Surveys

- **[Feature]** **Make every Design-tab option actually change the survey** — We're reviewing all the customization options across every screen to confirm each one truly affects what visitors see. Any option that isn't connected will be wired up or removed, so nothing on the form is misleading. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Some placement design settings (like iframe height and display format) are saved but don't yet change the visitor experience. This connects the remaining settings, or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore after-conversion delivery behaviors** — Certain post-conversion delivery and redirect steps from the old system weren't carried over yet. This brings them back so affected clients keep working as they did before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — A high-priority fix. Hundreds of data clients rely on custom validation checks that currently don't run on the new platform. This ports those checks so the right leads are accepted or rejected as they were in the old system. (#338)

## General / Across the App

- **[Task]** **Review of the Users management screen versus the old system** — A behind-the-scenes comparison of the new Users area against the legacy one, identifying which features are missing or improved. This guides what to add next so the Users screen reaches full capability. (#80)
- **[Feature]** **Remove controls that don't do anything** — Several admin settings (such as the Advertiser Web Presence tab, some user permission toggles, and a few data-client and pre-ping options) look active but have no effect. They'll be hidden or removed so the screens only show controls that actually work. (#296)

## Behind the Scenes

- **[Task]** **Read-only test environment using real-world data** — Setting up a safe, view-only copy of the app loaded with production-like data, so the team can verify behavior without any risk of changing live records. (#270)
- **[Feature]** **Automatic ticket creation from team conversations** — A helper that reads designated chat conversations and turns action items into tracked work items automatically, cutting out manual copy-and-paste. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work, or remove it** — The Modal Design tab's header and progress-bar settings currently have no effect on what visitors see. This will either connect them so they display properly or remove them to avoid confusion. (#294)

## Flows

- **[Task]** **Fix styling on the Flow form** — Parts of the Flow form look unfinished: some text boxes, color pickers, and checkboxes appear unstyled, and paired fields stack awkwardly instead of sitting side by side. This tidies up the form so it matches the rest of the app. (#152)

## Dashboard & Reports

- **[Task]** **Investigate report numbers that don't match the old system** — During testing, some dashboard report figures didn't line up with the legacy system. This looks into where the difference comes from and confirms the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->
