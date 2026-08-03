# Open Issues — Plain-Language Overview

_Last updated 2026-08-03 07:03:19 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Manually selected offers aren't carrying over from the old system** — On Manual-delivery placements, the list of hand-picked offers is coming across empty, so the new platform shows different offers than the old one. This fix makes sure your selected offers (and their order) appear and display correctly. (#370)
- **[Bug]** **Some offer settings never reach the live offer** — A handful of options you can set on an offer weren't actually being applied when the offer went live. This ensures the settings you save take effect (or are cleaned up if they were never meant to do anything). (#295)
- **[Bug]** **Can't set a survey to Display or AR on an offer** — The Display and AR controls on the Offer Details Delivery tab are missing their selectable buttons, so you can't choose a mode. This restores those controls so you can assign delivery modes without going back to the old app. (#371)
- **[Bug]** **Offer edits aren't showing up in History** — Editing and saving an offer succeeds, but the change isn't being recorded in the offer's History section. This fix makes sure your edits are logged so there's a clear record of who changed what. (#380)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — Right now the Preview button shows the last saved version, so you have to save before you can see edits. This lets Preview reflect your current, unsaved changes. (#292)
- **[Feature]** **Automatic performance estimate for new offers** — Instead of relying on a manual gut-check, new offers could get an automated projection of how they're likely to perform, based on your own historical offer data. An exploratory decision aid to help at offer intake. (#322)

## General / Across the App

- **[Task]** **Review of the Users area against the old system** — A thorough comparison of the old and new Users management screens to spot missing pieces (like bulk actions, last-login info, and 2FA status) so nothing important gets left behind. (#80)
- **[Feature]** **Clean up admin controls that don't do anything** — Several settings (such as the Advertiser Web Presence fields, certain user-permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no effect. These will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Bug]** **Pausing a publisher or property isn't always enforced** — In one part of the system, a paused publisher or property could still slip through. This fix makes the pause reliable so paused really means paused everywhere. (#299)

## Data Clients

- **[Feature]** **Bring back after-conversion delivery steps** — Certain post-conversion delivery and redirect behaviors from the old system haven't been carried over yet. This ports them so those clients keep working as before. (#327)
- **[Feature]** **Restore serve-time validation checks for data clients** — Hundreds of data clients rely on custom checks that run when an ad is served, and those aren't running on the new platform yet. This high-priority work re-creates them so validation happens as expected. (#338)

## Surveys

- **[Feature]** **Make design customizations actually show up** — Ensures every option on the survey Design tab is reflected in what visitors see, and reviews all entity forms so there are no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting placement design settings to the live widget** — Options like survey height and display format are being saved but not yet applied. This wires them through (or removes any that aren't needed) so your placement design choices take effect. (#293)

## Behind the Scenes

- **[Feature]** **A Slack helper that turns conversations into tracked tasks** — A tool that reads designated Slack channels, spots action items, and files them as tracked work automatically — saving the manual step of copying notes into task lists. (#272)
- **[Task]** **Strengthening our automated testing** — Behind-the-scenes improvements to the automated checks that catch problems before they reach you, making test results more reliable. (#379)

## Dashboard

- **[Task]** **Investigating report numbers that don't match the old system** — Dashboard report figures didn't line up with the legacy app during testing. This work compares the two over a fixed period to find where the difference comes from and confirm the numbers are trustworthy. (#271)

## Flows

- **[Task]** **Fix the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other screens — text boxes, color pickers, and paired fields don't display cleanly. This tidies up the layout so the form looks consistent and polished. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design tab's header and progress-bar settings are saved but don't currently affect what visitors see. This will either make those settings actually appear on the modal or remove them so the tab isn't misleading. (#294)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
