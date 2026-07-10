# Open Issues — Plain-Language Overview

_Last updated 2026-07-10 17:34:15 UTC · 23 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Testing an invalid offer link now shows a clear error** — Instead of quietly bouncing you back to the dashboard, entering a bad link will return a proper "this didn't work" message so you know the test failed. (#239)
- **[Feature]** **Preview your unsaved changes on placements and offers** — The Preview button will show the edits you're currently making, not just the last saved version, so you can check your work before committing it. (#292)
- **[Bug]** **Some saved offer settings aren't reaching the live page** — A number of offer options (including Modal-related fields, Display URL, and several data-client flags) are saved in the admin but never show up for visitors. This work makes sure each one either takes effect or is removed so nothing is misleading. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up under "Pixels to Fire on Success" currently never actually fire, meaning some conversions go unrecorded. This fix gets them working end to end. (#297)
- **[Feature]** **Automatic performance projections for new offers** — A new tool will estimate how a fresh offer is likely to perform based on your historical offer data, replacing the old manual gut-check review. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently ignore age, gender, state, zip, and device targeting and can fire for people they should exclude. This work confirms and corrects that behavior. (#333)
- **[Feature]** **Better Placement and Offer pickers on Offer Link Testing** — The dropdowns will load every placement and offer, let you search by name or ID, and default to a standard placement, making link testing much faster. (#347)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When someone opens a record for editing, others will see it's locked and by whom, and the system will warn you if a record changed while you had it open — so no one silently loses their work. (#267)
- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every manual and automated change to your records, with the person or system responsible and a timestamp, so you can always answer "who changed this and when." (#276)
- **[Feature]** **Removing admin controls that don't do anything** — Several settings (like the Advertiser Web Presence fields, some user permission toggles, and a few Data-Client and Pre-Ping options) are saved but currently have no effect. They'll be removed or hidden so the admin only shows controls that actually work. (#296)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-sharing page has no equivalent yet. This is a keep-or-retire decision to confirm whether anyone still needs it. (#328)

## Surveys

- **[Feature]** **Design tab settings will fully carry through to the live survey** — Every customization you set on the design tab will actually appear on the survey visitors see, with a full check across all screens to catch any options that currently do nothing. (#288)
- **[Bug]** **Voucher codes and info links missing from live surveys** — Configured voucher codes and the privacy/terms/details links show correctly in the old app but aren't appearing on the new survey page. This fix restores them, which matters for both conversions and compliance. (#291)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A handful of Placement design options (such as survey height and display format) are saved but not yet reflected on the live survey. Each will be wired up or removed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior for data clients** — The legacy "after-success" scripts that ran after a conversion weren't carried over. This brings that behavior back for the clients that still rely on it. (#327)
- **[Feature]** **Bring legacy pre-ping validation to the new platform** — Hundreds of data clients used custom serve-time validation checks that currently don't run on the new platform. This work restores those checks so leads are validated as before. (#338)

## Data & Reporting

- **[Task]** **Confirm the new dashboard reports match the old system** — Report numbers in the new platform didn't line up with the legacy app during testing. This investigation pins down why and confirms the figures you rely on are accurate. (#271)

## Flows

- **[Task]** **Tidy up the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other forms. This cleanup brings its layout and styling in line with the rest of the app. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab actually work** — All six settings on the Modal Design tab currently have no visible effect. Each will either be connected to the visitor modal or removed so the tab only shows what genuinely applies. (#294)

## Campaigns

- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — Campaign management from the old admin isn't available yet. This adds the ability to view, create, edit, and configure campaigns and offer groups, matching the legacy workflow. (#200)

## Users

- **[Task]** **Review the Users area against the old system** — A detailed comparison of the old and new Users screens to identify which features (like bulk actions, 2FA status, and last-login info) still need to be brought over. (#80)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of the app running against realistic data, locked to read-only so testing can happen safely without changing anything live. (#270)
- **[Feature]** **Turn conversations into tracked to-dos automatically** — A helper that reads team discussions and files the resulting action items for the team, reducing manual note-taking and follow-up. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 644378381710b4e7d907d237d4ef51cbe58ac839f9f1749c90d1103f1b99993e -->
