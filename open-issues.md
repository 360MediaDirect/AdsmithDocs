# Open Issues — Plain-Language Overview

_Last updated 2026-07-11 01:33:51 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Bring back Campaigns management** — A high-priority effort to add the Campaigns area to New Adsmith Frontend so you can view, create, edit, and configure campaigns and offer groups just like you could in the older system. Right now there's no way to manage campaigns on the new platform. (#200)
- **[Bug]** **Success pixels now fire correctly** — A high-priority fix so the conversion tracking pixels you set up under "Pixels to Fire on Success" actually fire. Today they silently do nothing, which means lost tracking; this restores accurate attribution. (#297)
- **[Bug]** **Saved offer settings will reach live placements** — Several options you save on an offer (including its Modal-tab settings and Display URL) currently never make it through to what visitors see. This ensures the settings you configure actually take effect. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently ignore age, gender, state, zip, and device targeting, so they can show to people they should exclude. This makes them honor the same targeting rules as regular offers. (#333)
- **[Feature]** **Live preview of unsaved offer and placement edits** — The Preview button will show your current, in-progress changes instead of only the last saved version, so you can check your work before committing it. (#292)
- **[Feature]** **Automatic performance estimates for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, replacing the manual gut-check review that's being retired. (#322)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record for editing, others will see it's locked and by whom, and you'll be warned if a record changed while you had it open. This stops one person's save from silently wiping out another's changes. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when across the app (both people and automated jobs), with a per-record history view, so "who changed this?" finally has an answer. (#276)
- **[Feature]** **Clean up controls that don't do anything** — Several settings that appear to save but have no real effect (like the Advertiser Web Presence fields, certain user-permission toggles, and a few Data-Client and Pre-Ping options) will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Bringing the Users screen up to par with the old system** — A documentation and planning review comparing the old Users area to the new one, identifying missing pieces (like bulk actions and last-login info) so they can be prioritized. (#80)
- **[Task]** **Decide the future of the file-share page** — A quick review to confirm whether the old file-share page is still used by anyone or can be retired. (#328)

## Surveys

- **[Feature]** **Make every design option actually change the survey** — A full check that each customization on the Design tab is reflected in the live survey, with any unused options fixed or removed, so what you set is what visitors see. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A handful of Placement Design-tab settings (like survey height and display format) either aren't shown to visitors or aren't wired up; this connects them or removes the ones that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — A near-complete effort to bring the older "after success" delivery and redirect steps to the new platform for the clients that still rely on them. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — A high-priority effort to bring across the custom serve-time validation that 448 data clients depend on, which currently doesn't run on the new platform. (#338)

## Dashboard & Reports

- **[Bug]** **Clear error for invalid links** — When testing a link that isn't valid, you'll get a clear failure message instead of being unexpectedly sent to the dashboard. (#239)
- **[Task]** **Confirm report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy app during testing, to find and fix any discrepancy and confirm the numbers can be trusted. (#271)

## Behind the Scenes

- **[Task]** **A safe, read-only testing environment** — Setting up a copy of the app loaded with production-like data that can be reviewed and verified without any risk of changing real data. (#270)
- **[Feature]** **Turn Slack conversations into tracked tasks automatically** — A helper that reads designated Slack channels and files action items as tracked issues, saving the manual step of copying notes over by hand. (#272)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Some parts of the Flow form look unstyled or misaligned; this tidies up the layout so it matches the polish of the Placement and Modal forms. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The six settings on the Modal Design tab currently have no effect on what visitors see. This will either wire them up so they work or remove them to avoid confusion. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
