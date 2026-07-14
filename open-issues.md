# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 07:34:16 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Protect records from being overwritten by two editors at once** — When you open a record that someone else is already editing, you'll see a clear "locked by…" banner, and if a record changes while you have it open, you'll be prompted to reload instead of accidentally wiping out the other person's work. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will let administrators see who changed what and when — across offers, placements, advertisers, modals, flows, and more — including automated changes, making it easy to answer "who edited this?" (#276)
- **[Feature]** **Clean up controls that don't actually do anything** — Several fields that currently save but have no effect (Advertiser Web Presence links, certain user permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden so the screens only show settings that truly work. (#296)
- **[Bug]** **Clearer result when testing an invalid link** — Instead of being bounced to the Dashboard, you'll get a clear error message when a tested link is invalid. (#239)
- **[Task]** **Users screen comparison with the old system** — A review of the old Users area versus the new one, so any missing options (like bulk role changes or last-login info) can be planned and added. (#80)
- **[Task]** **Decide the future of the old File Share page** — A quick review to confirm whether the legacy file-sharing page is still needed or can be retired. (#328)

## Offers
- **[Bug]** **Success tracking pixels will actually fire** — A high-priority fix so the conversion pixels you set up on an offer reliably fire on success, restoring accurate tracking and attribution. (#297)
- **[Bug]** **Saved offer settings will reach the live experience** — Several offer options you configure (including Modal-tab settings and Display URL) currently get lost before reaching visitors; this ensures they're either applied or clearly marked as not needed. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — A high-priority fix so auto-registered offers honor age, gender, state, zip, and device targeting the same way regular offers do, instead of firing for visitors they should skip. (#333)
- **[Feature]** **Preview offers and placements with your unsaved changes** — The Preview button will show the edits you're currently making, so you no longer have to save first just to see how a change looks. (#292)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical offer data, replacing the old manual gut-check review. (#322)

## Surveys
- **[Feature]** **Make sure Design tab choices show up in the survey** — Every customization on the Design tab will be reflected in the live survey, with a full check across entities to remove any settings that don't actually do anything. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey** — Remaining Placement design options (like survey height and display format) will be properly applied in the live survey, with unused options either wired up or removed. (#293)

## Data Clients & Pre-Pings
- **[Feature]** **Restore high-priority pre-serve checks for data clients** — The custom validation checks that ran for hundreds of data clients in the old system will be brought over so they run again, preventing bad or unqualified traffic from slipping through. (#338)
- **[Feature]** **Bring back post-conversion delivery steps** — The old "after success" delivery and redirect behavior for certain clients will be ported so those clients keep working as before. (#327)

## Behind the Scenes
- **[Task]** **Set up a safe testing environment** — A read-only staging setup using production-like data, so the product can be verified against realistic data without any risk of changing it. (#270)
- **[Feature]** **Automatic issue capture from team chat** — An internal helper that turns action items from team conversations into tracked tasks, reducing manual note-taking. (#272)

## Flows
- **[Task]** **Fix visual styling on the Flow form** — Cleans up unstyled areas of the Flow form (text boxes, color pickers, checkboxes, and side-by-side fields) so it looks consistent with the Placement and Modal forms. (#152)

## Modals
- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The Modal Design tab's header and progress-bar settings currently have no effect; they'll either be applied to the visitor modal or removed to avoid confusion. (#294)

## Campaigns
- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — A high-priority addition so you can view, create, edit, and configure campaigns and offer groups directly in the new platform, matching what the old admin offered. (#200)

## Reports
- **[Task]** **Investigate mismatched Dashboard report numbers** — A review comparing report figures between the old and new systems to find and explain any differences, so you can trust the numbers you see. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
