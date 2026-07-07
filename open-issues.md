# Open Issues — Plain-Language Overview

_Last updated 2026-07-07 00:31:36 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make sure survey design settings actually change the survey** — We're checking that every option on the survey Design tab flows through to what visitors see, so nothing you customize is quietly ignored. Where an option isn't connected, it will be wired up or removed. (#288)
- **[Bug]** **Survey styling options that don't take effect** — Many Placement Design settings (colors, header text, continue button, progress bar, legal text and more) are saved but don't yet change the live survey. This fixes them so the survey looks the way you set it up. (#290)
- **[Bug]** **Voucher code and info links missing on the live survey** — For affected data clients, the custom voucher-code line and the privacy/terms/details links appear in the old app but not the new one. This restores them, which matters for both the visitor experience and compliance. (#291)
- **[Feature]** **Finish connecting the remaining survey design settings** — A handful of leftover Design-tab settings (such as survey height and display format) will either start affecting the survey or be removed so the form only shows options that do something. (#293)

## Offers, Placements & Campaigns

- **[Feature]** **Bring the Campaigns area to the new platform** — The Campaigns module from the old admin isn't in New Adsmith Frontend yet. This adds it back so you can create, edit, and manage campaigns and their offer groups again. High priority. (#200)
- **[Feature]** **Better default ordering and filtering when building offer lists on Placements** — New placements will be set to use your manual offer order by default, and you'll be able to filter the available offers by category instead of scrolling the whole list. (#275)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — The Preview button will show your current edits before you save, so you can check a change without having to save it first. (#292)
- **[Bug]** **Some saved Offer settings don't reach the live offer** — Several offer options are saved but never make it to what visitors see. This ensures those settings either take effect or are cleaned up so the form doesn't show options that do nothing. (#295)

## General / Across the App

- **[Feature]** **Warn when two people edit the same record** — When someone else is already editing a record, you'll see who has it open, and you'll be protected from accidentally overwriting each other's changes. Works across Offers, Flows, Placements, Advertisers, and other entity screens. (#267)
- **[Feature]** **A searchable history of who changed what** — Every change across the app (by a person or by an automated process) will be recorded with a timestamp, and administrators will get a searchable Audit Log plus a history view on entity pages — making "who changed this and when" easy to answer. (#276)
- **[Feature]** **Clean up controls that don't do anything** — Some admin settings (like the Advertiser Web Presence fields, certain user permission toggles, and a few Data Client and Pre-Ping options) are saved but have no effect. These will be removed or hidden so the screens only show controls that work. (#296)
- **[Task]** **Compare the new Users area against the old one** — A review of the legacy Users screens versus the new ones, so we can plan which missing features (like bulk actions and login/2FA details) to bring over. This is a documentation and planning task. (#80)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — You'll get an export button on the breakdown-by-day view so you can download that data (for example, to a spreadsheet). High priority. (#286)
- **[Bug]** **Offer Detail page times out for "Last Month"** — Opening an Offer Detail page with the date filter set to "Last Month" currently shows a load error. This fixes the timeout so the report loads normally. (#318)
- **[Task]** **Confirm dashboard numbers match the old system** — Testers noticed dashboard report figures didn't line up with the legacy app. We're investigating where the difference comes from and confirming the numbers are accurate. (#271)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the app against production-like data for testing, locked to read-only so nothing can be changed by accident. (#270)
- **[Feature]** **Turn meeting notes into tracked work automatically** — A helper that reads team conversations and files the resulting to-dos as tracked issues, reducing manual copy-and-paste. No direct effect on the app you use. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — The Modal Design tab's settings currently don't change the visitor modal. These will either be connected so they take effect or removed so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Fix the look of the Flow form** — Some parts of the Flow form appear unstyled or misaligned compared to other forms. This tidies up the layout so paired fields, color pickers, and text boxes look consistent and polished. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6c27af732f3641fd9b535e157afcb427a79ad241cf9415444c675c49de3c7588 -->
