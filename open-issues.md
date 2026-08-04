# Open Issues — Plain-Language Overview

_Last updated 2026-08-04 06:49:39 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach visitors** — Several options you set on an offer (including the Modal-tab fields, Display URL, and "Force More Info Visible") weren't being carried through to the live experience. Each one will be properly connected or removed from the form so what you see reflects what visitors get. (#295)
- **[Bug]** **Restore the Display / AR choices on the Delivery tab** — On an offer's Delivery tab, the DISP and AR columns show as headings but the buttons to actually assign a survey to Display or AR are missing. This fix brings those controls back so you can set a survey's delivery mode without going to the old app. (#371)
- **[Bug]** **Offer edits will show up in History** — Right now, editing an offer saves your change but doesn't add a "History" entry, so the record looks like nothing happened. Once fixed, every field change will be logged in the offer's History section. (#380)
- **[Feature]** **Automatic performance estimate for new offers** — Instead of a manual gut-check, a new offer will be scored against your historical offer data to project how it's likely to perform. A helpful decision aid at intake — this is exploratory and medium priority. (#322)

## Placements

- **[Bug]** **Manually selected offers now carry over correctly** — On Manual-delivery placements, the list of hand-picked offers wasn't being migrated, so the new app showed the wrong or empty offers. This fix ensures your selected offers — and their order — appear exactly as configured. (#370)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show your current, in-progress edits instead of only the last saved version, so you can check a change before committing it. (#292)
- **[Feature]** **Connect the remaining Placement Design settings** — A few Design-tab settings (such as iFrame height and display format) aren't yet reflected in what visitors see. Each will be wired through to the widget or removed if it isn't needed. (#293)

## Data Clients

- **[Feature]** **Post-conversion delivery steps brought to the new platform** — The "after success" delivery and redirect behaviors from the old system are being rebuilt as a reusable setting, so those client-specific hand-offs keep working. Nearly complete. (#327)
- **[Feature]** **Serve-time validation checks for data clients** — High priority: legacy per-client pre-ping validation checks weren't running on the new platform for hundreds of data clients. This work restores those checks so leads are validated and accepted or rejected as intended. (#338)

## Admin

- **[Task]** **Reviewing the Users area against the old app** — A side-by-side comparison of the legacy Users screens and the new ones, to spot missing capabilities (like bulk role changes, last-login, and 2FA status) so they can be planned and added. (#80)
- **[Feature]** **Hide controls that don't actually do anything** — Some admin settings (the Advertiser "Web Presence" tab, a couple of user-permission toggles, and a few data-client/pre-ping options) are shown but have no effect. They'll be removed or hidden so the interface only offers real, working controls. (#296)

## Surveys

- **[Feature]** **Design customizations will show up in the survey** — Every option on the Design tab will be checked to make sure it's actually reflected in the live survey, with a review across all entity screens to catch any setting that looks active but does nothing. (#288)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The six Design-tab fields for modals (header title, subtitle, colors, progress bar) currently don't appear to visitors. They'll either be connected so they display, or removed so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or misaligned — plain text boxes, unstyled color pickers, and paired fields stacking vertically instead of side by side. This cleanup brings the form in line with the Placement and Modal forms. (#152)

## Dashboard

- **[Task]** **Confirm dashboard report numbers are accurate** — During testing, some dashboard report figures didn't match the old system. This investigation compares the two over a fixed date range to find any differences and confirm the numbers can be trusted. (#271)

## Publishers

- **[Bug]** **Pausing a publisher or property will be fully enforced** — On one delivery path, a paused publisher or property wasn't actually being stopped. This fix makes pausing take effect consistently everywhere. (#299)

## Behind the Scenes

- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads designated chat channels and files the action items as tracked issues, cutting out manual copy-and-paste when capturing follow-ups. (#272)
- **[Task]** **Strengthen automated testing** — A review of the automated test suite found gaps (some tests silently skipping, tests not running automatically, and occasional flakiness). Addressing these makes future releases more reliable. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
