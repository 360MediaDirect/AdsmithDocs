# Open Issues — Plain-Language Overview

_Last updated 2026-07-03 01:34:21 UTC · 28 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Protection against overwriting each other's edits** — When two people open the same record at once, you'll see who currently has it open, and you'll be warned before you can accidentally save over someone else's changes. (#267)
- **[Feature]** **Searchable history of changes** — A new Audit Log will record who changed what and when across the product (both manual edits and automated updates), so you can finally answer "who changed this and when?" and review a change history right from an item's page. (#276)
- **[Feature]** **Hide settings that don't actually do anything** — Several controls that look editable but currently have no effect (Advertiser Web Presence, some user permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden, so the screens only show settings that truly work. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper failure message instead of quietly sending you back to the Dashboard. (#239)
- **[Task]** **Review of the Users screen against the old system** — A behind-the-scenes comparison of the old Users area versus the new one, identifying which features are still missing so they can be prioritized. (#80)

## Leads & Compliance
- **[Feature]** **TrustedForm compliance tracking** — The larger effort to claim and safely store lead-verification certificates and harden the lead pipeline, so consent records are captured reliably before a lead is passed on. (#309)
- **[Feature]** **Turn cert-claiming on per advertiser** — A new toggle on the Data Client form will let you choose whether TrustedForm certificates are claimed for that client, instead of it only being changeable behind the scenes. (#305)
- **[Bug]** **Stop leads being sent to advertisers twice** — Fixes a rare case where a lead could be delivered to an advertiser more than once if something failed after the first successful send, protecting against double-billing and advertiser trust issues. (#303)
- **[Bug]** **Stop pointless retries of leads that can never succeed** — Leads that are rejected for good reasons (duplicate, do-not-call, failed validation) will no longer be retried repeatedly, keeping error reports cleaner and more trustworthy. (#304)
- **[Task]** **Review how long verification records are kept** — A policy check on how long TrustedForm certificate records (and the personal details they include) are retained, to confirm it meets data-protection requirements. (#306)

## Surveys
- **[Feature]** **Make Design tab settings actually change the survey** — A review to ensure every customization option on the Design tab is fully connected end-to-end, so the choices you make in the admin are reflected in what visitors see. (#288)
- **[Bug]** **Survey styling options that currently do nothing** — Many Design tab settings (colors, header, continue button, question text, legal text) are saved but don't yet affect the live survey; this connects them so your styling choices take effect. (#290)
- **[Feature]** **Finish connecting the last few survey settings** — Wraps up the remaining Design tab options that still aren't applied to the live survey, either making them work or removing ones that aren't needed. (#293)
- **[Bug]** **Voucher code and info links missing on live surveys** — Fixes a case where a configured voucher code line and the privacy/terms/details links don't appear on the live survey page even though they're set up in the admin. (#291)

## Dashboard
- **[Task]** **Pick your own date range on the Dashboard** — Choosing "Custom" in the date filter will open a start/end date picker so you can view Dashboard data for exactly the range you want. (#58)
- **[Feature]** **Change report dates without editing the web address** — New, easy-to-find date controls in the Dashboard will let you pull daily or custom-range reports directly, instead of having to hand-edit the address bar. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button will let you download the breakdown-by-day view (for example as a spreadsheet) for further analysis. (#286)
- **[Task]** **Check that report numbers match the old system** — An investigation into why some Dashboard report figures differed from the legacy system, to find the cause and confirm the numbers can be trusted. (#271)

## Offers
- **[Bug]** **Missing pixels never fire on a successful lead** — Fixes a case where success/conversion pixels configured on an offer were saved but never actually fired, which meant lost tracking with no visible error. (#297)
- **[Bug]** **Some saved offer settings never reach the live page** — Several offer options (including modal and more-info settings) are saved but get dropped before they reach visitors; this ensures each one is either applied or clearly retired. (#295)
- **[Feature]** **Preview offers and placements with your unsaved changes** — The Preview button will show your current in-progress edits, so you no longer have to save first just to see how a change looks. (#292)

## Behind the Scenes
- **[Task]** **A safe test environment with May and June data** — Sets up a separate practice environment loaded with real-looking data, so testing and report checks can happen without touching live information. (#270)
- **[Feature]** **Turn conversations into tracked work items automatically** — A Slack helper that reads discussions and files or updates issues automatically, reducing manual note-taking after meetings. (#272)

## Placements
- **[Feature]** **Better control over offer ordering and filtering** — Follows up on the offer selection list by considering making manual ordering the default and adding a way to filter available offers by category, so building a placement's offer list is faster. (#275)

## Modals
- **[Feature]** **Make the Modal Design tab work or remove it** — The Modal Design settings (header title, colors, progress bar) currently have no effect on what visitors see; this will either connect them or remove the tab to avoid confusion. (#294)

## Properties
- **[Bug]** **Domain restrictions that aren't taking effect** — Fixes a case where the allowed-domain settings on a Property are saved but ignored at run time, so domain restrictions you configure will actually be enforced. (#300)

## Campaigns
- **[Feature]** **Bring back the Campaigns area** — The Campaigns module from the old admin isn't in New Adsmith Frontend yet; this adds it so you can create, edit, and manage campaigns and their offer groups. High priority. (#200)

## Flows
- **[Task]** **Fix the appearance of the Flow form** — Addresses styling problems on the Flow form (plain text boxes, unstyled color pickers and checkboxes, fields stacking oddly) so it looks consistent with the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 0fee697ea8c356ff0dd7e2484fe5d7102761b0916f13b0161fbcef18cc7a1087 -->
