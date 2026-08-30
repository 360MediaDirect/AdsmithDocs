# Open Issues — Plain-Language Overview

_Last updated 2026-08-30 06:06:11 UTC · 15 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers & Placements

- **[Feature]** **Preview your unsaved changes before saving** — When editing a placement or offer, the Preview button will show exactly what you've changed on the page, so you no longer have to save first just to see how an edit looks. (#292)
- **[Bug]** **Offer settings that weren't reaching the live experience** — Several saved offer options (including the Modal-tab fields, Display URL, and "Force More Info Visible") weren't actually being applied on live surfaces. We're making sure each saved option either takes effect or is cleanly removed so nothing is misleading. (#295)
- **[Feature]** **Automatic performance projections for new offers** — Exploring a way to estimate how a new offer is likely to perform based on your own historical offer data, giving the team a data-driven gut-check at intake instead of relying on a manual review. (#322)
- **[Bug]** **Manually selected offers now show correctly** — On Manual-delivery placements, the specific offers you chose (and their order) weren't carried over, so the wrong or empty offers appeared. This fix ensures the new experience displays the same hand-picked offers as before. (#370)

## Reports & Dashboard

- **[Task]** **Making dashboard report numbers trustworthy** — Investigating why some dashboard report figures didn't match the previous system, so you can rely on the numbers you see. (#271)
- **[Feature]** **Notes on Placements, Advertisers, and Offers** — You'll be able to add short, categorized notes right from a Placement, Advertiser, or Offer's report page, with a recent-notes roll-up on the main Dashboard — matching the notes feature from the previous app, with the added convenience of seeing new notes appear without reloading. (#382)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery behavior** — Bringing over the "after-success" delivery and redirect steps from the previous system so data clients continue to behave correctly once a conversion completes. (#327)
- **[Feature]** **Restoring custom pre-ping validation** — Rebuilding the per–data-client validation checks that ran in the previous system so that these serve-time checks work again for the many clients that depend on them. This is high priority. (#338)

## Admin & Users

- **[Task]** **Closing the gaps in the Users area** — Comparing the new Users management screens against the previous system to identify and add missing capabilities like bulk role changes, last-login and two-factor status, and password/notification options when adding a user. (#80)
- **[Feature]** **Removing controls that don't do anything** — Cleaning up admin settings (certain user permission, Data-Client, and Pre-Ping options) that appear active but have no effect, so the interface doesn't imply behavior that isn't really there. (#296)

## Behind the Scenes

- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack discussions and automatically files the action items, reducing manual copy-paste when logging requests. (#272)
- **[Task]** **Strengthening our automated testing** — Improving the behind-the-scenes automated checks so they run reliably and catch problems earlier, which means fewer surprises reaching you. (#379)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Several parts of the Flow form (text boxes, color pickers, checkboxes, and side-by-side fields) currently appear unstyled or stacked awkwardly. This tidies up the form so it matches the polished look of the Placement and Modal forms. (#152)

## Surveys

- **[Feature]** **Design choices that actually show up in the survey** — Making sure every option on the design tab is reflected in the live survey view, plus a full check across all entities to confirm no setting is quietly ignored. (#288)

## Publishers & Properties

- **[Bug]** **Pausing a publisher or property now sticks** — A pause set on a publisher or property wasn't being enforced on one of the serving paths. This fix ensures paused items are consistently blocked everywhere. (#299)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
