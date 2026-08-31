# Open Issues — Plain-Language Overview

_Last updated 2026-08-31 06:08:16 UTC · 15 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Missing offer options now carry through to what visitors see** — Several offer settings you fill in today (like the Modal-tab fields, Display URL, and certain delivery flags) weren't actually reaching the live offer. This fix makes sure the options you save show up where they should, or removes ones that do nothing so the form only shows settings that matter. (#295)
- **[Bug]** **Manually selected offers now appear correctly** — On placements set to manual offer delivery, your hand-picked offer list was coming through empty in New Adsmith Frontend, causing the wrong offers to show. This restores your selected offers and their order so the live result matches what you configured. (#370)
- **[Feature]** **Preview your unsaved offer and placement edits** — The Preview button will show the changes you're currently making, even before you save, so you can check your work without having to save first. (#292)
- **[Feature]** **Automatic performance estimates for new offers** — Instead of a manual gut-check, New Adsmith Frontend will estimate how a new offer is likely to perform based on your historical offer data, giving you a data-backed projection at intake. (#322)

## Admin & Users

- **[Task]** **Bringing the Users area up to full parity** — A review compared the older Users management to the new one and found missing pieces (like bulk role changes, selecting multiple users at once, last-login and two-factor details, and a password field when adding a user). This tracks closing those gaps so the Users area feels complete. (#80)
- **[Feature]** **Removing admin controls that don't do anything** — Some settings in the Admin area (certain user permission toggles and a few data-client and pre-ping options) look active but have no effect. They'll be hidden or removed so you're not misled into thinking they change something. (#296)

## Data Clients & Pre-Pings

- **[Feature]** **Post-conversion delivery steps restored** — Certain after-success behaviors from the older system that run once a lead converts weren't carried over. This brings them back for the clients that rely on them. (#327)
- **[Feature]** **Custom pre-ping validation restored for data clients** — Hundreds of data clients relied on custom checks that ran before serving and weren't yet active in New Adsmith Frontend. This high-priority work makes those checks run again so leads are validated the way they used to be. (#338)

## Dashboard & Reports

- **[Task]** **Confirming dashboard report numbers are accurate** — Some dashboard figures didn't match the older system during testing. This high-priority investigation pins down why and makes sure the numbers you see are trustworthy. (#271)
- **[Feature]** **Add and view notes on Placement, Advertiser, and Offer dashboards** — You'll be able to attach short, categorized notes (with a topic and priority) to a placement, advertiser, or offer, and see a recent-notes roll-up on the main Dashboard — with new notes appearing instantly without reloading the page. (#382)

## Surveys

- **[Feature]** **Design-tab choices reliably show up in the survey** — Every customization you set on the design tab will be reflected in the actual survey view, and a full check across all entity forms ensures no setting is left disconnected. (#288)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned compared to other forms — text boxes, color pickers, checkboxes, and paired fields that should sit side by side. This clean-up brings the Flow form's look in line with the rest of the app. (#152)

## Publishers & Properties

- **[Bug]** **Pausing a publisher or property works consistently** — A pause could be ignored on one of the serving paths, meaning a paused publisher or property might still serve. This fix makes the pause take effect everywhere it should. (#299)

## Behind the Scenes

- **[Feature]** **Automatically turning conversations into tracked work** — A helper that reads designated chat conversations and files the resulting to-dos as tracked issues, cutting out manual copy-paste. No direct effect on the product screens. (#272)
- **[Task]** **Strengthening automated testing** — A review of the app's automated tests found gaps (some tests weren't truly running, and the suite wasn't running consistently). Addressing these makes future releases more reliable. No user-facing change. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
