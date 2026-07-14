# Open Issues — Plain-Language Overview

_Last updated 2026-07-14 17:28:04 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes before you save** — On the placement and offer edit screens, the Preview will show the changes you're currently making rather than the last saved version, so you can check your work without saving first. (#292)
- **[Bug]** **Some saved offer settings never reach the live page** — Certain offer options you set (such as modal text and display URL) are saved but don't currently appear where visitors see them; this fix ensures configured settings actually take effect or are cleanly removed. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — A high-priority fix so the conversion pixels you set up on offers actually fire, restoring accurate attribution and revenue tracking that's currently being lost silently. (#297)
- **[Task]** **Auto-register offers now respect visitor targeting** — A high-priority fix so auto-register offers honor age, gender, state, zip, and device targeting, preventing them from firing for visitors who should be excluded. (#333)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, new offers could get a data-driven estimate of how they're likely to perform based on your historical offer data, helping you make faster intake decisions. (#322)

## General / Across the App

- **[Bug]** **Invalid link tests will show a clear error** — When you test a link that doesn't work, you'll get an obvious failure message instead of being unexpectedly sent to the dashboard. (#239)
- **[Feature]** **Protection against two people overwriting each other's edits** — When someone else is already editing a record, you'll see a clear "locked by" notice, and the system will warn you rather than silently discarding changes when two people edit the same item. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will be able to see who changed what and when across offers, placements, and other entities, with a searchable audit log and per-record history for easy troubleshooting. (#276)
- **[Feature]** **Clean up controls that don't actually do anything** — Several admin settings (some Advertiser web-presence fields, unused user permission toggles, and a few data-client and pre-ping options) currently look active but have no effect; these will be removed or hidden to avoid confusion. (#296)
- **[Task]** **Decide the future of the old file-share page** — A quick review to confirm whether the legacy file-share page is still needed and either rebuild it in the new admin or retire it intentionally. (#328)

## Surveys & Modals

- **[Feature]** **Design customizations will show up in the survey** — Every option on the design tab will be properly connected end-to-end, so what you set in the form is what visitors actually see, with a full check to remove any options that don't do anything. (#288)
- **[Feature]** **Finish connecting Placement design settings** — Remaining Placement design-tab settings (like survey height and display format) will be fully wired to the live widget, or removed if they aren't used. (#293)
- **[Feature]** **Fix the Modal design tab** — The Modal design tab's header and progress-bar settings currently save but don't appear anywhere; they'll either be shown in the visitor modal or removed from the form. (#294)

## Behind the Scenes

- **[Task]** **A safe, read-only staging environment for testing** — Sets up a testing environment using production-like data that can't be accidentally changed, making it easier to verify the product against real-world data. (#270)
- **[Task]** **Investigate report numbers that don't match the old system** — Looking into why some dashboard report totals differed from the legacy system, to pinpoint the cause and confirm the numbers you see are accurate. (#271)
- **[Feature]** **A Slack helper that turns conversations into tracked tasks** — A behind-the-scenes tool to automatically capture action items from Slack and file them as tracked issues, reducing manual note-taking. (#272)

## Data Clients & Pre-Pings

- **[Feature]** **Restore post-conversion delivery scripts** — The after-success delivery behavior from the old system will be rebuilt in the new platform so partner delivery and redirects continue working as before. (#327)
- **[Feature]** **Bring back custom pre-ping validation for data clients** — A high-priority effort to restore the custom serve-time validation many data clients relied on, so lead-quality checks run correctly on the new platform. (#338)

## Flows

- **[Task]** **Fix the look of the Flow form** — Cleans up styling on the Flow form so text boxes, color pickers, checkboxes, and paired fields display correctly and consistently with the other forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — A high-priority addition so you can view, create, edit, and configure campaigns and offer groups in New Adsmith Frontend, matching what the legacy admin offered. (#200)

## Users

- **[Task]** **Compare the old and new Users areas** — A review of the legacy Users module against the new one to identify missing capabilities (like bulk actions and login/2FA details) and prioritize what to add next. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
