# Open Issues — Plain-Language Overview

_Last updated 2026-08-09 06:14:20 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer settings never reach live ads** — Several options you can set on an offer (including its Modal-tab fields and a few delivery flags) aren't being passed through to what visitors actually see. This fix makes sure the settings you save are the ones that apply, or clearly removes options that don't do anything. (#295)
- **[Bug]** **Manually selected offers weren't carried over from the old system** — On placements set to manual delivery, the list of hand-picked offers was coming across empty, so the new app showed different offers than the old one. This restores the correct selected offers and their order. (#370)
- **[Bug]** **Display/AR controls missing on Offer Delivery** — The controls to set a survey to Display or AR on the Offer Details Delivery tab are being restored, so you can configure delivery mode without switching back to the old app. (#371)
- **[Bug]** **Offer edits not appearing in History** — After editing and saving an offer, the change wasn't showing up in the offer's History section. This ensures your edits are recorded there. (#380)
- **[Feature]** **Preview shows your unsaved changes** — The Preview button on placement and offer edit pages will reflect the changes you're currently making, so you no longer have to save first just to see how something looks. (#292)
- **[Feature]** **Automatic performance projection for new offers** — Instead of a manual gut-check review, new offers could be scored against past offers and historical results to estimate how they're likely to perform. This is an exploratory idea to help at offer intake. (#322)

## Surveys

- **[Feature]** **Every survey design option actually takes effect** — A full check to confirm that each customization option in the design tabs is truly reflected in the live survey, with any options that do nothing either fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A handful of Placement design-tab settings (like survey height and display format) aren't yet reaching the live survey. This wires up the remaining ones so they take effect, or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — Certain "after success" delivery and redirect steps from the old system are being brought over so they run correctly on the new platform. (#327)
- **[Feature]** **Restore custom pre-check validation for data clients** — Legacy per-client validation that ran at serve time hasn't yet carried over, affecting a large number of clients. This work re-creates that validation so those checks run again. High priority. (#338)

## Dashboard & Reports

- **[Task]** **Investigate report numbers that don't match the old system** — Some dashboard report figures didn't line up with the legacy app during testing. This looks into where the difference comes from and confirms the numbers are correct. (#271)
- **[Feature]** **Add notes to Placements, Advertisers, and Offers** — You'll be able to attach short, categorized notes (with a topic and priority) directly from a Placement, Advertiser, or Offer detail page, and see a recent-notes roll-up on the main Dashboard. (#382)

## Admin

- **[Task]** **Review of user-management features vs. the old system** — A behind-the-scenes comparison of the old Users area against the new one to identify which features still need to be added (like bulk actions and last-login details). (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Some settings currently appear in the admin area but have no effect (for example certain Advertiser web-presence fields and unused permission toggles). These will be removed or hidden so the screens only show controls that actually work. (#296)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The Modal Design tab's settings (header text, colors, progress bar, etc.) currently save but never show up in the visitor modal. This either makes them display properly or removes the tab if it isn't needed. (#294)

## Advertisers

- **[Feature]** **Show Web Presence links on the Advertiser detail page** — The website, social profiles, and a "Search on Google" shortcut you enter on the Web Presence tab will appear as icon links in the Advertiser detail header, matching the old app (and now including all networks). (#383)

## Publishers

- **[Bug]** **Pausing a publisher or property now takes full effect** — A pause wasn't being enforced on one of the serving paths, so a paused publisher or property could still be treated as active. This makes pausing behave consistently everywhere. (#299)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form look unstyled or misaligned (plain textareas, unstyled color pickers, fields stacking instead of sitting side by side). This tidies up the form so it matches the other screens. (#152)

## Behind the Scenes

- **[Feature]** **Slack-to-issue helper** — An internal tool that turns action items from Slack conversations into tracked work items automatically, so notes don't have to be copied over by hand. No visible change in the product. (#272)
- **[Task]** **Improvements to automated testing** — Behind-the-scenes fixes to the automated test suite so it catches more problems reliably. No visible change in the product. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
