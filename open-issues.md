# Open Issues — Plain-Language Overview

_Last updated 2026-07-09 03:04:00 UTC · 24 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against two people editing the same record** — When someone opens a record to edit it, others will see it's locked and by whom, and the system will stop a save from quietly overwriting a change someone else just made. No more accidentally wiping out a colleague's edits. (#267)
- **[Feature]** **Full activity history of who changed what** — A searchable "Audit Log" will record every change to offers, placements, advertisers, and more — both by people and by automated jobs — with a timestamp and who made it, so you can finally answer "who changed this and when." (#276)
- **[Feature]** **Removing settings that don't actually do anything** — Several controls that look like they work but have no effect (some Advertiser Web Presence fields, certain user-permission toggles, and a few Data Client and Pre-Ping options) will be hidden or removed so screens only show settings that really matter. (#296)
- **[Bug]** **Invalid links now show a clear error** — Testing an invalid link currently dumps you back on the Dashboard with no explanation; this fix will show a proper failure message so you know the link didn't work. A high-priority fix that's nearly done. (#239)
- **[Task]** **Making warning and info banners look consistent** — Alert and info banners currently vary slightly in shade from screen to screen; this tidy-up ensures they all look identical across the app. (#341)
- **[Task]** **Deciding the future of the old file-share page** — A review of whether the legacy file-share page is still used, so it can either be rebuilt in the new platform or retired cleanly. (#328)
- **[Task]** **Comparing the old and new Users screens** — A documentation review lining up the legacy Users area against the new one to catch anything missing, such as bulk role changes and login/2FA details. This groundwork is well underway. (#80)

## Offers

- **[Bug]** **Some saved offer settings never reach the live page** — A number of offer options you can set and save (including Modal-tab settings, "Force More Info Visible," and Display URL) currently get dropped before they reach visitors. This fix ensures each saved setting either shows up live or is cleanly removed if it's not needed. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — Certain automatic offers currently fire for every visitor, ignoring age, gender, state, zip, and device targeting. This work makes sure they only show to the visitors they're meant for. A high-priority fix. (#333)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your own historical offer data, replacing today's manual gut-check review. (#322)

## Surveys

- **[Feature]** **Design tab changes will fully show up on the live survey** — An end-to-end check to make sure every customization you set on the design tab actually appears on the survey visitors see, with no dead options left behind. (#288)
- **[Bug]** **Voucher codes and info links missing on live surveys** — Voucher codes and the privacy/terms/details links you configure aren't showing on the new survey page even though they save correctly. Since the voucher code is needed to pass a lead and the links are compliance items, this high-priority fix restores them. (#291)
- **[Feature]** **Finishing the Placement design settings on surveys** — Several Placement design-tab settings (like iframe height and display format) are saved but not yet reflected on the live survey. This work wires each one through or removes it if unused. (#293)

## Placements

- **[Feature]** **Preview will show your unsaved changes** — On placement and offer edit screens, the Preview button will show your current edits rather than the last saved version, so you can check a change before committing it. (#292)
- **[Feature]** **Historical placement reports will show offer impressions** — Offer impressions currently show as 0 in older placement reports; this fills in that number so historical reporting is complete and accurate. (#339)

## Pre-Pings

- **[Feature]** **Display-trigger pre-pings will run real checks at show time** — Certain offers will properly check with the advertiser before being shown and be hidden if rejected, matching how the old system worked. A high-priority fix. (#337)
- **[Feature]** **Bringing over the legacy per-client pre-ping checks** — Hundreds of data clients rely on custom pre-ping validation from the old system that isn't running yet on the new platform. This work ports those checks so serve-time validation behaves as it should. High priority. (#338)

## Behind the Scenes

- **[Task]** **A read-only staging environment for testing** — Setting up a safe, prod-like environment for testing and verification where no changes can accidentally be written. Nearly complete. (#270)
- **[Feature]** **A Slack helper that turns conversations into tracked tasks** — A bot that reads designated Slack channels and files action items as tracked issues automatically, reducing manual copy-paste from meeting notes. (#272)

## Reports

- **[Task]** **Investigating why report numbers differ from the old system** — A deep-dive comparing dashboard report figures between the legacy and new platforms to find where any differences come from and confirm the numbers can be trusted. (#271)

## Data Clients

- **[Feature]** **Restoring after-success delivery behavior** — The post-conversion delivery and redirect steps from the old system are being rebuilt as a reusable, configurable option so active clients keep working as before. This work is nearly done. (#327)

## Modals

- **[Feature]** **Making the Modal Design tab actually work** — The Modal Design tab settings (header title, subtitle, colors, progress bar) currently save but don't appear to visitors. This work either connects them to the live modal or removes them if the modal is meant to be header-less. (#294)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear unstyled or awkwardly laid out compared to other forms. This tidy-up gives text boxes, color pickers, checkboxes, and paired fields a consistent, polished appearance. Partly done. (#152)

## Campaigns

- **[Feature]** **Bringing the Campaigns module to the new platform** — The Campaigns area from the old admin isn't in the new platform yet, so campaigns and offer groups can't be managed. This rebuilds it so you can view, create, edit, and configure campaigns as before. A critical, high-priority addition. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: e97c0c87fd1c264309b547c86ecde9d1b7abd3cebd9c6dc642ac728d6283da48 -->
