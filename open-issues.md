# Open Issues — Plain-Language Overview

_Last updated 2026-07-11 13:30:34 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Bring back the Campaigns module** — Campaign management from the old system isn't available yet in New Adsmith Frontend. This high-priority work will let you view, create, and edit campaigns and manage offer groups and their offers, just like before. (#200)
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers currently never fire, so successful conversions aren't being counted. This fix makes configured success pixels work reliably again. (#297)
- **[Bug]** **Some saved offer settings aren't reaching live pages** — A number of offer options you can set on the form (including modal fields and a few delivery flags) aren't making it through to what visitors actually see. This work ensures each setting is either honored on live surfaces or removed if unused. (#295)
- **[Task]** **Auto-register offers now respect visitor targeting** — Auto-register offers currently ignore age, gender, state, zip, and device targeting, so they can fire for people they should skip. This work makes them honor the same targeting rules as regular offers. (#333)
- **[Feature]** **Preview offers and placements with unsaved changes** — Today the Preview button shows the last-saved version, so you have to save before you can see edits. Soon the preview will reflect your current, in-progress changes without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, New Adsmith Frontend will estimate how a new offer is likely to perform based on your historical offer data, giving you a helpful projection at intake. (#322)

## Admin Area

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record, one can currently save over the other's changes without warning. This adds an editing lock and a "changed by someone else" alert so nobody loses work, across all the main entity screens. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when across the app, including automated changes, so you can easily answer "who edited this and when." You'll be able to search and filter it, and view a record's history from its detail page. (#276)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings (Advertiser Web Presence fields, some user-permission toggles, a couple of Data-Client and Pre-Ping options) are saved but have no effect. These will be hidden or removed so the screens only show controls that actually work. (#296)
- **[Task]** **Users screen comparison with the old system** — A behind-the-scenes review comparing the old Users management to the new one, identifying which features still need to be carried over. Groundwork to bring the Users area up to full parity. (#80)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent yet. This is a quick decision on whether it's still needed or can be retired. (#328)

## Surveys

- **[Feature]** **Make sure every survey design option actually works** — A full review to confirm that each customization on the design tab is reflected in the live survey, with any options that don't do anything fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Some Placement design options (like iframe height and display format) are saved but not applied to the survey widget. This work wires the remaining settings through so they take effect. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore custom pre-delivery checks for data clients** — The old system's per-client validation checks (used by 448 data clients) don't run yet on the new platform. This work brings those checks back so leads are validated as before. (#338)
- **[Feature]** **Restore after-success delivery scripts** — Post-conversion delivery and redirect behavior for certain clients wasn't carried over. This adds a general, configurable way to run those after-success actions again. (#327)

## Behind the Scenes

- **[Task]** **A staging environment for safe testing** — Setting up a read-only staging version of New Adsmith Frontend that mirrors production data, so the team can verify things against realistic data without risk of changing anything. (#270)
- **[Feature]** **Turn Slack conversations into tracked to-dos automatically** — An internal helper that reads designated Slack channels and files action items as tracked issues, cutting out manual copy-paste. (#272)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or stack awkwardly compared to other screens. This cleans up the layout so text boxes, color pickers, and paired fields look consistent and tidy. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — All six fields on the Modal design tab are saved but never shown to visitors. This work either wires them into the visitor modal or removes the tab if it isn't needed. (#294)

## Dashboard

- **[Task]** **Investigate why dashboard numbers don't match the old system** — Testers noticed report figures on the dashboard didn't line up with the legacy app. This investigation will pin down the cause and confirm the numbers are accurate. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
