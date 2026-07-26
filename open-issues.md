# Open Issues — Plain-Language Overview

_Last updated 2026-07-26 06:52:40 UTC · 14 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on placements and offers** — When editing a placement or offer, the Preview button will show your latest changes right away, so you no longer have to save first just to see how an edit looks. (#292)
- **[Bug]** **Some saved offer options weren't showing to visitors** — A number of offer settings you fill in (including modal-related options and display details) weren't making it through to the live experience. This fix ensures the choices you save actually take effect, or removes any options that do nothing. (#295)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature that estimates how a new offer is likely to perform based on your historical offer data, giving you a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Surveys

- **[Feature]** **Make sure every design option actually changes the survey** — A thorough review across all entities to confirm that each customization option you set on a Design tab is truly reflected in what visitors see, with any non-working options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — A handful of Placement design options (such as height and display format) will properly take effect in the survey visitors see, and any leftover options that don't do anything will be cleaned up. (#293)

## Data Clients

- **[Feature]** **Bring post-conversion delivery steps to the new platform** — Certain after-success behaviors (delivery and redirect steps that run once a visitor converts) from the older system are being carried over, so those clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — High priority. Many data clients rely on custom validation that runs before a lead is served, and that logic isn't yet active on the new platform. This work restores those checks so leads are validated the same way they used to be. (#338)

## General / Across the App

- **[Task]** **Comparing the old and new Users area** — A detailed review of the Users section against the previous system to spot missing pieces (like bulk actions, last-login info, and two-factor status) so the new Users area can catch up to what you had before. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Some settings across Advertisers, Users, Data Clients, and Pre-Pings currently save but have no effect. These misleading controls will be hidden or removed so what you see in the admin area is trustworthy and accurate. (#296)

## Behind the Scenes

- **[Task]** **A safe, look-only test environment** — Setting up a separate testing environment loaded with realistic data where changes can't accidentally be saved, so the team can verify the product against real-world numbers. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads team conversations and automatically files the resulting to-dos, reducing manual note-taking and making sure requests don't slip through the cracks. (#272)

## Reports

- **[Task]** **Checking dashboard report numbers against the old system** — An investigation into why some dashboard figures didn't match the previous system, to pin down the cause and confirm the numbers you see are accurate. (#271)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Some parts of the Flow form appear unstyled or awkwardly stacked. This work brings its appearance in line with the Placement and Modal forms so paired fields sit side by side and everything looks polished. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — The Modal Design tab's settings (header text, colors, progress bar) currently have no effect on what visitors see. This work will either make those options work or remove the tab so it isn't misleading. (#294)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
