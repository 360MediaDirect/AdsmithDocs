# Open Issues — Plain-Language Overview

_Last updated 2026-07-11 09:31:46 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Bring back the Campaigns module** — Campaign management from the old admin isn't in New Adsmith Frontend yet. Once added, you'll be able to view, create, and edit campaigns and manage their offer groups again — a high-priority, core piece of the migration. (#200)
- **[Bug]** **Success pixels aren't firing** — Conversion tracking pixels set on offers currently never fire, so conversions go unrecorded with no visible warning. This fix makes configured success pixels fire reliably again. (#297)
- **[Task]** **Auto-register offers are ignoring targeting rules** — Auto-register offers currently fire for every visitor, even ones who should be excluded by age, gender, state, ZIP, or device. This high-priority fix makes them respect the same targeting rules as normal offers. (#333)
- **[Bug]** **Some saved offer settings don't reach the live experience** — Several offer options you can set today (including Modal-tab fields and a few backend flags) quietly never make it to what visitors actually see. This work makes each option either fully take effect or be removed so nothing is misleading. (#295)
- **[Feature]** **Preview your unsaved changes on placements and offers** — Today the Preview button shows the last saved version, so you have to save before you can see a change. Soon Preview will reflect your current edits without saving first. (#292)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool that estimates a new offer's likely performance based on your historical offer data, replacing an informal manual review. It would give you a data-grounded gut-check at intake. (#322)

## Admin / Users

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record for editing, others will see it's locked and by whom, and saves will be checked so one person can't silently overwrite another's changes. Applies across all the entity edit screens. (#267)
- **[Feature]** **Remove settings that don't do anything** — Several admin controls (Advertiser Web Presence fields, some user-permission toggles, and a few Data Client and Pre-Ping options) are saved but never actually used. Hiding or removing them prevents confusion about settings that have no effect. (#296)
- **[Task]** **Finish bringing the Users screen up to parity** — A review comparing the old Users area to the new one, so missing capabilities (like bulk role changes and login/2FA details) can be prioritized. Behind-the-scenes analysis to guide upcoming work. (#80)
- **[Task]** **Decide the future of the File Share page** — The old file-share page has no equivalent yet. This is a keep-or-retire decision so it's either rebuilt or intentionally dropped. (#328)

## Surveys & Modals

- **[Feature]** **Make sure every design option actually applies** — A full review across all screens to confirm that every customization option on a form truly shows up in what visitors see, with any dead options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A handful of Placement Design-tab settings (like survey height and display format) don't yet affect the live survey. This wires them through so they take effect, or removes any that aren't needed. (#293)
- **[Feature]** **Wire up or remove the Modal Design tab** — The entire Modal Design tab currently has no effect on the visitor modal. This work either makes those header and progress-bar settings work or removes the tab if it isn't needed. (#294)

## Data Clients

- **[Feature]** **Restore file-based pre-ping validation** — Custom pre-ping checks used by 448 data clients aren't running on the new platform, so their validation silently doesn't happen. This high-priority work restores those checks at serve time. (#338)
- **[Feature]** **Restore post-success delivery for clients** — The old "after success" delivery/redirect behavior for clients like bperx and rwdb wasn't carried over. This ports all three behaviors so post-conversion delivery works again. (#327)

## Reports & Dashboard

- **[Task]** **Confirm report numbers match the legacy system** — During testing, some dashboard report figures didn't match the old system. This investigation pins down where the difference comes from and either fixes it or confirms the numbers are correct. (#271)

## General / Across the App

- **[Feature]** **Searchable history of who changed what** — A new admin Audit Log that records every change to records — manual or automated — with who made it and when, plus a per-record history view. Makes troubleshooting "who changed this and when" easy. (#276)
- **[Bug]** **Testing an invalid link now shows a clear error** — Entering an invalid link during link testing currently drops you on the dashboard with no explanation. This fix shows a proper error result instead. (#239)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or stack awkwardly compared to other forms. This cleans up spacing, text boxes, color pickers, and side-by-side fields so the form looks consistent. (#152)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only testing environment** — A staging copy of the app running against realistic data, locked to read-only so testing can happen safely without changing anything live. (#270)
- **[Feature]** **Turn conversations into tracked tasks automatically** — An internal helper that reads designated Slack conversations and files the action items as tracked issues, reducing manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
