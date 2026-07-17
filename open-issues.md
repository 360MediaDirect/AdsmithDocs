# Open Issues — Plain-Language Overview

_Last updated 2026-07-17 01:33:54 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Right now the "pixels to fire on success" you set up on an offer silently never run, so conversions aren't being recorded and you get no error to warn you. This high-priority fix will make configured success pixels reliably fire, restoring accurate conversion and revenue tracking. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for every visitor, even ones outside the age, gender, state, ZIP, or device targeting you've set. This fix will make those offers respect the same targeting rules as regular offers, so they only fire for the right audience. (#333)
- **[Bug]** **Some saved offer settings never reach the live offer** — A number of options you can set on an offer (including its Modal-tab fields, Display URL, and several data-client flags) are being dropped and never take effect for visitors. This work will make sure each saved setting is either actually used or removed from the form so nothing is misleading. (#295)
- **[Feature]** **Preview unsaved changes on placements and offers** — Today the Preview button shows the last saved version, so you have to save before you can see your edits. Once done, Preview will reflect your current in-progress changes, letting you check your work before committing it. (#292)
- **[Feature]** **Predict how a new offer will perform** — Instead of relying on a manual gut-check, this explores an automated projection of a new offer's likely performance based on your historical offer data. It would give you a data-driven estimate at intake to help decide whether an offer is worth running. (#322)

## Surveys

- **[Feature]** **Make every survey design setting actually work** — This reviews all customization options across the product's forms to confirm each one is truly connected to what visitors see. The result is that the choices you make on a design tab reliably show up in the live survey, with no dead options. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — A handful of Placement design options (like iFrame height and display format) are saved but not yet applied to the visitor-facing survey. This finishes wiring them up so your settings take effect, and removes any that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore custom pre-check rules for data clients** — Hundreds of data clients rely on custom serve-time validation that hasn't yet been carried over to New Adsmith Frontend, so that logic isn't running today. This high-priority work will bring those checks back so leads are validated as expected before delivery. (#338)
- **[Feature]** **Bring back post-conversion delivery steps** — Certain client-specific actions that run after a successful conversion weren't carried over from the old system. This work restores them as a reusable, configurable option so those clients keep working as before. (#327)

## Admin & Users

- **[Task]** **Close the gap between the old and new Users area** — A detailed review compares the old Users management screens with the new ones to spot missing capabilities (like bulk actions, password entry, and login/2FA info). The outcome guides which features to add so the new Users area is as capable as the old one. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings across screens (Advertiser web presence fields, certain user permission toggles, and some data-client and pre-ping options) are saved but have no effect, which is confusing and misleading. This will hide or remove them so every control you see actually works. (#296)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of the app will be connected to production-like data for verification, locked to read-only so nothing can be accidentally changed. This lets the team validate the product against realistic data without any risk to live information. (#270)
- **[Feature]** **Auto-create task items from team conversations** — A helper that reads designated team chat channels and turns action items into tracked tasks automatically, avoiding manual copy-paste. It's a workflow convenience for the team and has no direct effect on the product screens. (#272)

## Modals

- **[Feature]** **Make the Modal design tab work (or remove it)** — The entire design tab for modals is currently saved but never shown to visitors. This will either build those header and progress-bar options into the live modal or remove the tab, so what you configure matches what visitors actually see. (#294)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form look unstyled or misaligned — plain text boxes, unstyled color pickers, and paired fields stacking vertically instead of side by side. This cleanup brings the Flow form in line with the polished look of the other forms. (#152)

## Reports & Dashboard

- **[Task]** **Confirm dashboard report numbers match the old system** — During testing, some dashboard report totals didn't line up with the legacy app, making it hard to trust the numbers. This investigation compares the two over a fixed period to find and explain any differences and confirm the figures are accurate. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->
