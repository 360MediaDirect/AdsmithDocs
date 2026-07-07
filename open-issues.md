# Open Issues — Plain-Language Overview

_Last updated 2026-07-07 01:34:20 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make every survey Design setting actually take effect** — When you customize a survey's look and behavior, those choices will reliably appear in the live survey. We're checking each option across the product to make sure nothing is a dead setting that saves but does nothing. (#288)
- **[Bug]** **Connect the rest of the survey Design settings to what visitors see** — Today only a couple of the roughly thirty styling and behavior options on the Placement Design tab actually reach the published survey. This wires up the rest (colors, buttons, header text, legal text, and more) so what you set is what visitors get. (#290)
- **[Bug]** **Restore the voucher code and info links on live surveys** — For some data clients, the custom voucher-code question and the privacy/terms/details links are set up correctly but aren't showing on the live survey the way they did before. This brings them back. (#291)
- **[Feature]** **Finish wiring the remaining Placement Design settings** — A handful of leftover Design-tab settings (such as height and display format) will either start working on the live survey or be removed if they aren't needed, so nothing misleading remains. (#293)

## General / Across the App

- **[Task]** **Close the gaps between the old and new Users area** — A review comparing the legacy Users screens with the new ones, so missing pieces like bulk role changes, extra filters, and login details can be planned and added. (#80)
- **[Feature]** **Stop two people from overwriting each other's edits** — When someone else is already editing a record, you'll see a clear notice and won't be able to accidentally save over their changes. This protection will apply across all editable screens. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will be able to look up who changed what and when across offers, placements, advertisers, and more — including automated changes — making it much easier to track things down. (#276)
- **[Feature]** **Remove settings that don't do anything** — Several controls (like the Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) currently save but have no effect. These will be removed or hidden so the interface only shows things that actually work. (#296)

## Offers & Placements

- **[Feature]** **Better control over offer order and filtering on Placements** — New placements can default to your manual offer order so your arrangement is respected, and you'll be able to filter the available offers list by category instead of only searching by text. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit screens will show your current in-progress edits, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Make sure saved offer settings reach the live experience** — Several offer options are saved but never actually make it to what visitors see. This ensures each saved field either takes effect or is cleaned up if it's not meant to be used. (#295)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory feature to estimate how a new offer is likely to perform, based on your own historical offer data, giving a helpful data-driven read at intake instead of relying on a manual gut-check. (#322)

## Behind the Scenes

- **[Task]** **A safe, view-only testing environment** — Setting up a testing space that uses realistic, production-like data in read-only mode, so the team can verify the product without any risk of changing real records. (#270)
- **[Feature]** **Turn team conversations into tracked work automatically** — A helper that reads designated chat channels and files or updates work items from them, cutting out manual copy-and-paste when capturing action items. (#272)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Fixes styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields look consistent with the rest of the product instead of appearing plain or misaligned. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — Right now the Modal Design tab's settings (header title, subtitle, colors, progress bar) save but don't affect the visitor modal. These will either be connected to the live modal or removed so the tab isn't misleading. (#294)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — The Campaigns area from the old admin isn't in the new platform yet. This adds it back so you can create, edit, and manage campaigns and their offer groups — a core capability that's currently missing. (#200)

## Reports

- **[Task]** **Investigate why dashboard report numbers don't match the old system** — A review comparing report figures between the legacy system and the new platform over the same dates, to pinpoint any differences and confirm the numbers can be trusted. (#271)

## Link Testing

- **[Bug]** **Show a clear error for invalid links** — When you test a link that isn't valid, you'll get a clear failure message instead of being unexpectedly sent to the dashboard. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: b39611ee25f08f99131383e979b65278c59628a3fdeb736c1b956498b1042356 -->
