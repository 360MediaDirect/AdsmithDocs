# Open Issues — Plain-Language Overview

_Last updated 2026-07-03 18:27:24 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Warn when two people edit the same record** — When you open a record to edit, others will see it's being worked on, and if someone else changes it while you have it open, you'll be prompted to reload instead of silently overwriting their work. This protects against lost changes across all entity screens. (#267)
- **[Feature]** **Bring the Campaigns module into New Adsmith Frontend** — A high-priority addition. You'll be able to view, create, edit, and configure campaigns — including offer groups, CTA text, and offer handling — just as you can in the legacy admin. (#200)
- **[Feature]** **Remove settings that don't actually do anything** — Some controls (like the Advertiser "Web Presence" fields, a couple of user permission toggles, and some Data-Client and Pre-Ping options) are saved but have no effect. These will be hidden or removed so the screens only show settings that truly work. (#296)
- **[Bug]** **Show a clear error when a tested link is invalid** — In Link Testing, entering a bad link currently sends you to the Dashboard. Once fixed, you'll see a proper error message instead. (#239)
- **[Task]** **Review of the Users area against the legacy system** — A behind-the-scenes comparison of the old and new Users screens to plan which features still need to be brought over (such as bulk actions and login/2FA details). (#80)

## Surveys

- **[Feature]** **Make sure every Design tab option actually changes the survey** — An end-to-end review confirming that each customization you set on the Design tab is reflected in what visitors see, with any settings that do nothing fixed or removed. (#288)
- **[Bug]** **Connect the remaining survey Design settings to the live survey** — Many survey styling and behavior options (colors, buttons, header text, progress bar, legal text, and more) are saved but don't yet affect the live widget. This work makes them take effect as expected. (#290)
- **[Feature]** **Finish connecting the last few survey Design settings** — Wraps up the remaining survey settings (like iFrame height and display format) so they render correctly, and cleans up any that won't be used. (#293)
- **[Bug]** **Restore the voucher code and info links on the live survey** — For affected data clients, the voucher code line and the privacy/terms/details links aren't showing even though they're set up in the admin. This fix brings them back, matching the legacy display. (#291)

## Placements

- **[Feature]** **Better ordering and filtering for placement offers** — New placements will be able to default to Manual Order so your drag-to-reorder actually takes effect, and you'll be able to filter the available offers list by category. (#275)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — The Preview button will show the edits you've made in the form, even before saving, so you no longer have to save first just to see how a change looks. (#292)

## Dashboard

- **[Feature]** **Export the breakdown-by-day view** — A new export button will let you download the day-level breakdown data for use in a spreadsheet. (#286)
- **[Task]** **Investigate report numbers that don't match the legacy system** — A review to find and explain why some Dashboard report figures differ from the old app, so the numbers can be trusted and validated. (#271)

## Offers

- **[Bug]** **Make sure saved offer options reach the live experience** — Several offer settings are saved but never make it to the live widget. This work ensures each saved option either takes effect or is cleaned up if it's no longer needed. (#295)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design tab's settings (header title, subtitle, colors, progress bar) currently have no effect. They'll either be connected to the visitor modal or removed so the screen isn't misleading. (#294)

## Flows

- **[Task]** **Fix the appearance of the Flow form** — Some parts of the Flow form look unstyled or misaligned compared to other forms. This tidies up the layout so paired fields, text boxes, and color pickers display properly. (#152)

## Behind the Scenes

- **[Task]** **Set up a read-only test environment with production-like data** — A staging setup that mirrors real data for safe testing and verification, with changes blocked so nothing can be accidentally altered. (#270)
- **[Feature]** **A Slack helper that turns conversations into tracked tasks** — An internal tool to automatically capture action items from Slack discussions and file them as tracked issues, reducing manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
