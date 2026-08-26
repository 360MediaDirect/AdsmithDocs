# Open Issues — Plain-Language Overview

_Last updated 2026-08-26 06:08:48 UTC · 17 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach live ads** — Several options you fill in on an offer (including its Modal-tab fields, "Force More Info Visible," Display URL, and certain data-client flags) currently get dropped before the ad is shown, so they have no effect. This fix ensures each of those settings either works as expected or is cleared out if it's not needed. (#295)
- **[Bug]** **Manually selected offers now carry over from the old system** — For placements set to deliver a hand-picked offer list, the new platform was showing the wrong or no offers because the selected list wasn't being brought over. This fix restores your chosen offers in the right order so old and new match. (#370)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — The Preview button will show exactly what you're editing right now, instead of only the last saved version, so you won't have to save first just to check how a change looks. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature that would estimate how a new offer is likely to perform, based on your own historical offer data, replacing the informal manual gut-check review. (#322)

## Data Clients & Pre-Pings

- **[Feature]** **Post-conversion delivery steps brought into the new platform** — Certain "after success" behaviors that ran for some clients in the old system weren't available in New Adsmith Frontend. This work ports them over as a reusable, configurable option so those clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-checks for data clients** — Hundreds of data clients relied on custom validation that ran before a lead was served in the old system and currently doesn't run at all. This high-priority work re-establishes those checks so leads are validated consistently. (#338)

## Dashboard & Reports

- **[Task]** **Confirm report numbers match the old system** — A high-priority investigation into why some Dashboard report figures didn't line up with the legacy app, so you can trust that the numbers you see are accurate and consistent. (#271)
- **[Feature]** **Notes on Placements, Advertisers, and Offers** — You'll be able to add short, categorized notes (with a topic and priority) directly on a Placement, Advertiser, or Offer's report page, and see a recent-notes roll-up on the main Dashboard. New notes will appear right away without reloading the page. (#382)

## Surveys

- **[Feature]** **Design settings that actually change the survey** — A thorough check to make sure every option on the Design tab truly affects what visitors see in the survey, across all entity screens, with any unused options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design options to the live survey** — A few Placement Design-tab settings (such as survey height and display format) don't yet affect the live survey. This work wires the remaining options through, or removes any that aren't needed, so the form reflects reality. (#293)

## Users & Admin

- **[Task]** **Review of the Users area against the old system** — A comparison of the new Users screens with the legacy version to spot any missing capabilities (like bulk role changes and login details) and plan what to add next. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings across Advertisers (Web Presence), user permissions, Data Clients, and Pre-Pings currently save but have no effect. These will be hidden or removed so the admin screens only show controls that actually work. (#296)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned (plain text boxes, unstyled color pickers, fields that stack instead of sitting side by side). This work polishes the form so it matches the cleaner styling used elsewhere. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — The Modal Design tab's settings (header title, colors, progress bar, etc.) currently have no effect on what visitors see. This work either connects them so they display, or removes the tab if a header isn't wanted. (#294)

## Publishers & Properties

- **[Bug]** **Pausing a Publisher or Property now takes full effect** — Pausing wasn't being enforced consistently on one of the serving paths, so a paused Publisher or Property could still be served. This fix makes the pause reliably stop delivery everywhere. (#299)

## Behind the Scenes

- **[Feature]** **A helper that turns team conversations into tracked tasks** — An internal tool to automatically capture action items from team chats and log them as work items, reducing manual note-taking. No direct effect on the product screens. (#272)
- **[Task]** **Strengthen automated testing** — Behind-the-scenes maintenance to improve the automated checks that guard the admin screens, so problems are caught earlier and more reliably. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
