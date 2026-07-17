# Open Issues — Plain-Language Overview

_Last updated 2026-07-17 13:31:36 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — When an advertiser sets up conversion tracking pixels to fire when an offer succeeds, those pixels currently never run, so conversions go unrecorded with no visible warning. This high-priority fix restores accurate tracking of successful conversions. (#297)
- **[Bug]** **Auto-register offers are ignoring visitor targeting** — Certain automatically-registered offers are being shown to visitors who should be excluded by age, gender, state, zip, or device rules. This high-priority fix ensures those offers respect the same targeting rules as regular offers. (#333)
- **[Bug]** **Some saved offer settings never reach live pages** — A number of options you set on an offer (including modal settings and several delivery flags) are saved but quietly dropped before reaching the live experience. This work makes sure the settings you configure actually take effect, or removes options that do nothing. (#295)
- **[Feature]** **Preview shows your unsaved edits on Placements and Offers** — The Preview button will reflect the changes you're currently making, even before saving, so you can check your work without having to save first. (#292)
- **[Feature]** **Predicted performance for new offers** — When a new offer comes in, New Adsmith Frontend will estimate how it's likely to perform based on your historical offer data, giving you a data-driven gut-check in place of a manual review. This is exploratory with no set deadline. (#322)

## Data Clients

- **[Feature]** **Port over post-conversion delivery behavior** — Legacy after-success delivery and redirect steps for certain clients haven't yet been carried into New Adsmith Frontend. This work brings those behaviors back so post-conversion handling continues to work for affected clients. (#327)
- **[Feature]** **Bring back file-based pre-ping checks** — Hundreds of data clients rely on custom serve-time validation checks that don't yet run on the new platform. This high-priority, large effort restores those checks so the right validation happens before offers are delivered. (#338)

## Surveys

- **[Feature]** **Design-tab settings actually change what visitors see** — Customizations you make on the design tab will be reliably reflected in the survey view, and every form option across the product will be checked to confirm it truly does something. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey widget** — Several placement design options (like survey height and display format) are saved but not yet shown to visitors. This work wires them through, or removes any option that isn't meant to be used. (#293)

## Admin / Users

- **[Task]** **Users screen comparison with the old system** — A review of the Users area against the previous system to identify which capabilities (like bulk actions and login details) are still missing, so they can be prioritized. This is a documentation and planning effort. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings across Advertisers, user permissions, and data-client screens are saved but have no effect. They'll be hidden or removed so the admin area only shows controls that actually work, avoiding confusion. (#296)

## Behind the Scenes

- **[Task]** **Read-only test environment for verification** — Setting up a safe, view-only copy of the app running against realistic data so the team can validate behavior without any risk of changing live records. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels and automatically logs action items, reducing manual note-taking and follow-up. (#272)

## Reports & Dashboard

- **[Task]** **Confirm dashboard numbers match the old system** — Investigating why some dashboard report figures differed from the legacy system during testing, so you can trust that the reports show consistent, accurate numbers. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — Every field on the Modal design tab currently has no effect on what visitors see. This work either wires those fields through so they change the modal, or removes the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly and inputs missing their intended styling. This cleanup brings the Flow form in line with the polished look of the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->
