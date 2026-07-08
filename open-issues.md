# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 20:29:06 UTC · 23 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else already has a record open, you'll see a clear "locked by…" notice and be warned before saving, so simultaneous edits can no longer quietly wipe out one person's changes. (#267)
- **[Feature]** **Remove settings that don't actually do anything** — Several controls that look active but have no effect (such as the Advertiser Web Presence fields, some user permission toggles, and a few Data Client and Pre-Ping options) will be hidden or removed so the screens only show settings that truly work. (#296)
- **[Feature]** **A searchable history of who changed what** — Administrators will get an Audit Log that records every change to offers, placements, and other records — including automated changes — with the person, the time, and what changed, making it easy to answer "who edited this and when." (#276)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will show a proper error message instead of unexpectedly sending you back to the Dashboard. (#239)
- **[Task]** **Decide the future of the old file-share page** — A review to confirm whether the legacy file-sharing page is still needed in the new platform or can be retired. (#328)

## Offers
- **[Feature]** **Preview your unsaved changes** — The Preview button on Offers and Placements will show the edits you've just made, so you can check how a change looks before saving. (#292)
- **[Bug]** **Make all saved offer settings take effect** — Some offer options (including Modal-tab fields and a few delivery settings) are saved but never reach what visitors actually see; this will ensure your saved choices are honored or clearly removed if unused. (#295)
- **[Feature]** **Automatic performance estimate for new offers** — Instead of relying on a manual gut-check, new offers could be scored against your historical offer data to project how they're likely to perform. This is exploratory work with no set deadline. (#322)
- **[Task]** **Apply visitor targeting to auto-register offers** — A high-priority fix so auto-registered offers respect age, gender, state, zip, and device targeting like other offers, instead of firing for visitors they should exclude. (#333)

## Surveys
- **[Feature]** **Design settings that reliably match the live survey** — A full review to make sure every option on the Design tab actually changes what visitors see, with any unconnected options fixed or removed across all entities. (#288)
- **[Bug]** **Make the survey Design tab settings actually work** — Today most of the ~30 styling and behavior settings (colors, buttons, header, legal text, and more) are saved but have no effect; this connects them so your customizations appear in the live survey. (#290)
- **[Feature]** **Finish connecting the remaining survey Design settings** — A follow-up to wire up the last few Design-tab options (like survey height and question display format) or remove them if they aren't needed. (#293)

## Pre-Pings
- **[Feature]** **Run the display pre-ping check when offers are shown** — A high-priority fix so offers using the "display" pre-ping actually verify with the advertiser at serve time and hide when rejected, matching the legacy system. (#337)
- **[Feature]** **Bring the legacy custom pre-ping checks to the new platform** — Restores the per-client validation used by hundreds of data clients so their custom serve-time checks run again instead of silently doing nothing. (#338)

## Reports & Dashboard
- **[Task]** **Track down why report numbers don't match the old system** — An investigation to compare the new platform's report figures against the legacy app over a fixed date range and explain any differences, so you can trust the numbers. (#271)
- **[Feature]** **Fix offer impressions showing as zero in historical placement reports** — Historical placement reports will show real offer-impression counts instead of zeros, an improvement over the legacy behavior. (#339)

## Data Clients
- **[Feature]** **Restore post-conversion delivery scripts** — The legacy "after success" delivery and redirect behaviors used by active data clients will be brought over to the new platform so post-conversion handling works as before. (#327)

## Flows
- **[Task]** **Tidy up the look of the Flow form** — Styling fixes so the Flow form's text boxes, color pickers, checkboxes, and paired fields display cleanly and consistently instead of appearing plain or misaligned. (#152)

## Modals
- **[Feature]** **Make the Modal Design tab work — or remove it** — Right now the entire Modal Design tab (header text, colors, progress bar) is saved but has no effect on the visitor modal; this will either connect those settings or remove the tab. (#294)

## Campaigns
- **[Feature]** **Bring Campaigns into the new platform** — The Campaigns module from the legacy admin isn't available yet; this adds the ability to view, create, edit, and configure campaigns and their offer groups, matching the old workflow. A core, high-priority gap. (#200)

## Users
- **[Task]** **Compare the old and new Users screens** — A documentation review identifying which Users features from the legacy system still need to be added to the new platform (such as bulk actions and last-login details), to guide upcoming work. (#80)

## Behind the Scenes
- **[Task]** **Set up a read-only test environment** — Deploying the app against a copy of production data for safe testing and verification, with no ability to change live data. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — An internal helper that reads designated Slack channels and automatically files or updates issues, so action items from meetings aren't lost. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 767867793bb373f1048c3d378d806ae5492206e4d988e86f295446991f13d4bc -->
