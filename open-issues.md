# Open Issues — Plain-Language Overview

_Last updated 2026-07-16 21:21:35 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Conversion pixels aren't firing on successful offers** — A high-priority fix so that the tracking pixels set up on offers actually fire when someone completes an offer. Right now they're silently doing nothing, which means completed conversions aren't being counted. Once fixed, you'll get accurate credit for the results you're driving. (#297)
- **[Task]** **Auto-register offers will respect audience targeting** — A high-priority fix so that "auto-register" offers honor the same age, gender, state, ZIP, and device rules as regular offers. Today they can fire for visitors who should be excluded; this makes their targeting consistent and trustworthy. (#333)
- **[Bug]** **Saved offer settings will actually reach live offers** — Several options you set on an offer (including modal settings, display URL, and various delivery flags) aren't currently making it through to what visitors see. This work makes sure each saved setting either works as expected or is removed so it isn't misleading. (#295)
- **[Feature]** **Preview offers and placements with your unsaved changes** — The Preview button will show the edits you're currently making, rather than the last saved version. You'll be able to check how a change looks before committing to it. (#292)
- **[Feature]** **Smarter performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform, based on your historical offer data, replacing the old manual gut-check. It would give you a data-grounded read on expected results at intake. (#322)

## Surveys

- **[Feature]** **Design settings will consistently show up in the survey** — A full sweep to make sure every customization option in the Design tab actually takes effect in the live survey, with no "dead" options that look adjustable but do nothing. You'll be able to trust that what you set is what visitors see. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live survey** — Some placement design options (like survey height and display format) are saved but never applied. This wires them up so they work, and cleans up any options that were never truly connected. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back file-based pre-ping checks for data clients** — A high-priority effort to restore custom, serve-time validation rules for hundreds of data clients that don't yet run on New Adsmith Frontend. Once complete, those clients' checks will run again so leads are validated as they were before. (#338)
- **[Feature]** **Restore post-success delivery steps for data clients** — The legacy "after-success" delivery and redirect behavior is being ported over. Affected data clients will again get the correct follow-up actions after a successful conversion. (#327)

## Admin & Users

- **[Task]** **Reviewing the Users area against the old system** — A documentation effort comparing the new Users management screens to the legacy version to spot any missing capabilities (like bulk actions or last-login info). This guides what still needs to be added for a complete experience. (#80)
- **[Feature]** **Cleaning up admin controls that don't do anything** — Certain settings (such as the Advertiser Web Presence tab, some user permission toggles, and a few data-client and pre-ping options) currently save but have no effect. They'll be removed or hidden so the admin screens only show controls that genuinely work. (#296)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design tab's settings (header title, colors, progress bar, and more) currently don't appear in the modal visitors see. This work will either make those settings take effect or remove the tab, so it's no longer misleading. (#294)

## Flows

- **[Task]** **Polishing the look of the Flow form** — Some parts of the Flow form appear unstyled or awkwardly laid out compared to other screens. This tidies up the form's appearance so paired fields sit side by side and everything matches the rest of the app. (#152)

## Dashboard & Reports

- **[Task]** **Investigating dashboard report numbers vs. the old system** — Reviewers noticed dashboard report figures didn't match the legacy system. This looks into where the difference comes from and confirms the numbers can be trusted, so reporting lines up as expected. (#271)

## Behind the Scenes

- **[Task]** **Read-only staging environment for testing** — Setting up a safe, view-only copy of the app running against realistic data, used for testing and verification without any risk of changing live records. (#270)
- **[Feature]** **Turning conversations into tracked work items automatically** — A tool to capture action items from team chats and log them as tracked issues, reducing manual copy-and-paste. This is an internal workflow improvement with no direct change to the product screens. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->
