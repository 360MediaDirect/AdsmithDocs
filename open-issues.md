# Open Issues — Plain-Language Overview

_Last updated 2026-07-12 05:03:50 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — Conversion tracking pixels that admins set up under "Pixels to Fire on Success" are silently never firing, which means completed conversions aren't being tracked. This fix ensures configured success pixels actually fire so you don't lose credit for conversions. High priority. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several fields you can fill in on an offer (including the Modal-tab settings, Display URL, "Force More Info Visible," and certain data-client options) are being dropped before they reach visitors, so they have no effect. Each will be either fully wired up or removed so what you see on the form matches what actually happens. (#295)
- **[Task]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire for every visitor regardless of age, gender, state, ZIP, or device targeting, so they can reach people they should exclude. This work makes them respect the same targeting rules as regular offers (or documents the difference deliberately). High priority. (#333)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — Today the Preview button shows the last saved version, so you have to save before you can see a change. Soon Preview will reflect your current, unsaved edits so you can check your work before committing it. (#292)
- **[Feature]** **Smart performance projections for new offers** — An automated, data-driven estimate of how a new offer is likely to perform, based on your historical offer data — replacing the informal manual gut-check. It would give you a helpful performance projection right at offer intake. (#322)

## Admin & Users

- **[Feature]** **Protection against two people overwriting each other's edits** — When two admins open the same record, one can currently save over the other's changes without warning. This adds a gentle lock and a "this was changed by someone else — please reload" prompt so no one's work is silently lost. Works across all editable screens. (#267)
- **[Task]** **Users screen: closing gaps with the previous system** — A review of the Users area comparing it to the older system, identifying missing pieces like bulk actions, select-all, last-login and two-factor status, and password/notification options on the add-user form. This guides the work to bring the Users screen up to full capability. (#80)
- **[Feature]** **Clean up admin controls that don't do anything** — Some settings currently save but have no real effect (for example the Advertiser "Web Presence" fields, certain user-permission toggles, and a few Data-Client and Pre-Ping options). These will be hidden or removed so you're not misled into thinking a setting is working when it isn't. (#296)
- **[Task]** **Decide the future of the old file-share page** — The previous system had a file-share page with no equivalent here. This is a quick decision on whether it's still needed or can be retired. (#328)

## Surveys & Modals

- **[Feature]** **Design-tab settings that actually change the survey** — A thorough check to make sure every customization option on the Design tab is truly reflected in what visitors see, with any dead options fixed or removed across all screens. You'll be able to trust that the settings you change take effect. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live survey** — A handful of Placement Design-tab settings (like survey height and display format) are saved but not yet applied to the visitor experience. These will be fully wired up or removed so nothing on the form is misleading. (#293)
- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design tab's fields (header title, subtext, colors, progress bar) currently save but don't change the visitor modal at all. They'll either be made to work or removed so the tab isn't misleading. (#294)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back per-client validation checks at serve time** — The previous system ran custom pre-ping validation for 448 data clients that currently isn't running here, meaning those checks silently do nothing. This restores that validation so the right checks run again before offers are served. High priority. (#338)
- **[Feature]** **Restore post-conversion delivery behavior for data clients** — The "after-success" delivery and redirect steps from the old system (still needed for active clients) weren't carried over. This adds a flexible, configurable way to run them again after a conversion. (#327)

## Behind the Scenes

- **[Task]** **Safe, read-only test environment for verification** — Setting up a testing environment that mirrors production data but can't change anything, so the team can validate the product against realistic data without risk. (#270)
- **[Feature]** **Auto-create tasks from Slack conversations** — A helper that reads designated Slack channels and turns action items into tracked issues automatically, cutting out manual copy-and-paste and posting confirmation links back in Slack. (#272)

## General / Across the App

- **[Feature]** **A searchable history of who changed what** — A complete, tamper-proof log of every change across the product — manual and automated — with who did it and when, plus a searchable Audit Log page and per-record history. Makes it easy to answer "who changed this and when?" (#276)
- **[Bug]** **Clear error when testing an invalid link** — Testing an invalid link currently dumps you back on the dashboard with no explanation. This will instead show a clear failure message so you know the link didn't pass. Nearly complete. (#239)

## Flows

- **[Task]** **Tidy up the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned — plain textareas, unstyled color pickers and checkboxes, and paired fields stacking oddly instead of sitting side by side. This brings the Flow form in line with the polished look of the Placement and Modal forms. Partly done. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — Campaign management from the previous system isn't available here yet, so campaigns and offer groups can't currently be created or edited. This adds a full Campaigns area to view, create, configure, and manage campaigns and their offers. Critical, high priority. (#200)

## Dashboard & Reports

- **[Task]** **Make dashboard report numbers match the old system** — During testing, some dashboard report figures didn't line up with the previous system, making it hard to trust the numbers. This investigation pins down where the difference comes from and either fixes it or confirms the figures are correct. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
