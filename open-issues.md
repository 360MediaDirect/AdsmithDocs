# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 00:23:14 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on placements and offers** — When editing a placement or offer, the Preview button will show your current in-progress edits, so you can check your work before saving. (#292)
- **[Bug]** **Some saved offer options never reach the live experience** — Several offer settings (including modal fields, Display URL, and certain data-client options) are saved but don't currently affect what visitors see; this fix ensures each setting either takes effect or is cleaned up. (#295)
- **[Bug]** **Success pixels aren't firing** — Conversion tracking pixels set on an offer's success step currently never fire, meaning lost tracking. This fix makes configured pixels reliably fire so attribution is captured. (#297)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, new offers could get a data-driven estimate of likely performance based on your historical offer data, giving a helpful starting read at intake. (#322)
- **[Bug]** **Auto-register offers are ignoring visitor targeting** — Auto-register offers currently fire for everyone, even visitors who should be excluded by age, gender, state, ZIP, or device. This ensures those offers respect the same targeting rules as regular offers. (High priority.) (#333)

## General / Across the App

- **[Bug]** **Invalid link tests should show a clear error** — Testing a bad link currently dumps you on the dashboard with no explanation; you'll instead see a clear error message telling you the link failed. (#239)
- **[Feature]** **Protection against two people editing the same record** — When someone else is already editing a record, you'll see who has it open and be prevented from accidentally overwriting their changes, with a prompt to reload if something changed while you had it open. (#267)
- **[Feature]** **Searchable history of who changed what** — A new Audit Log will record every change across the platform — by both people and automated processes — with timestamps, so administrators can search "who changed this and when" and view a history on each record. (#276)
- **[Feature]** **Clean up controls that don't actually do anything** — Certain settings (Advertiser Web Presence fields, some user permission toggles, and a few Data-Client and Pre-Ping options) are shown but currently have no effect. They'll be removed or hidden so the screens only show controls that work. (#296)
- **[Task]** **Decide the future of the legacy file-share page** — The old file-share page has no equivalent yet; this reviews whether anyone still needs it before keeping or retiring it. (#328)

## Surveys

- **[Feature]** **Make sure every survey design setting actually shows up** — A full review to confirm each design-tab customization option is reflected in the live survey, so nothing you configure is silently ignored. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A handful of placement design options (like survey height and display format) aren't yet reflected in the live survey; each will either be wired up or removed so the form only offers settings that work. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior for clients** — Certain after-success delivery and redirect behaviors from the old system weren't carried over; this brings them back for the clients that still rely on them. (#327)
- **[Feature]** **Restore custom pre-ping validation for data clients** — Hundreds of data clients relied on custom checks that ran before a lead was served in the old system and don't currently run. This ports that logic so those clients' validation works again. (High priority.) (#338)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging environment that mirrors real data for verification, with safeguards so no live data can be changed during testing. (#270)
- **[Feature]** **Automatic issue-filing from team chat** — A tool that turns action items from team conversations into tracked tasks automatically, reducing manual copy-and-paste. (#272)

## Reports

- **[Task]** **Confirm report numbers match the old system** — Investigating why some dashboard report figures differed from the legacy system during testing, so you can trust the numbers you see. (#271)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or awkwardly stacked. This tidies up the layout so it matches the polished look of other forms. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The Modal Design tab's settings currently don't affect the visitor-facing modal. Each field will either be made to work or removed so the tab isn't misleading. (#294)

## Campaigns

- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — The Campaigns feature from the old admin isn't available yet. This adds it back so you can create, edit, and manage campaigns and offer groups. (Critical, high priority.) (#200)

## Users

- **[Task]** **Compare the new Users area to the old one** — A review of the Users screens against the legacy system to spot missing capabilities (like bulk actions and login/2FA details) and prioritize what to add. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
