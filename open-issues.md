# Open Issues — Plain-Language Overview

_Last updated 2026-07-03 09:02:59 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Task]** **Reviewing the Users screens against the old system** — We're comparing the older Users management area to the new one to make sure nothing you rely on (like bulk role changes or last-login details) is missing before we finish the new screens. (#80)
- **[Feature]** **Warning when two people edit the same record** — If someone else is already editing an offer, placement, advertiser, or other record, you'll see who has it open and be protected from accidentally overwriting their changes. (#267)
- **[Feature]** **Searchable history of who changed what** — A new Audit Log will record every change across the app — by a person or an automated job — with a timestamp, so you can quickly answer "who changed this and when." (#276)
- **[Feature]** **Removing settings that don't actually do anything** — Some fields in the admin (certain Advertiser web-presence, user permission, Data Client, and Pre-Ping options) are being hidden or removed because they currently have no effect, so the screens only show controls that really work. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Testing an invalid link will show a proper failure message instead of silently sending you back to the dashboard. (#239)

## Surveys
- **[Feature]** **Design settings that actually change the survey** — We're making sure every option on the Design tab is reflected in the live survey, and auditing every entity's form options so nothing is a dead setting that looks active but does nothing. (#288)
- **[Bug]** **Most survey styling settings didn't reach visitors** — Many Design-tab options (colors, buttons, header text, legal text, and more) were saved but never showed up on the live survey; these are being connected so what you configure is what visitors see. (#290)
- **[Bug]** **Missing voucher code and info links on the live survey** — A configured voucher code line and the privacy/terms/details links weren't appearing on the new survey page even though they're set up in the admin; this restores them to match the older app. (#291)
- **[Feature]** **Finishing the remaining survey Design settings** — A handful of leftover Design-tab options (like survey height and display format) will either be wired up to the live survey or cleaned out of the form. (#293)

## Dashboard
- **[Feature]** **Pick report dates without editing the web address** — You'll be able to choose a day or date range directly from the dashboard toolbar instead of manually changing the address bar, while shareable links still keep working. (#268)
- **[Task]** **Making dashboard numbers match the old system** — We're investigating why some dashboard report totals differ from the legacy app so we can confirm the figures are accurate and consistent. (#271)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example, to a spreadsheet). (#286)

## Leads & Compliance
- **[Feature]** **Certifying leads for compliance (TrustedForm)** — Ongoing work to capture and retain compliance certificates before a lead is sent to an advertiser, with per-client controls, so lead delivery meets compliance requirements. (#309)
- **[Bug]** **Preventing the same lead being sent twice** — Fixing a case where a lead could be delivered to an advertiser more than once if a later step failed, which avoids duplicate submissions and double-billing. (#303)
- **[Bug]** **Stop retrying leads that can never succeed** — Leads that are permanently rejected (for example, duplicates or do-not-call) will no longer be retried repeatedly, keeping the system cleaner and error alerts more trustworthy. (#304)

## Offers
- **[Bug]** **Some saved offer options never reached the live page** — Several offer settings (including Modal-tab fields and display options) were being dropped before reaching visitors; each will be connected or cleaned up so saved settings behave as expected. (#295)
- **[Bug]** **Success tracking pixels weren't firing** — Conversion pixels set on an offer weren't actually firing because of a formatting mismatch; this fix ensures configured success pixels fire so you don't lose tracking. (#297)

## Placements
- **[Feature]** **Better defaults and filtering for offer ordering** — Follow-up work so a placement's manually arranged offer order is respected by default, and so you can filter the available offers by category when building the list. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit screens will show your current edits rather than only the last saved version, so you can check changes before saving. (#292)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the app against prod-like data for testing, with safeguards that prevent any accidental changes to that data. (#270)
- **[Feature]** **Turning Slack chats into tracked work items** — A helper that reads designated Slack conversations and automatically files the action items as tracked issues, reducing manual note-taking. (#272)

## Campaigns
- **[Feature]** **Bringing Campaigns into the new platform** — The Campaigns area from the old admin is being rebuilt so you can create, edit, and manage campaigns and their offer groups in New Adsmith Frontend. (#200)

## Modals
- **[Feature]** **Fixing the Modal Design tab** — The Modal Design tab's settings currently have no effect on what visitors see; each option will either be made to work or removed so the tab isn't misleading. (#294)

## Properties
- **[Bug]** **Domain restrictions weren't taking effect** — Domain settings entered on a Property weren't actually being applied at runtime; this fix makes the saved domain allow-list work as intended. (#300)

## Flows
- **[Task]** **Tidying up the Flow form's appearance** — Continuing to fix styling on the Flow form so fields, color pickers, and paired inputs display neatly instead of looking unstyled or misaligned. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d38d8ca1795a452a0f0d67dcfaeace8d181daef5615cf577e333d88f335aa7ae -->
