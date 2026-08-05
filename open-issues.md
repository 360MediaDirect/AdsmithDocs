# Open Issues — Plain-Language Overview

_Last updated 2026-08-05 06:50:44 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach the live ad** — Several options you set on an offer (the Modal-tab fields, the offer-level "Force More Info Visible," Display URL, and some data-delivery flags) currently don't carry through to what visitors actually see. This fix makes sure every saved option either takes effect or is cleaned up so it isn't misleading. (#295)
- **[Bug]** **Manually selected offers now show correctly on Manual-delivery placements** — On placements set to deliver offers manually, the new platform was showing the wrong or no offers because the hand-picked offer list wasn't carried over. Once fixed, these placements will display the same offers, in the same order, as before. (#370)
- **[Bug]** **Display/AR controls back on the Offer Details Delivery tab** — The Display and AR columns currently show as headings only, so you can't set a survey to Display or AR. This restores the selectable controls so you can configure delivery mode without switching to the old app. (#371)
- **[Bug]** **Offer edits will show up in History** — Right now, editing an offer saves your change but doesn't add a "History" entry, so there's no record of what changed. This fix makes every edit appear in the offer's History section. (#380)
- **[Feature]** **Preview shows your unsaved changes on Placements and Offers** — Today the Preview button only shows the last-saved version, so you must save before you can see a tweak. You'll be able to preview your in-progress edits without saving first. (#292)
- **[Feature]** **Automatic performance projection for new offers** — When a new offer comes in, the product will estimate how it's likely to perform based on your own historical offer data, replacing today's informal manual gut-check with a data-driven projection at intake. (#322)

## Surveys & Modals

- **[Feature]** **Every design option actually shows up in the survey** — This makes sure all the customizations on the Design tab are connected end-to-end and reflected in what visitors see, plus a sweep across all entities to confirm no option is a dead control. (#288)
- **[Feature]** **Finishing the Placement Design-tab settings** — A handful of Placement Design settings (like survey height and display format) are saved but not yet applied to the live widget. This wires the remaining ones through, or removes any that aren't needed, so what you set is what visitors get. (#293)
- **[Feature]** **Modal Design tab will do what it says** — The Modal Design tab's header and progress-bar settings are currently saved but never shown to visitors. This will either make those settings work in the visitor modal or remove them so the tab isn't misleading. (#294)

## Data Clients

- **[Feature]** **Post-conversion delivery steps brought over from the old system** — Certain "after success" actions that run once a lead converts (like delivery and redirect steps for specific clients) weren't yet available on the new platform. This ports them over so those clients keep working as expected. (#327)
- **[Feature]** **Custom pre-check validation restored for data clients** — Many data clients relied on a custom serve-time validation step that isn't running on the new platform yet. This high-priority work brings that validation back so leads are checked and accepted or rejected consistently. (#338)

## Behind the Scenes

- **[Feature]** **Turning conversations into tracked work automatically** — A new helper will read designated chat channels and file the action items as tracked issues automatically, saving the manual copy-and-paste step. This is internal tooling with no direct change to the product screens. (#272)
- **[Task]** **Tightening up automated testing** — A review of the automated test suite found a few gaps to close so testing catches problems more reliably. Behind-the-scenes quality work with no visible change to the app. (#379)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned — plain text boxes, unstyled color pickers, and paired fields stacking instead of sitting side by side. This cleans up the form's appearance to match the rest of the app. (#152)

## Users

- **[Task]** **Reviewing the Users area against the old system** — A detailed comparison of the old and new Users screens to spot missing capabilities (like bulk actions, last-login and two-factor status, and password-on-create) and prioritize what to add next. (#80)

## Dashboard & Reports

- **[Task]** **Checking why dashboard report numbers differ from the old system** — During testing, some dashboard report figures didn't match the legacy app. This investigation compares the two over a fixed date range to find the cause and confirm the numbers can be trusted. (#271)

## Publishers & Properties

- **[Bug]** **Pausing a publisher or property will be fully enforced** — A gap in one of the checks means pausing didn't reliably take effect everywhere. This fix ensures a paused publisher or property is consistently blocked from serving. (#299)

## General / Across the App

- **[Feature]** **Removing admin controls that don't actually do anything** — Several settings currently save but have no effect (for example, the Advertiser "Web Presence" fields and a couple of user-permission toggles that imply access limits that aren't real). These will be hidden or removed so the admin screens only show controls that truly work. (#296)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
