# Open Issues — Plain-Language Overview

_Last updated 2026-07-10 13:39:02 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels that admins set up under "Pixels to Fire on Success" currently never fire, so conversions may be going unrecorded. This high-priority fix will make configured success pixels reliably fire when a lead converts. (#297)
- **[Bug]** **Some saved offer settings never reach the live offer** — A number of options you can fill in on the Offer form (including the Modal-tab fields, "Force More Info Visible," Display URL, and several data-client flags) aren't actually carried through to what visitors see. Each will be either properly wired up or removed so the form only shows options that do something. (#295)
- **[Bug]** **bPerx voucher code missing from the offer preview** — For bPerx offers, the "Your Voucher Code" line that should appear isn't showing in the preview (and likely the live survey) on the test environment. This fix restores the voucher code so previews match what customers expect. (#344)
- **[Task]** **Auto-register offers now respect visitor targeting** — Auto-register offers are currently skipping the age/gender/state/zip/device rules, so they can fire for visitors who should be excluded. Once addressed, these offers will honor the same targeting rules as regular offers. (#333)
- **[Feature]** **Preview shows your unsaved edits** — On placement and offer edit screens, the Preview button will reflect the changes you're currently making instead of only the last-saved version, so you can check your work before saving. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your own historical offer data, replacing the informal manual gut-check. It's meant as a helpful decision aid at offer intake. (#322)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When two admins open the same record, the app will warn that someone else is editing and prevent one person's save from silently wiping out the other's changes. This will work consistently across all entity screens. (#267)
- **[Feature]** **A searchable activity history for every change** — A new Audit Log will record who changed what and when across offers, placements, advertisers, and more (including automated changes), so you can answer "who changed this and when." (#276)
- **[Feature]** **Cleaning up controls that don't do anything** — Several admin fields that currently save but have no effect (Advertiser Web Presence links, some user permission toggles, a couple of Data-Client and Pre-Ping options) will be removed or hidden so the interface only shows controls that actually work. (#296)
- **[Bug]** **Clearer error when testing an invalid link** — Testing an invalid link currently dumps you on the dashboard with no explanation; instead you'll see a clear failure message in the Link Testing screen. (#239)
- **[Task]** **Decision on the legacy file-share page** — The old file-share page has no equivalent yet. This is a review to decide whether it's still needed and should be rebuilt, or safely retired. (#328)

## Surveys

- **[Bug]** **Voucher code and info links missing on the live survey** — For an affected data client, the voucher code line and the privacy/terms/details links are configured but not appearing on the new survey page (they show in the old app). This fix restores both, which matter for passing leads and for compliance. (#291)
- **[Feature]** **Design-tab customizations fully reflected in the survey** — A thorough check to make sure every design/customization option you set actually shows up in the survey, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A handful of Placement Design-tab options (like survey height and display format) aren't yet applied to the live survey. Each will be either wired up so it takes effect or removed from the form. (#293)

## Pre-Pings

- **[Feature]** **Display pre-pings will run the real check at serve time** — Certain pre-pings currently only check that a field exists rather than performing the actual advertiser check, so offers that should be hidden can still show. This high-priority fix makes them behave like the legacy system and hide rejected offers. (#337)
- **[Feature]** **Bringing over legacy per-client pre-ping checks** — Custom pre-ping validations used by hundreds of data clients in the old system haven't been carried over yet. This work maps and re-enables those checks so offers are validated correctly before being shown. (#338)

## Reports

- **[Task]** **Confirming report numbers match the legacy system** — Some dashboard report figures didn't line up with the old app during testing. This investigation pins down where the difference comes from and either corrects it or confirms the numbers are right. (#271)
- **[Feature]** **Offer impressions restored in historical placement reports** — Historical placement reports currently show offer impressions as zero. This improvement populates that figure so the reports show accurate offer-impression counts. (#339)

## Modals

- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — All six fields on the Modal Design tab currently save but have no effect on what visitors see. Each will be either connected to the visitor modal or removed from the form. (#294)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacking instead of sitting side-by-side). This cleanup brings the Flow form in line with the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bringing the Campaigns module to the new platform** — The Campaigns module from the old admin isn't in New Adsmith Frontend yet. This high-priority work adds the ability to view, create, edit, and configure campaigns and their offer groups, matching the legacy system. (#200)

## Data Clients

- **[Feature]** **Restoring after-success delivery behavior** — Legacy post-conversion delivery/redirect steps for certain clients haven't been carried over yet. This work brings those behaviors back as a configurable option so active clients keep working as before. (#327)

## Admin / Users

- **[Task]** **Reviewing the Users area against the old system** — A documentation review comparing the new Users screens to the legacy version to spot missing features (like bulk actions, last-login, and two-factor status) and prioritize what to add. (#80)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the app connected to production-like data for testing, locked to read-only so it can't accidentally change real records. (#270)
- **[Feature]** **Turning conversations into tracked work items automatically** — A helper that reads designated Slack conversations and files or updates GitHub issues automatically, reducing manual copy-paste when capturing action items. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 20c05265760e30b087db164aa9ffb7701fea9cb19d23bb2497ef9c503a36041b -->
