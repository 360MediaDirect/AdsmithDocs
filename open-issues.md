# Open Issues — Plain-Language Overview

_Last updated 2026-08-18 06:06:46 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Manually selected offers aren't carrying over from the old system** — On placements set to "Manual" delivery, the new app is showing an empty "Selected Offers" list, so visitors see the wrong offers. This fix ensures your hand-picked offers (and their order) appear exactly as they did in the old app. (#370)
- **[Bug]** **Set surveys to Display or AR from Offer Details** — The Display and AR options on the Offer Details → Delivery tab currently show as headings only, with no way to actually choose them. This restores the selection controls so you can assign a survey's delivery mode again. (#371)
- **[Bug]** **Some offer settings never reach the live offer** — Several saved offer options (including Modal-tab fields, Display URL, and "Force More Info Visible") are quietly getting dropped and never appear where visitors see them. This work makes sure the options you set actually take effect, or removes any that do nothing. (#295)
- **[Bug]** **Offer edits should show up in History** — Right now, editing an offer doesn't always add an entry to its "History" section, even after a successful save. This fix ensures your changes are properly recorded so you have a reliable trail of what changed and when. (#380)
- **[Feature]** **Preview offers and placements with your unsaved changes** — The Preview button will show your in-progress edits instead of only the last saved version, so you can check how a change looks before committing to it. (#292)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool to automatically estimate a new offer's likely performance based on your historical offer data, replacing today's manual gut-check review. (#322)

## Behind the Scenes

- **[Feature]** **Turn Slack conversations into tracked work items** — Behind-the-scenes tooling to automatically capture action items from team discussions, reducing manual note-keeping. No direct effect on the product screens. (#272)
- **[Task]** **Strengthening our automated testing** — Improvements to the internal test suite so more of the app is genuinely checked before release, making the product more reliable over time. This is behind-the-scenes quality work. (#379)

## Surveys

- **[Feature]** **Make every survey customization option actually work** — A thorough review to confirm that every design and form option you can set is truly reflected in the live survey, with anything unused either fixed or removed. Fewer settings that appear to do nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Some Placement Design-tab settings (like iFrame height and display format) are saved but don't yet show up in the survey visitors see. This wires them through so your choices take effect. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery steps** — Certain "after-success" behaviors from the old system weren't carried into the new platform. This work brings that delivery/redirect behavior back so conversions are handled correctly. (#327)
- **[Feature]** **Bring back custom pre-check validation for data clients** — A high-priority effort to restore the per-client checks that run before a lead is delivered. Hundreds of data clients relied on this in the old system, and it currently doesn't run on the new platform. (#338)

## Dashboard

- **[Task]** **Confirm dashboard report numbers match the old system** — An investigation into why some dashboard figures didn't line up with the legacy app during testing, so you can trust the reported numbers. (#271)
- **[Feature]** **Add notes to Placements, Advertisers, and Offers** — Brings back the ability to attach short, categorized notes to a record from its detail page, with a recent-notes roll-up on the main Dashboard. Notes will appear immediately without needing a page reload. (#382)

## General / Across the App

- **[Task]** **Closing the gaps between the old and new Users area** — A review comparing the old Users screens with the new ones to identify missing capabilities (like bulk role changes and last-login info) so the new Users area catches up to what you had before. (#80)
- **[Feature]** **Remove settings that don't actually do anything** — Several admin controls (such as the Advertiser Web Presence tab, certain user permission toggles, and some data-client and pre-ping options) are saved but have no effect. These will be hidden or removed so the screens only show controls that genuinely work. (#296)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — The entire Modal Design tab (headers, colors, progress bar) currently has no effect on what visitors see. This work either wires those settings through to the live modal or removes the tab if it isn't needed. (#294)

## Advertisers

- **[Feature]** **Show advertiser website and social links on the detail page** — The Web Presence details you enter for an advertiser aren't currently displayed anywhere. This adds the familiar cluster of website, social, and "Search on Google" icon links to the Advertiser detail page. (#383)

## Publishers & Properties

- **[Bug]** **Make pausing a publisher or property reliable** — A pause check on one of the serving paths never actually triggers, so a paused publisher or property may still serve. This fix ensures pausing is enforced consistently everywhere. (#299)

## Flows

- **[Task]** **Fix the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacked instead of side-by-side). This tidies up the form so it matches the look of the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
