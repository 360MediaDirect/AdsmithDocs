# Open Issues — Plain-Language Overview

_Last updated 2026-08-28 09:03:46 UTC · 15 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never appear where they should** — Several options you can set on an offer (including the four Modal-tab fields, Display URL, "Force More Info Visible," and certain data-client flags) aren't currently carried through to the live experience. This fix ensures the settings you save actually take effect, or removes options that do nothing. (#295)
- **[Bug]** **Manually chosen offers now show up correctly** — On placements set to manual offer delivery, the specific offers you picked (and their order) weren't carrying over into New Adsmith Frontend, so the wrong or empty offers displayed. Your hand-selected offer lineup will match what you configured. (#370)
- **[Feature]** **Preview your unsaved edits before saving** — On the placement and offer edit screens, the Preview button will reflect the changes you're currently making, so you can check your work without having to save first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, new offers could get an estimated performance projection based on your own historical offer data, giving you a data-driven read at intake. This is an exploratory feature with no set deadline. (#322)

## Dashboard & Reports

- **[Feature]** **Attach notes to Placements, Advertisers, and Offers** — You'll be able to add short, categorized notes (with topic and priority) right from an object's report dashboard, see them appear without reloading the page, and view a recent-notes roll-up on the main Dashboard. This brings back a familiar capability from the previous app. (#382)
- **[Task]** **Confirming report numbers match the old system** — A high-priority investigation into why some Dashboard report figures didn't line up with the legacy app, so you can trust that the numbers are accurate and consistent. (#271)

## Data Clients

- **[Feature]** **Restoring "after-success" delivery behavior** — Post-conversion delivery and redirect steps from the old app are being brought over so that everything that happened after a successful conversion continues to work as before. Nearly complete. (#327)
- **[Feature]** **Bringing over custom pre-ping validation** — Hundreds of data clients relied on custom checks that ran before serving; this high-priority work reconnects that validation in New Adsmith Frontend so those clients behave as they did in the old system. (#338)

## Admin & Users

- **[Task]** **Closing the gap between the old and new Users area** — A detailed review comparing the previous Users management to New Adsmith Frontend, identifying missing pieces (like bulk actions and extra columns) so the new Users area can match what people relied on before. (#80)
- **[Feature]** **Removing admin controls that don't do anything** — Certain settings (some user-permission toggles, a couple of Data-Client fields, and a Pre-Ping option) currently appear but have no effect. They'll be hidden or removed so the admin screens only show controls that actually work. (#296)

## Surveys

- **[Feature]** **Design choices reliably show up in the survey** — Every customization on the design tab will be checked to confirm it truly carries through to what visitors see, and all entity form options will be audited so nothing is left disconnected. (#288)

## Flows

- **[Task]** **Cleaning up the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacking instead of sitting side by side). This tidies up the layout to match the polished look of other forms. (#152)

## Publishers

- **[Bug]** **Pausing a publisher or property will fully take effect** — A flaw meant one path wasn't recognizing the paused state, so enforcement was inconsistent. Once fixed, pausing reliably stops serving as expected. (#299)

## Behind the Scenes

- **[Feature]** **Turning conversations into tracked work automatically** — A helper that reads discussion notes and files them as work items, reducing manual copy-and-paste when capturing action items. No user-facing change. (#272)
- **[Task]** **Strengthening automated testing** — A review of the product's automated test coverage surfaced gaps (some tests weren't truly running, and the suite wasn't run regularly). Addressing these helps catch issues earlier, behind the scenes. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
