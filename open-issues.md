# Open Issues — Plain-Language Overview

_Last updated 2026-07-12 01:33:51 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings don't reach live pages** — A few options you set on an offer (including its modal fields, a "force more info" setting, display URL, and several data-handling flags) currently get dropped before they take effect. Once fixed, the choices you make on an offer will actually show up where visitors see them. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up under "Pixels to Fire on Success" silently never fire, which means completed conversions aren't being reported. This high-priority fix ensures the pixels you configure actually run when a conversion happens, so your attribution data is accurate. (#297)
- **[Task]** **Auto-register offers ignore visitor targeting** — Auto-register offers are being served to visitors even when age, gender, state, ZIP, or device targeting should exclude them. This high-priority fix will make these offers respect the same targeting rules as regular offers (or clearly document any intentional difference). (#333)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, new offers could be scored against your historical offer data to estimate how they're likely to perform. You'd get a helpful projection at intake to guide decisions. (#322)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — Right now the Preview button shows the last-saved version, so you have to save before you can see edits. Soon Preview will reflect your current, unsaved changes so you can check your work before committing it. (#292)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When two users open the same record, one can unknowingly save over the other's changes. This adds a clear "someone else is editing this" notice and warns you if a record changed while you had it open, preventing lost work. (#267)
- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every change to your records — who made it, when, and what changed — including automated updates. You'll be able to search this history and view it right from an entity's detail page. (#276)
- **[Feature]** **Clean up controls that don't do anything** — Several admin settings (Advertiser Web Presence fields, some user permission toggles, and a few Data Client and Pre-Ping options) are shown but currently have no effect. These will be removed or hidden so the screens only offer controls that actually work. (#296)
- **[Task]** **Decide the future of the file-share page** — The old file-share page has no equivalent in New Adsmith Frontend. This is a decision to either bring it back or officially retire it, so there's no confusion about where it went. (#328)
- **[Bug]** **Invalid links should show an error, not bounce to the Dashboard** — When you test an invalid link, you're currently sent to the Dashboard instead of seeing a clear failure message. This fix will show a proper error result so you know the link didn't work. (#239)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a testing environment that mirrors real data but can't change anything, so the team can verify behavior against production-like data without risk. (#270)
- **[Task]** **Investigating why some report numbers differ from the old system** — Reviewers noticed dashboard report figures didn't line up with the legacy system. This investigation will pinpoint the cause and confirm the numbers can be trusted. (#271)
- **[Feature]** **Turning conversations into tracked work automatically** — A helper that reads team conversations and files the resulting to-dos automatically, reducing manual follow-up. No visible change in the product itself. (#272)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — Certain "after success" delivery and redirect steps from the old system weren't carried over. This brings that behavior back for the clients that still rely on it. (#327)
- **[Feature]** **Restore custom pre-ping validation for data clients** — Hundreds of data clients relied on custom serve-time checks that don't currently run in New Adsmith Frontend. This high-priority work brings that validation back so those clients behave as expected. (#338)

## Surveys

- **[Feature]** **Make survey design options actually change the survey** — An end-to-end check to ensure every design/customization option you set is reflected in what visitors see, with any dead options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — A handful of Placement design settings (like survey height and display format) are saved but don't yet affect the survey. Each will be wired up so it works, or removed if it isn't needed. (#293)

## Modals

- **[Feature]** **Make the Modal design settings work** — The entire Modal Design tab (header text, colors, progress bar, etc.) currently has no effect on what visitors see. Each field will either be connected so it works or removed to avoid confusion. (#294)

## Flows

- **[Task]** **Fix the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned, with fields stacking oddly instead of sitting side by side. This tidies up the form so it matches the look of other screens. (#152)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — Campaign management from the old system isn't yet available in New Adsmith Frontend. This high-priority work adds the ability to view, create, edit, and configure campaigns and their offer groups. (#200)

## Admin / Users

- **[Task]** **Review of missing Users features vs. the old system** — A documented comparison of what the old Users area could do versus the new one, highlighting gaps like bulk actions and login/2FA details, to guide what to add next. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
