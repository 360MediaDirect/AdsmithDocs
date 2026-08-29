# Open Issues — Plain-Language Overview

_Last updated 2026-08-29 06:05:41 UTC · 15 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Bug]** **Manually selected offers now carry over correctly** — On placements set to manual offer delivery, the new platform was showing the wrong or empty offer list because the hand-picked offers (and their order) weren't being brought over. Once fixed, these placements will display the same offers, in the same order, as before. (#370)
- **[Bug]** **Saved offer settings will actually reach the live experience** — Several options you can set on an offer (including the Modal-tab fields, Display URL, Force More Info visibility, and certain data-client settings) currently save but never take effect. This work makes sure each saved option is either used or cleaned up so nothing is misleading. (#295)
- **[Feature]** **Preview offers and placements with your unsaved changes** — The Preview button will show your in-progress edits instead of only the last saved version, so you can check how a change looks before committing to it. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, replacing the informal manual gut-check with a data-driven projection at intake. (#322)

## Dashboard & Reports
- **[Task]** **Confirming dashboard report numbers match the old system** — High-priority investigation into why some dashboard report figures didn't line up with the legacy app, so you can trust that the numbers are accurate and consistent. (#271)
- **[Feature]** **Notes on Placements, Advertisers, and Offers** — Bringing back the ability to attach short, categorized notes (with topic and priority) directly to a Placement, Advertiser, or Offer, plus a recent-notes roll-up on the main Dashboard. New notes will appear right away without needing to reload the page. (#382)

## Admin / Users
- **[Task]** **Closing gaps between the old and new Users area** — An ongoing review of the Users screens to bring back missing capabilities from the legacy app, such as bulk actions, role changes for multiple users at once, and additional user details. (#80)
- **[Feature]** **Removing admin controls that don't do anything** — Some settings (certain user permission toggles and a few Data-Client and Pre-Ping options) currently save but have no effect. Hiding or removing them prevents confusion about access and behavior that isn't really there. (#296)

## Data Clients & Pre-Pings
- **[Feature]** **Restoring post-conversion delivery behaviors** — The legacy "after-success" delivery and redirect steps that run once a lead converts are being brought over to the new platform, so affected data clients keep working as they did before. (#327)
- **[Feature]** **Restoring custom pre-ping validation for data clients** — High-priority work to bring over legacy per-client validation checks that run before serving, which currently don't run on the new platform. This ensures leads are validated consistently for the hundreds of data clients that rely on it. (#338)

## Behind the Scenes
- **[Feature]** **Turning Slack conversations into tracked tasks automatically** — A helper that reads designated Slack channels and files action items as tracked issues, reducing manual copy-and-paste when capturing follow-ups. (#272)
- **[Task]** **Strengthening our automated testing** — Fixing gaps in the automated checks that verify the app works, so problems are caught reliably before they reach you rather than being missed. (#379)

## Flows
- **[Task]** **Tidying up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned, with fields stacking vertically instead of sitting side by side. This work brings its look in line with the Placement and Modal forms. (#152)

## Surveys
- **[Feature]** **Making sure every design option actually shows up in the survey** — A review to confirm that each customization you set on the design tab is reflected in the live survey view, with any unused options fixed or removed. (#288)

## Publishers & Properties
- **[Bug]** **Pausing a publisher or property will fully take effect** — A pause on a publisher or property wasn't being enforced everywhere, so serving could continue on one path. This fix makes pausing reliable and consistent. (#299)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
