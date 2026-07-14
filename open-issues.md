# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 19:30:24 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on an offer ("Pixels to Fire on Success") currently never fire, so those conversions go unrecorded with no visible error. This high-priority fix makes configured success pixels fire reliably again. (#297)
- **[Task]** **Auto-register offers now respect visitor targeting** — Auto-register offers currently fire for everyone, ignoring age, gender, state, zip, and device targeting rules. This work makes them honor targeting (or clearly documents the intended behavior) so offers only reach the right visitors. High priority. (#333)
- **[Bug]** **Some saved offer settings never reach live pages** — Several saved offer options (such as modal settings, Display URL, and a few data-client flags) are currently dropped before visitors ever see them. Fixing this ensures the settings you save actually take effect. (#295)
- **[Feature]** **Preview shows your unsaved changes** — On the placement and offer edit pages, the Preview button will reflect the changes you've made but not yet saved, so you can check your edits without having to save first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — New offers will get an automated, data-driven estimate of how they're likely to perform, based on your historical offer data — replacing the old manual gut-check review. (#322)

## Admin / Across the App

- **[Feature]** **Prevent two people from overwriting each other's work** — When someone opens a record for editing, others will see it's locked and by whom, and you'll be warned if a record changed while you had it open — so edits can't be silently wiped out by a second editor. (#267)
- **[Feature]** **Full activity/audit log** — A new searchable log will record every change across the app — who made it, what changed, and when — including automated changes, making it easy to answer "who changed this and when?". (#276)
- **[Task]** **Users screen feature review** — A review comparing the new Users area with the older version to close gaps like bulk role changes, last-login, and two-factor status. This is a planning and documentation step. (#80)
- **[Feature]** **Remove controls that don't do anything** — Several admin settings that look active but have no effect (Advertiser Web Presence fields, a couple of user permission toggles, Data-Client Template/Gateway, and the Pre-Ping Hash option) will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Decide the future of the file-share page** — The older file-share page has no equivalent yet; this decides whether to rebuild it or retire it for good. (#328)

## Surveys / Modals

- **[Feature]** **Make design options actually apply** — A review across all entities to confirm every design-tab customization is fully connected, so the styling choices you make are reflected in the live survey view rather than quietly doing nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings** — Placement design options like iFrame height and display format will be fully wired up so they take effect (and any leftover options that go nowhere will be either connected or removed). (#293)
- **[Feature]** **Wire up or remove the Modal Design tab** — The Modal Design tab's six settings (header text, colors, progress bar) currently have no effect. This work either makes them work in the visitor modal or removes them so the tab isn't misleading. (#294)

## Data Clients / Pre-Pings

- **[Feature]** **Restore custom pre-ping validation for data clients** — Custom serve-time checks used by 448 data clients from the older system aren't running on the new platform. This high-priority work brings that validation back so those clients behave as expected. (#338)
- **[Feature]** **Bring over after-success delivery** — The older post-conversion delivery/redirect behavior for certain clients hasn't been carried over yet. This restores that step so conversions continue to hand off correctly. (#327)

## Flows

- **[Task]** **Fix Flow form styling** — Parts of the Flow form currently look unstyled or misaligned — plain text boxes, unstyled color pickers, and paired fields stacking instead of sitting side by side. This tidies up the form to match the rest of the app. (#152)

## Campaigns

- **[Feature]** **Add the Campaigns module** — Campaign management isn't available in New Adsmith Frontend yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups, matching what the older admin could do. High priority. (#200)

## Reports & Dashboard

- **[Task]** **Look into mismatched dashboard report numbers** — During testing, some dashboard report figures didn't match the older system. This investigation finds where the difference comes from and confirms the numbers can be trusted. (#271)

## Behind the Scenes

- **[Task]** **Safe testing environment** — Setting up a look-but-don't-touch staging copy that mirrors real data, so new work can be verified against realistic information without any risk of changing live records. (#270)
- **[Feature]** **Auto-create tasks from conversations** — An internal helper that reads team conversations and files the resulting to-dos automatically, so action items are captured without manual copying. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
