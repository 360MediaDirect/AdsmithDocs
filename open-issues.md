# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 15:31:10 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some offer settings never reach the live experience** — A number of options you set when editing an offer (such as modal settings and the display URL) aren't currently being applied to what visitors actually see. This fix makes sure the choices you save on an offer take effect. (#295)
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers to record successful leads are silently not firing, which means lost tracking with no warning. This high-priority fix ensures a configured success pixel actually fires. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers currently fire regardless of age, gender, state, ZIP, or device targeting, so they can reach visitors they should exclude. This work aligns them with normal offers so targeting is respected. (#333)
- **[Feature]** **Preview your unsaved offer and placement edits** — On the offer and placement edit screens, the Preview button will show your current in-progress changes instead of only the last saved version, so you can check edits before committing them. (#292)
- **[Feature]** **Performance projections for new offers** — A new tool will estimate how a new offer is likely to perform based on your historical offer data, giving Kurt a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Admin / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else is already editing a record, you'll see a clear notice and be protected from accidentally saving over their changes. This safeguard works across all editable screens (offers, flows, placements, advertisers, and more). (#267)
- **[Feature]** **Clean up controls that don't actually do anything** — Several settings that appear editable but have no effect (like the Advertiser Web Presence tab, certain user permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden so the admin area only shows controls that work. (#296)
- **[Task]** **Bringing the Users area to feature parity** — A review comparing the old Users management to the new one, guiding which missing pieces (like bulk actions and additional columns) still need to be added. (#80)
- **[Bug]** **Invalid links should show an error, not the dashboard** — When testing a link that's invalid, you'll get a clear failure message instead of being unexpectedly sent to the dashboard. (#239)
- **[Task]** **Decide the future of the file-share page** — The old file-share page has no equivalent yet; this is a keep-or-retire decision so it's either rebuilt or intentionally dropped. (#328)

## Surveys

- **[Feature]** **Make every survey design option actually change the survey** — A full check to ensure each customization in the Design tab is reflected in the live survey, with any options that don't do anything either wired up or removed. (#288)
- **[Feature]** **Finish connecting placement design settings to the survey** — Several placement Design-tab settings (such as height and display format) don't yet affect what visitors see; this completes the wiring so they take effect. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore post-conversion delivery for data clients** — After-success delivery and redirect behavior from the old system will be carried over so data clients keep working correctly once a lead succeeds. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Custom validation that runs before serving offers for hundreds of data clients hasn't been carried over yet; this high-priority work brings that logic to the new platform so those clients behave as before. (#338)

## Behind the Scenes

- **[Task]** **Set up a safe testing environment** — A read-only staging setup using production-like data, so the team can verify the product against realistic data without any risk of changing live records. (#270)
- **[Feature]** **Turn Slack conversations into tracked to-dos automatically** — A helper that reads designated Slack discussions and files the action items for the team, reducing manual copy-and-paste when capturing follow-ups. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The Modal Design tab's settings (header text, colors, progress bar) currently don't change anything visitors see; this will either connect them to the visitor modal or remove them so nothing is misleading. (#294)

## Flows

- **[Task]** **Fix unstyled areas of the Flow form** — Parts of the Flow form (text boxes, color pickers, checkboxes, and side-by-side fields) look broken or unstyled; this tidies them up to match the polished look of other forms. (#152)

## Campaigns

- **[Feature]** **Bring back the Campaigns area** — The Campaigns module from the old admin isn't available yet in New Adsmith Frontend. This critical, high-priority work adds it back so you can create, edit, and manage campaigns and offer groups. (#200)

## Reports

- **[Task]** **Confirm dashboard report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy app, so the numbers can be trusted and any discrepancy is explained and corrected. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f12be1691f4d05be7a51684fc6fe5ab6d4c4751d5a9de6a600395df673d554b3 -->
