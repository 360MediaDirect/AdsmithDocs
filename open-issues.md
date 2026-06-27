# Open Issues — Plain-Language Overview

_Last updated 2026-06-27 10:39:12 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Behind the Scenes

- **[Task]** **Review whether an old stats job is still needed** — Behind-the-scenes maintenance to confirm an older reporting routine can be retired or merged, with no change to what you see. (#33)
- **[Feature]** **Faster "today" numbers** — Work on the system that powers up-to-the-hour figures (impressions, clicks, leads, revenue) so "today" views stay current and accurate. (#34)
- **[Feature]** **Reliable historical reporting totals** — Behind-the-scenes work that rolls up daily numbers so longer-term reports stay correct and consistent. (#35)
- **[Task]** **Safe testing of the new lead pre-check** — The new pre-ping process will run quietly alongside the existing one to confirm it produces the same results before it takes over. (#40)
- **[Feature]** **Per-advertiser pre-check validation** — Each advertiser's pre-ping setup will be verified ahead of the switchover so leads are handled correctly. (#41)
- **[Task]** **Speed boost for the Survey Engine** — A new caching layer will make surveys and offer checks respond faster. High priority. (#42)
- **[Task]** **Deploy new scheduled jobs in parallel** — The new background jobs will run side-by-side with the old ones and be monitored before any switch. (#43)
- **[Task]** **Gradual switch of survey-stats jobs** — Carefully retiring an older hourly survey-stats routine after the replacement proves stable. (#44)
- **[Task]** **Gradual switch of stats and reporting jobs** — Retiring several older stats and reporting routines once the replacements are confirmed reliable. (#45)
- **[Task]** **Gradual switch of critical jobs** — The most important background jobs (lead processing, offer-cap reset) will be switched over last, with close monitoring and instant rollback ready. (#46)
- **[Task]** **Document how to undo a change safely** — Clear rollback steps for each major system so the team can recover quickly if anything goes wrong. (#48)
- **[Task]** **Troubleshooting guides for the support team** — Step-by-step guides for resolving common issues, helping the team respond faster. (#49)

## Dashboard

- **[Task]** **Restore the missing Dashboard sections** — Campaign stats, top offers, and watch lists will return to the Dashboard, and the date-range selection will update them. High priority. (#240)
- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open a date picker so you can view Dashboard data for any start and end date instead of only the preset ranges. (#58)
- **[Feature]** **New "Other Dashboard" views plus an activity log** — You'll get views for offers with sustained performance and for CLP offer performance (flagging anything converting under 30%), plus a searchable record of changes like pausing offers or editing caps. (#256)
- **[Feature]** **Light mode option** — A toggle will let you switch between dark and light themes, with your choice remembered between sessions. (#59)
- **[Task]** **Cleaner, consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for better readability. (#263)

## Flows

- **[Feature]** **Clearer "Step order" setting** — The Step order field will get a plain-language label and inline help that explains what it controls, so it's no longer confusing. (#226)
- **[Task]** **Fix the Flow form's appearance** — Several parts of the Flow form (text boxes, color pickers, checkboxes, paired fields) will be properly styled and laid out to match the Placement and Modal forms. (#152)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other** — When someone is already editing a record, you'll see who has it open, and the system will warn you before a save could undo someone else's changes. This protection will apply across all editable screens. (#267)
- **[Task]** **Stronger brand guidelines for AI output** — A complete brand-guidelines document will be used as the main input for AI-generated content, improving the quality and consistency of results. (#264)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — A Campaigns area will be added so you can create, edit, and manage campaigns and offer groups just like in the legacy system. This is a core feature that's currently missing. High priority. (#200)

## Placements

- **[Feature]** **Easier offer management on Placements** — Selected offers will default to manual order with drag-and-drop reordering, a clear "X" to remove an offer, and the ability to filter the offer list by taxonomy. (#235)

## Pre-Pings

- **[Feature]** **Catch missing required fields before sending** — When a pre-ping runs before pushing data, leads missing required fields will be stopped up front rather than relying on the advertiser's response, preventing incomplete leads from slipping through. (#218)

## Users

- **[Task]** **Review of the Users area against the old system** — A documentation review comparing the new Users screens to the legacy version to identify gaps and prioritize what to add next. (#80)

## Link Testing

- **[Bug]** **Show a clear error for invalid links** — Testing an invalid link will return a helpful error message instead of unexpectedly sending you to the Dashboard. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
