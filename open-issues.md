# Open Issues — Plain-Language Overview

_Last updated 2026-07-05 09:01:26 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make every survey design option actually change the survey** — A wide review is underway to ensure each customization on the Design tab (colors, buttons, text styles, headers, and more) truly shows up in the live survey visitors see, with no settings that quietly do nothing. (#288)
- **[Bug]** **Design-tab styling that doesn't reach the live survey** — Today most survey styling choices are saved but never applied to what visitors see. This work connects those settings — headers, progress bar, button and answer styling, legal text and more — so what you configure is what shows. (#290)
- **[Feature]** **Finish connecting the last survey design settings** — A follow-up to fully wire up the remaining Design-tab options (like survey height and display format) so they take effect, and to clean up any options that don't belong. (#293)
- **[Bug]** **Missing voucher code and info links on live surveys** — For affected data clients, the voucher code line and the privacy/terms/details links are configured but not appearing on the live survey the way they did in the old system. This fix restores them. (#291)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is editing a record, others will see a clear "being edited by…" notice, and you'll be warned instead of accidentally saving over a change someone else just made. Applies across all the entity screens. (#267)
- **[Feature]** **A searchable history of who changed what** — A new audit log will record every change to offers, placements, advertisers, and more — both manual edits and automated updates — so admins can look up who changed something and when. (#276)
- **[Feature]** **Tidy up admin controls that don't do anything** — Some settings (like the Advertiser Web Presence fields and a few user-permission toggles) are saved but have no real effect. These will be removed, hidden, or properly implemented so the screens only show controls that actually work. (#296)
- **[Bug]** **Invalid links send you to the dashboard instead of an error** — When testing a link that isn't valid, you're currently bounced to the dashboard. This fix will show a clear failure message right in the Link Testing screen. (#239)

## Placements & Offers

- **[Feature]** **Better control over the offer list on placements** — New placements will default to your manual offer order (so the order you set is actually used), and you'll be able to filter the available offers by category to find them faster. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show the changes you're currently making, so you no longer have to save first just to see how an edit looks. (#292)
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of offer options are saved but get dropped before they display to visitors. This fix ensures those settings either take effect or are cleaned up if they're not needed. (#295)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example to a spreadsheet) for your own analysis. High priority. (#286)
- **[Task]** **Checking dashboard numbers against the old system** — An investigation into why some dashboard report figures don't match the legacy system, to pinpoint and fix any differences so you can trust the numbers. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The Modal Design tab settings (header title, colors, progress bar) currently have no effect on the modal visitors see. This work will either connect them so they work or remove them to avoid confusion. (#294)

## Flows

- **[Task]** **Polish the look of the Flow form** — Fixing unstyled text boxes, color pickers, and checkboxes, and letting paired fields sit side by side, so the Flow form looks as clean and consistent as the other forms. (#152)

## Campaigns

- **[Feature]** **Bring Campaigns into New Adsmith Frontend** — The Campaigns area from the old admin is being rebuilt so you can view, create, edit, and manage campaigns and their offer groups — including titles, question text, CTA text, and offer handling. High priority. (#200)

## Users

- **[Task]** **Compare the Users area with the old system** — A detailed review of the old and new Users screens to identify missing capabilities (such as bulk role changes, last-login, and two-factor status) so they can be planned back in. (#80)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of New Adsmith Frontend using production-like data for testing and verification, locked to read-only so nothing can be changed by accident. (#270)
- **[Feature]** **Automatically turning conversations into tracked tasks** — An internal helper that reads team discussions and files the resulting to-dos automatically, reducing manual copy-and-paste and keeping work items up to date. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
