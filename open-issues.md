# Open Issues — Plain-Language Overview

_Last updated 2026-07-07 21:31:50 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Protection against two people editing the same record at once** — When someone opens a record (an offer, placement, advertiser, and so on) to edit it, others will see it's already being worked on and won't be able to accidentally overwrite each other's changes. If a record was changed while you had it open, you'll be prompted to reload instead of losing work. (#267)
- **[Feature]** **A searchable history of who changed what** — Administrators will get an audit log that records every change across the app, both by people and by automated processes, with timestamps and before/after details. You'll be able to answer "who changed this, and when?" right from a record's history. (#276)
- **[Feature]** **Cleaning up settings that don't actually do anything** — Several admin controls (some Advertiser web-presence fields, a couple of user permission toggles, and a few Data-Client and Pre-Ping options) currently save but have no effect. These will be removed or hidden so the screens only show settings that really work. (#296)
- **[Bug]** **Invalid links in Link Testing will show a clear error** — Right now, testing a bad link quietly sends you to the dashboard. After this fix, you'll get a proper error message telling you the link failed. A high-priority fix that's nearly finished. (#239)
- **[Task]** **Closing gaps in the Users area** — An ongoing review comparing the older Users management screens with the new ones, to bring back missing capabilities (like bulk actions and richer user details) so nothing important is lost in the move. (#80)
- **[Task]** **Deciding the future of the old File Share page** — The legacy file-share page has no equivalent yet. This is a decision on whether to rebuild it or officially retire it. (#328)

## Surveys
- **[Feature]** **Making every survey design setting actually take effect** — A thorough check to ensure that each customization you set on the design tab is genuinely reflected in the live survey, with any settings that do nothing being fixed or removed. (#288)
- **[Bug]** **Most survey styling options aren't reaching visitors yet** — Around 30 look-and-feel settings (colors, buttons, headers, legal text, and more) can be saved but don't currently change what visitors see. This work wires them through so your design choices actually appear. High-progress work. (#290)
- **[Bug]** **Voucher codes and info links missing on the live survey** — A configured voucher-code question and the privacy/terms/details links aren't showing on the new survey page even though they're set up correctly. This fixes the display so they appear like they did before — important for both leads and compliance. (#291)
- **[Feature]** **Finishing the last few survey design settings** — Wraps up the remaining design-tab options (such as survey height and display format) that weren't completed earlier, so each one either works in the live survey or is removed from the form. (#293)

## Offers
- **[Feature]** **Preview edits before saving** — On placement and offer edit screens, the Preview button will show your current unsaved changes instead of the last-saved version, so you can check how an edit looks without saving first. (#292)
- **[Bug]** **Some saved offer settings never reach the live offer** — A number of offer options (including modal-related fields and several backend flags) are saved but dropped before they get to what visitors see. Each will be properly connected or cleaned up so offers behave as configured. (#295)
- **[Feature]** **Automatic performance estimates for new offers** — An exploratory feature to predict how a new offer is likely to perform based on your historical offer data, giving the team a data-driven gut-check at intake instead of relying on a manual review. (#322)
- **[Task]** **Auto-register offers should respect visitor targeting** — Auto-register offers currently fire for everyone, ignoring age, gender, state, zip, and device targeting. This work makes them honor the same targeting rules as regular offers (or documents it as intentional), so offers don't reach people they should exclude. High priority. (#333)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging version of the product using production-like data that can't be changed, so the team can verify things against realistic data without any risk to live records. (#270)
- **[Feature]** **Turning Slack conversations into tracked tasks** — A helper that reads designated Slack discussions and automatically files the action items as tracked issues, cutting out manual copy-and-paste. (#272)

## Flows
- **[Task]** **Tidying up the Flow form's appearance** — Some parts of the Flow form look unstyled or misaligned compared to other forms (text boxes, color pickers, checkboxes, and side-by-side fields). This is a careful clean-up so the Flow form matches the rest of the app. Partially done. (#152)

## Campaigns
- **[Feature]** **Bringing the Campaigns area into the new platform** — The Campaigns module from the older admin isn't in the new one yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups, matching what the legacy system does. A critical, high-priority addition. (#200)

## Modals
- **[Feature]** **Making the Modal Design tab meaningful** — Every field on the Modal design tab currently saves but has no visible effect. This work either connects them to the visitor-facing modal or removes the tab if a header isn't needed. (#294)

## Pre-Pings
- **[Feature]** **Restoring legacy pre-ping coverage** — An older per-client pre-ping capability isn't available in the new platform, which could affect offers that still rely on it. This confirms what's still needed and rebuilds the missing path. High priority. (#330)

## Reports
- **[Task]** **Making dashboard report numbers match the old system** — Reviewers noticed dashboard figures didn't line up with the legacy app. This investigation pins down where the difference comes from and either corrects it or confirms the numbers are trustworthy. (#271)

## Data Clients
- **[Feature]** **Restoring post-conversion delivery for data clients** — Certain after-success behaviors (delivery and redirect steps that run once a lead converts) haven't been carried over yet. This work determines which are still needed and rebuilds them in the new platform. (#327)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: db2e2e32afdf249c2931b9305c5b4e9f6e133e4b3e0fdf0fc98b37cd3f75c917 -->
