# Open Issues — Plain-Language Overview

_Last updated 2026-07-03 15:39:19 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Survey

- **[Feature]** **Design choices show up on the live survey** — Every customization you make on a survey's Design tab will actually appear on the survey your visitors see, so nothing you set is silently ignored. (#288)
- **[Bug]** **Survey styling settings that currently do nothing** — Many Design-tab options (colors, continue button, header text, legal text, progress bar) are saved but don't change the live survey today. This work makes them take effect as expected. (#290)
- **[Bug]** **Missing voucher code and info links on live surveys** — A configured voucher code line and the privacy/terms/details links weren't showing on the live survey even though they're set up in the admin. This restores them to match the older system. (#291)
- **[Feature]** **Finish connecting the rest of the survey Design settings** — A remaining handful of survey styling and behavior options will be either wired up to the live widget or cleaned out of the form so there are no dead controls. (#293)

## Dashboard

- **[Feature]** **Pick report dates right in the dashboard** — You'll be able to choose a day or date range from controls in the dashboard instead of editing the web address by hand, while still getting a shareable link. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (for example to a spreadsheet). High priority. (#286)
- **[Task]** **Confirm dashboard numbers match the old system** — Behind-the-scenes review comparing new dashboard report figures against the legacy system for the same dates, so you can trust the numbers. (#271)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else is already editing a record, you'll see who has it open, and the app will warn you before your save could wipe out their changes. This protects records across all entity screens. (#267)
- **[Feature]** **A searchable history of who changed what** — A new admin Audit Log will record every change to offers, placements, advertisers, and more (including automatic changes), so you can look up who changed something and when. (#276)
- **[Feature]** **Clean up admin controls that do nothing** — Several settings that appear editable but currently have no effect (some advertiser web-presence fields, certain user permission toggles, and a few data-client/pre-ping options) will be hidden or removed to avoid confusion. (#296)

## Lead Processing & Compliance

- **[Feature]** **TrustedForm compliance handling** — Adds proper claiming and retaining of compliance certificates for leads and hardens the lead pipeline before it goes live. Ongoing, high priority. (#309)
- **[Bug]** **Stop the same lead being sent twice** — Fixes a case where a lead could be delivered to an advertiser more than once if a later step failed, preventing double-billing and advertiser-trust issues. High priority. (#303)
- **[Bug]** **Stop pointless retries on unfixable failures** — Leads that are correctly rejected (duplicate, do-not-call, validation) will no longer be retried needlessly, keeping the system cleaner and error alerts more meaningful. (#304)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on placements** — The default offer sort will honor your manual ordering, and you'll be able to filter the available offers list by category so it's easier to find the right ones. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show your current in-progress edits instead of only the last saved version, so you can check changes before saving. (#292)

## Offers

- **[Bug]** **Saved offer options that never reach the live experience** — Several offer settings are saved but don't currently make it through to what visitors see; this ensures each one is either applied or removed so nothing is misleading. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels configured on offers currently never fire, meaning lost tracking. This fixes them so a configured pixel actually fires on success. High priority. (#297)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — Every field on the modal's Design tab is currently saved but has no effect on the visitor modal. This work will either connect those fields or remove the tab so it's honest. (#294)

## Properties

- **[Bug]** **Domain restrictions that currently have no effect** — Website domain settings on Properties are saved but ignored at run time, so allow-listing doesn't work today. This makes those restrictions actually take effect. (#300)

## Flows

- **[Task]** **Fix unstyled and misaligned Flow form elements** — Parts of the Flow form look broken or unstyled and some paired fields stack vertically instead of side by side. This cleans up the form's appearance to match the other screens. (#152)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — The new platform doesn't yet have the Campaigns area from the older system. This adds the ability to view, create, edit, and configure campaigns and their offer groups. Critical, high priority. (#200)

## Users

- **[Task]** **Compare the Users area to the old system** — A review of what the legacy Users management offered versus the new one, so gaps like bulk actions and extra columns can be prioritized and closed. (#80)

## Link Testing

- **[Bug]** **Show a clear error for invalid links** — Testing an invalid link currently dumps you on the dashboard with no explanation; this will show a clear failure message instead. Nearly complete. (#239)

## Behind the Scenes

- **[Task]** **A safe, read-only staging environment** — Sets up a test environment loaded with production-like data that can be reviewed without any risk of changing live records. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — An internal helper that reads team conversations and files them as tracked tasks automatically, reducing manual note-taking. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d38d8ca1795a452a0f0d67dcfaeace8d181daef5615cf577e333d88f335aa7ae -->
