# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 05:03:32 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach the live page** — Several options you set on an offer (including its Modal-tab fields, "Force More Info Visible," Display URL, and certain delivery flags) are saved but currently have no effect on what visitors see. Each will be properly connected or removed so the form only shows options that actually do something. (#295)
- **[Feature]** **Preview unsaved changes on placements and offers** — The Preview button will show your in-progress edits instead of only the last saved version, so you can check how a change looks before committing it. (#292)
- **[Task]** **Auto-register offers should respect visitor targeting** — Auto-register offers can currently fire for visitors they should exclude (by age, gender, state, zip, or device). This work confirms the correct behavior and makes those offers honor your targeting rules. (#333)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, giving you a data-driven gut-check at intake. (#322)

## Surveys

- **[Bug]** **Design settings that don't actually change the survey** — Many styling and behavior options on the Placement Design tab (colors, continue button, question text, header, legal text, progress bar) are saved but don't currently affect the live survey. This work connects them so what you configure is what visitors see. (#290)
- **[Bug]** **Voucher code and info links missing on the live survey** — A custom question (voucher code) and the privacy/terms/details links configured for a data client aren't showing on the survey page, even though they appear in the legacy app. This fix restores them, which matters for lead delivery and compliance. (#291)
- **[Feature]** **Finish connecting the remaining survey design options** — A follow-up pass to wire up the last few Design-tab settings (such as survey height and display format) and to either activate or remove a handful of options that still have no effect. (#293)
- **[Feature]** **Make sure every design option truly works everywhere** — A full review across all entities to confirm each customization option flows from the form through to what visitors actually see, with any unused options fixed or removed. (#288)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is editing a record, others will see it's locked and by whom, and you'll be warned if a record changed while you had it open — so edits are no longer silently lost. (#267)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings that appear in the admin but have no real effect (Advertiser Web Presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping options) will be hidden or removed to avoid confusion. (#296)
- **[Task]** **Users management: what's still missing vs. the old system** — A documented comparison between the old and new Users areas that identifies gaps (like bulk actions and 2FA status) to guide bringing the new screen up to par. (#80)
- **[Task]** **Decide the fate of the old file-share page** — A quick review to confirm whether the legacy file-share page is still needed, then either add it to the new admin or officially retire it. (#328)

## Reports & Dashboard

- **[Task]** **Confirm dashboard numbers match the legacy system** — An investigation into why some dashboard report figures differed from the old system, pinpointing the cause so you can trust the numbers you see. (#271)
- **[Bug]** **Testing an invalid link should show a clear error** — Right now, entering an invalid link quietly sends you to the dashboard. Instead, you'll get a clear failure message telling you the link didn't pass. (#239)

## Modals

- **[Feature]** **Make the Modal Design tab actually work** — Every field on the Modal Design tab (header title, subtitle, colors, progress bar) is currently saved but has no effect on the visitor modal. Each will be either connected so it displays or removed from the form. (#294)

## Flows

- **[Task]** **Fix visual glitches on the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other screens. This tidies up the layout so text boxes, color pickers, and paired fields display cleanly. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns area into the new platform** — The Campaigns module from the old admin isn't available yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups, matching the legacy workflow. (#200)

## Pre-Pings

- **[Feature]** **Restore legacy pre-ping coverage** — An older, per-client pre-ping method isn't available in the new platform, which could affect offers that still rely on it. This work ports the missing behavior or confirms the new pre-ping fully covers it. (#330)

## Data Clients

- **[Feature]** **Bring back after-success delivery for data clients** — The legacy post-conversion delivery/redirect behavior hasn't been carried over yet. This determines which of those behaviors are still needed and rebuilds them in the new platform. (#327)

## Behind the Scenes

- **[Task]** **Read-only staging environment for safe testing** — Setting up a staging copy of the app wired to production-like data for verification, with safeguards so no changes can be made there. (#270)
- **[Feature]** **Automatically turn Slack discussions into tracked tasks** — A helper that reads designated Slack conversations and files action items as tracked issues, cutting out manual copy-and-paste. (#272)
- **[Feature]** **Company-wide history log of changes** — A searchable record of every change to key records (who changed what and when), plus per-record history, to make troubleshooting far easier. (#276)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: db2e2e32afdf249c2931b9305c5b4e9f6e133e4b3e0fdf0fc98b37cd3f75c917 -->
