# Open Issues — Plain-Language Overview

_Last updated 2026-08-23 06:06:58 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach the live offer** — Certain options you set on an offer (including all the Modal-tab settings, "Force More Info Visible", Display URL, and several delivery flags) currently save but never actually take effect when the offer is shown. This work makes sure each option either works or is cleaned up, so nothing on the form is misleading. (#295)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, New Adsmith Frontend will estimate how a new offer is likely to perform based on your own historical offer data, giving you a data-driven read right at intake. (#322)
- **[Bug]** **Manually selected offers now carry over correctly** — On Manual-delivery placements, the "Selected Offers" list was coming through empty, so the wrong offers were being displayed. This fix ensures your chosen offers, in the right order, match what you set. (#370)

## Placements

- **[Feature]** **Preview your unsaved edits on placements and offers** — The Preview button will show the changes you're currently making, so you no longer have to save first just to see how an edit will look. (#292)
- **[Feature]** **Placement Design settings now apply to the live survey** — Several Design-tab options (like iFrame height and display format) were being saved but not reflected for visitors. This finishes connecting them so your design choices actually show up. (#293)

## Data Clients

- **[Feature]** **Legacy pre-ping checks brought to the new platform** — Custom serve-time validation used by hundreds of data clients wasn't running yet on the new platform. This high-priority work restores it so the right leads are accepted or rejected as before. (#338)
- **[Feature]** **After-conversion delivery behaviors restored** — Post-conversion redirect and delivery steps that existed in the old app are being brought over, so affected clients keep working exactly as they did. (#327)

## Reports & Dashboard

- **[Task]** **Confirming report numbers match the old system** — Investigating why some Dashboard report figures didn't line up with the legacy app, so you can trust the numbers you see. (#271)
- **[Feature]** **Add and view notes on Placement, Advertiser, and Offer dashboards** — You'll be able to attach short, categorized notes to these records and see a recent-notes roll-up on the main Dashboard, just like the old app — with notes appearing right away instead of needing a page reload. (#382)

## Admin & Users

- **[Feature]** **Removing admin controls that don't do anything** — Some settings (the Advertiser Web Presence fields, certain user-permission toggles, and a few data-client and pre-ping options) currently save but have no real effect. They'll be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Closing the gap between the old and new Users area** — A review of which Users features from the legacy app are still missing (things like bulk role changes and last-login and 2FA columns), so the new Users area can catch up. This is an analysis and documentation step. (#80)

## Behind the Scenes

- **[Feature]** **Turning conversations into tracked tasks automatically** — Behind-the-scenes tooling to capture action items from team chats and file them as tracked work items, without manual copy-and-paste. (#272)
- **[Task]** **Making automated testing more reliable** — Behind-the-scenes maintenance to strengthen the app's automated checks so problems are caught earlier and more consistently. (#379)

## Surveys

- **[Feature]** **Design choices reliably flow into the survey** — A thorough check across all screens to make sure every design and customization option you set actually appears in the survey, with no "dead" options that do nothing. (#288)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The Modal Design tab's settings (header title, subtitle, colors, and progress bar) currently have no effect on what visitors see. This will either make them work or remove them so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned — plain text boxes, unstyled color pickers, and paired fields stacking on top of each other instead of sitting side by side. This brings its appearance in line with the rest of the app. (#152)

## Publishers & Properties

- **[Bug]** **Pausing a publisher or property now takes effect everywhere** — A pause wasn't being enforced on one of the serving paths, meaning paused publishers or properties could still serve. This makes pausing behave consistently. (#299)

## Advertisers

- **[Feature]** **Show website and social links on the Advertiser detail page** — The Web Presence details you enter (website, social profiles, and a handy "Search on Google" shortcut) will appear as icon links in the Advertiser detail header, opening safely in a new tab. (#383)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
