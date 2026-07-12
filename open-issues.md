# Open Issues — Plain-Language Overview

_Last updated 2026-07-12 15:21:41 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers & Campaigns
- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — Campaign management isn't available yet in the new platform. Once added, you'll be able to view, create, edit, and configure campaigns — including offer groups, questions, CTA text, and offer handling — just like the legacy system. This is high priority. (#200)
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers are currently saved but never actually fire, meaning successful conversions can go unrecorded. The fix ensures your configured success pixels fire as expected. This is high priority. (#297)
- **[Task]** **Auto-register offers ignore visitor targeting** — Auto-register offers are currently shown to everyone, even when age, gender, state, zip, or device targeting should exclude them. This work makes sure those offers respect the same targeting rules as regular offers. This is high priority. (#333)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several offer options you can fill in today (like Display URL and certain modal and data-handling settings) don't actually carry through to what visitors see. This cleans that up so every option either works or is removed from the form. (#295)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — Today the Preview button shows the last saved version, so you have to save before you can see edits. This update lets Preview reflect your current in-progress changes without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, replacing a manual gut-check review. It would give you a data-grounded projection at intake. (#322)

## General / Across the App
- **[Feature]** **Warn when two people edit the same record** — If a teammate is editing a record you have open, you'll see a clear "locked by" notice and be prevented from accidentally overwriting each other's changes. This protects your work across all entity screens. (#267)
- **[Feature]** **Searchable activity/audit log** — A new admin log that records every change to records — who changed what and when, including automated changes — so you can easily track history and troubleshoot. Each entity screen will also show its own change history. (#276)
- **[Feature]** **Clean up controls that don't do anything** — Several settings across Advertisers (Web Presence), Users (permissions), Data Clients, and Pre-Pings currently save but have no effect. These will be removed or hidden so the app only shows controls that actually work. (#296)
- **[Task]** **Users screen review against the legacy system** — A documentation review comparing the new Users management screen with the legacy version to identify missing pieces (like bulk actions, last-login, and two-factor status). This guides upcoming improvements to the Users area. (#80)
- **[Bug]** **Invalid link tests send you to the Dashboard** — When you test a link that isn't valid, you're currently dropped on the Dashboard instead of seeing an error. The fix shows a clear failure message in the Link Testing screen. (#239)
- **[Task]** **Decide the future of the legacy file-share page** — The old file-share page has no equivalent in the new platform. This is a decision on whether to rebuild it or retire it, based on whether anyone still uses it. (#328)

## Surveys
- **[Feature]** **Make sure every Design tab setting actually changes the survey** — A thorough check across all entity forms to confirm each Design/customization option truly affects what visitors see, fixing or removing any that don't. Your survey customizations will reliably show up. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live survey** — A handful of Placement design options (like survey height and display format) are saved but don't yet affect the survey widget. This wires them through or removes any that aren't needed. (#293)

## Data Clients & Pre-Pings
- **[Feature]** **Restore after-success delivery for data clients** — Post-conversion delivery and redirect behavior from the legacy system hasn't been carried over yet. This brings it back as a configurable option so conversions are handled correctly for the clients that rely on it. (#327)
- **[Feature]** **Restore custom pre-ping validation for data clients** — Custom serve-time validation used by hundreds of data clients in the legacy system isn't running on the new platform. This ports that logic so those checks apply as intended. This is high priority. (#338)

## Modals
- **[Feature]** **Make the Modal Design tab work — or remove it** — Every field on the Modal Design tab currently saves but has no effect on what visitors see. This either wires the header and progress-bar settings through to the visitor modal or removes the tab if it isn't needed. (#294)

## Flows
- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned — plain text boxes, unstyled color pickers, and fields that stack instead of sitting side by side. This tidies the form so it matches the polished look of the Placement and Modal forms. (#152)

## Dashboard
- **[Task]** **Confirm Dashboard report numbers match the legacy system** — During testing, some Dashboard report figures didn't line up with the legacy app. This investigation compares the two over a fixed date range to find and explain any differences and confirm the numbers can be trusted. (#271)

## Behind the Scenes
- **[Task]** **Set up a safe, read-only test environment** — A staging setup using production-like data for verification and testing, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Automatically turn team conversations into tracked tasks** — An internal helper that reads designated Slack channels and files action items as tracked issues automatically, reducing manual copy-paste work. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
