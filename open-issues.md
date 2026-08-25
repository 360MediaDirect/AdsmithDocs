# Open Issues — Plain-Language Overview

_Last updated 2026-08-25 06:07:34 UTC · 17 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Placements & Offers

- **[Feature]** **Preview shows your unsaved edits** — When you preview a placement or offer while editing, the preview will reflect the changes you've made right now, instead of only the last version you saved. No more saving just to see how a tweak looks. (#292)
- **[Feature]** **Placement Design settings that actually show up** — Several Design-tab options on Placements are saved but don't yet change what visitors see. This work connects them so choices like display format and survey height take effect (and removes any options that do nothing). (#293)
- **[Bug]** **Offer settings that weren't reaching visitors** — A number of saved offer options (including Modal-tab settings and Display URL) never made it to the live offer visitors see. This fixes the hand-off so your saved choices are honored or clearly retired. High priority. (#295)
- **[Bug]** **Manually selected offers now carry over correctly** — On placements using manual offer delivery, the list of hand-picked offers wasn't transferring into New Adsmith Frontend, so visitors saw the wrong or empty offers. This ensures your selected offers and their order match. High priority, nearly complete. (#370)
- **[Feature]** **Automatic performance estimate for new offers** — An exploratory tool to project how a new offer is likely to perform based on your historical offer data, giving Offers an at-a-glance read at intake instead of relying on a manual gut-check. (#322)

## Data Clients

- **[Feature]** **After-conversion delivery steps restored** — Post-conversion redirect and delivery behaviors from the old system are being carried into New Adsmith Frontend so affected clients keep working as before. Nearly complete. (#327)
- **[Feature]** **File-based pre-ping checks brought forward** — Hundreds of data clients relied on custom pre-ping validation that currently doesn't run in the new platform. This work restores that check at serve time so pass/reject decisions are enforced consistently. High priority. (#338)

## Dashboard & Reports

- **[Task]** **Confirming report numbers match the old system** — An investigation into why some dashboard report figures didn't line up with the legacy app, so you can trust the numbers you see. High priority. (#271)
- **[Feature]** **Notes on Placements, Advertisers, and Offers** — Bringing back the ability to add short, categorized notes right from a Placement, Advertiser, or Offer report, with a recent-notes roll-up on the main Dashboard. New notes will appear without needing a page reload. (#382)

## General / Across the App

- **[Task]** **Users screen feature review** — A review comparing the Users area against the old system to spot missing capabilities (like bulk role changes and last-login info) and plan what to add. (#80)
- **[Feature]** **Removing controls that don't do anything** — Some admin options (such as the Advertiser Web Presence fields and certain user-permission toggles) are saved but have no effect, which can be misleading. These will be hidden or removed, or properly wired up. (#296)

## Surveys

- **[Feature]** **Design choices reflected in the survey view** — Making sure every customization on the Design tab actually shows up in the live survey, plus a full check across all screens to catch any option that isn't fully connected. (#288)

## Flows

- **[Task]** **Tidier Flow form layout** — Fixing styling gaps on the Flow form so text boxes, color pickers, checkboxes, and paired fields display cleanly instead of looking unstyled or stacked awkwardly. In progress. (#152)

## Modals

- **[Feature]** **Modal Design tab wired up or removed** — The Modal Design tab's settings (header text, colors, progress bar) currently don't change what visitors see. This work either makes them take effect or removes them so nothing on the form is misleading. (#294)

## Publishers & Properties

- **[Bug]** **Pausing a publisher or property works reliably** — A pause check wasn't matching correctly, so pausing a publisher or property didn't fully stop it in one path. This ensures a paused item is consistently blocked. High priority. (#299)

## Behind the Scenes

- **[Feature]** **Automatic issue capture from team chats** — An internal helper to turn action items from team conversations into tracked tickets, reducing manual note-keeping. No visible change in the product. (#272)
- **[Task]** **Strengthening automated testing** — Behind-the-scenes improvements to the automated test suite so problems are caught earlier and more reliably before reaching you. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
