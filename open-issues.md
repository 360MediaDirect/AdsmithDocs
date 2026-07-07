# Open Issues — Plain-Language Overview

_Last updated 2026-07-07 12:47:57 UTC · 23 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make every survey design choice show up on the live survey** — We're going through all the design and customization options and making sure each one actually changes what visitors see, fixing or removing any setting that currently has no effect. (#288)
- **[Bug]** **Most survey styling settings don't reach the published survey** — About thirty look-and-feel settings on the Placement Design tab (colors, continue button, header text, legal text, progress bar, and more) are saved but don't appear on the live survey today. This work makes them take effect so what you set is what visitors get. (#290)
- **[Bug]** **Voucher code and info links missing on the live survey** — For affected clients, the voucher code line and the privacy/terms/details links are set up in the admin but aren't showing on the live survey page the way they did before. This restores them so leads and compliance links display correctly. (#291)
- **[Feature]** **Finish connecting the last few survey design settings** — A handful of remaining Placement Design settings (such as height, display format, and skip behavior) will either start working on the live survey or be removed if they're no longer needed, so nothing on the form is misleading. (#293)

## General / Across the App

- **[Feature]** **Stop two people from overwriting each other's edits** — When someone opens a record to edit it, others will see it's being worked on, and the system will warn you if a record changed while you had it open — so nobody's changes get silently lost. (#267)
- **[Feature]** **A searchable history of every change** — A new activity log will record who changed what and when across the product, including automated changes, so you can answer "who edited this and when" and review past actions. (#276)
- **[Feature]** **Remove settings that don't actually do anything** — Several controls (like the Advertiser Web Presence fields, some user permission toggles, and a few data-client and pre-ping options) are saved but currently have no effect. We'll hide or remove them so the screens only show controls that really work. (#296)
- **[Task]** **Decide the future of the legacy file-share page** — We'll confirm whether the old file-share page is still needed and either give it a home in the new product or formally retire it. (#328)

## Offers

- **[Bug]** **Some saved offer options never reach the live page** — Around fourteen offer settings (including the offer's modal fields and a "force more info" option) are saved but don't currently affect what visitors see. Each will be wired up to work or cleared away if it's not needed. (#295)
- **[Feature]** **Automatic performance estimate for new offers** — Instead of a manual gut-check, new offers could get an automated projection of likely performance based on our own history of past offers — an at-a-glance decision aid when reviewing incoming offers. (#322)
- **[Task]** **Auto-register offers should respect targeting rules** — Auto-register offers currently fire for every visitor even when age, gender, state, zip, or device targeting is set. We'll confirm the intended behavior and make these offers honor the same targeting rules as regular offers. (#333)

## Placements

- **[Feature]** **Preview your unsaved changes** — The Preview button on Placement and Offer edit screens will show the changes you've just made, even before you save, so you don't have to save first just to see how something looks. (#292)
- **[Feature]** **Bring back the banner placement type** — We'll confirm whether banner placements are still in use and, if so, rebuild that placement type in the new product so it works like it did before. (#326)

## Reports & Dashboard

- **[Task]** **Look into dashboard numbers not matching the old system** — During testing, some dashboard report totals didn't line up with the legacy system. We're comparing the two over a fixed date range to find and explain any differences, and confirm the numbers are trustworthy. (#271)
- **[Bug]** **Testing an invalid link should show a clear error** — Right now, entering an invalid link during link testing sends you to the dashboard. This fix will show a clear failure message instead so you know the link didn't pass. (#239)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design tab's fields (header title, subtext, colors, progress bar) currently don't affect the visitor modal. We'll either make them take effect or remove the tab if the modal is meant to have no header. (#294)

## Campaigns

- **[Feature]** **Bring the Campaigns module into the new product** — The Campaigns feature from the old admin isn't in the new product yet. This adds it back so you can view, create, edit, and configure campaigns and their offer groups. This is a high-priority, core piece of functionality. (#200)

## Flows

- **[Task]** **Fix the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other forms (plain text boxes, unstyled color pickers, fields stacking instead of sitting side by side). This tidies up the layout so it matches the rest of the product. (#152)

## Pre-Pings

- **[Feature]** **Restore the older per-client pre-ping behavior** — An older pre-ping method used by some offers isn't available in the new product yet. We'll confirm which offers still rely on it and make sure that behavior is fully covered so those offers keep working. This is high priority. (#330)

## Data Clients

- **[Feature]** **Bring over the after-conversion client steps** — Certain post-conversion delivery and redirect steps from the old system (for clients like bPerx and rwdb) haven't been carried over yet. We'll map each one to the new product or confirm it's no longer needed. (#327)

## Users

- **[Task]** **Compare the old and new Users screens** — A review is underway to spot anything the old Users area could do that the new one can't yet (like bulk role changes, last-login and two-factor status, and password setup), so we can plan what to add. (#80)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A separate environment that mirrors real data will be used for verification and testing, locked so nothing can be changed there. This helps us validate the product against realistic data without risk. (#270)
- **[Feature]** **A helper that turns conversations into tracked to-dos** — An assistant that reads designated chat channels and automatically logs action items as tracked tasks, cutting out manual copying and keeping follow-ups from slipping through the cracks. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 0f0dc75345ae083c3f2607503afd91bf3b9663925bf97592fab1f9e589c4ec62 -->
