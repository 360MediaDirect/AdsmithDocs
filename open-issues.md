# Open Issues — Plain-Language Overview

_Last updated 2026-07-04 11:30:48 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make every survey design option actually take effect** — We're checking each customization on the survey's Design tab so the choices you make (and any options across other screens) really show up for visitors instead of being saved but ignored. (#288)
- **[Bug]** **Design settings that don't reach the live survey** — Right now only a couple of the survey's styling and behavior settings (like colors, the continue button, headers, and legal text) actually change what visitors see. This work connects the rest so the survey looks the way you set it up. (#290)
- **[Bug]** **Voucher code and info links missing on the live survey** — A configured voucher code line and the privacy/terms/details links aren't appearing on the new survey page even though they're set up correctly, and they do show in the old system. This restores both. (#291)
- **[Feature]** **Finish connecting the last few survey Design settings** — A handful of remaining Design-tab settings (such as height and display format) still don't affect the live survey. Each will either be made to work or removed so nothing on the form is misleading. (#293)

## Admin & Users

- **[Task]** **Review of what's missing in the new Users area** — A side-by-side comparison of the old and new Users screens to catch gaps like bulk actions, last-login and two-factor status, so the new Users management can catch up to what you had before. (#80)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else is already editing a record, you'll see who has it open and be kept from accidentally saving over their changes, with a clear prompt to reload if something changed while you were working. (#267)
- **[Feature]** **Clear out admin controls that don't do anything** — Some settings (like the Advertiser Web Presence fields, certain user permission toggles, and a few Data Client and Pre-Ping options) are saved but have no effect. They'll be removed or hidden so the admin only shows controls that truly work. (#296)

## General / Across the App

- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every manual and automated change across the product with a timestamp and who made it, so you can look up exactly when and by whom a record was edited. (#276)
- **[Bug]** **Invalid links should show an error, not send you to the Dashboard** — When you test a link that's invalid, you'll get a clear failure message instead of being unexpectedly dropped onto the Dashboard. (#239)

## Placements

- **[Feature]** **Better control over the offers list on a placement** — New placements will default to your Manual Order (so the order you arrange actually sticks), plus you'll be able to filter the available offers by category to find them faster. (#275)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — The Preview button will show the edits you're currently making rather than the last saved version, so you can check your work without having to save first. (#292)

## Dashboard

- **[Task]** **Look into Dashboard numbers not matching the old system** — We're comparing report figures between the old and new platforms over the same dates to find and explain any differences, so you can trust the Dashboard numbers. (#271)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example as a spreadsheet) for your own analysis. (#286)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a testing copy of the product using production-like data where nothing can be changed, so the team can verify things safely before release. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads team chat and files the resulting to-dos for us, reducing manual copy-and-paste and helping make sure requests don't slip through the cracks. (#272)

## Offers

- **[Bug]** **Some saved Offer settings never reach the live widget** — A number of saved offer options (including the Modal-tab fields and several other flags) currently get dropped before they can affect what visitors see. Each will be connected properly or removed if it's not needed. (#295)

## Modals

- **[Feature]** **Make the Modal Design tab do something** — The six settings on the Modal Design tab are saved but have no effect on the visitor-facing modal. They'll either be wired up to actually change the modal or removed so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or awkwardly stacked compared with other forms. This tidies up the layout and styling so paired fields, text boxes, and color pickers display cleanly. (#152)

## Campaigns

- **[Feature]** **Bring Campaigns into the new platform** — The Campaigns area from the old admin isn't in the new one yet. This adds it back so you can view, create, edit, and configure campaigns and their offer groups just like before. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
