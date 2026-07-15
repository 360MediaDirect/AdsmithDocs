# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 19:28:17 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers to fire on success are currently being saved but never actually firing, meaning some conversions go untracked. This fix ensures configured success pixels fire reliably. High priority. (#297)
- **[Bug]** **Some saved offer settings never reach live pages** — A number of offer options (including the Modal-tab settings, several URL/display fields, and certain data-client flags) are saved but silently dropped before they reach the live experience. This work makes sure each option either takes effect or is cleaned up so nothing looks configurable when it isn't. (#295)
- **[Task]** **Auto-register offers should respect visitor targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting, so they can fire for people who should be excluded. This corrects the behavior (or documents it as intended) so targeting is applied consistently. High priority. (#333)
- **[Feature]** **Preview shows your unsaved changes** — On the placement and offer edit screens, Preview will reflect the edits you're currently making instead of only the last saved version, so you can check your changes before saving. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, giving you a data-driven gut-check at intake instead of relying on a manual review. (#322)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When someone opens a record for editing, others will see it's locked and by whom, and you'll be warned if a record changed while you had it open. This prevents one person accidentally wiping out another's changes across all entity screens. (#267)
- **[Feature]** **Remove controls that don't actually do anything** — Several settings (an Advertiser "Web Presence" tab, certain user permission toggles, and a few Data-Client and Pre-Ping options) look functional but currently have no effect. They'll be hidden or removed so the screens only show controls that truly work. (#296)
- **[Bug]** **Testing an invalid link should show a clear error** — Right now, entering an invalid link during link testing quietly sends you back to the dashboard. This fix gives you a proper error message so you know the link failed. (#239)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent in New Adsmith Frontend. This is a decision on whether to rebuild it or retire it for good. (#328)
- **[Task]** **Review of the Users area against the old system** — A documentation review comparing the Users screens in New Adsmith Frontend to the legacy system, so we can confirm what's carried over and what still needs attention. (#80)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back per-client "pre-ping" validation checks** — Hundreds of data clients relied on custom validation checks that ran before serving in the old system and aren't yet active in New Adsmith Frontend. This work restores those checks so client-specific rules apply again. High priority. (#338)
- **[Feature]** **Restore post-conversion delivery steps for clients** — The legacy "after-success" delivery and redirect steps for certain clients weren't carried over. This adds a flexible, configurable version so those clients keep working as expected after a conversion. (#327)

## Surveys & Placements

- **[Feature]** **Make sure every design option actually shows up** — A review across all screens to confirm each design and form option you set is truly reflected in the live survey view, with any unused options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A handful of Placement Design-tab settings (like iFrame height and display format) are saved but not yet applied to the live widget. This wires them through, or removes any that aren't needed. (#293)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A staging copy of the app running against production-like data, locked to read-only so it can be used for testing without any risk of changing real records. (#270)
- **[Feature]** **Automatically turn Slack conversations into tracked tasks** — A helper that reads designated Slack channels and files action items as tracked issues automatically, cutting out manual copy-and-paste from meeting notes. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — The Modal Design tab's fields (header text, colors, progress bar, etc.) are saved but don't currently appear in the visitor-facing modal. This either connects them so they take effect or removes the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned compared to other forms (plain text boxes, unstyled color pickers, fields stacking oddly). This gives the form a careful cleanup so it matches the rest of the app. (#152)

## Dashboard & Reports

- **[Task]** **Confirm dashboard report numbers match the old system** — During testing, some dashboard report figures didn't line up with the legacy app. This investigates where the difference comes from and either fixes it or confirms the numbers are correct. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d541cdec2d7ef7e80b16585fe689f12231c8b31406080f26d5421cd3a156890a -->
