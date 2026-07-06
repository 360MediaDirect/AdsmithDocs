# Open Issues — Plain-Language Overview

_Last updated 2026-07-06 13:13:11 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Bug]** **Invalid links now show a clear error instead of bouncing to the Dashboard** — When you test a link that isn't valid, you'll see a proper failure message right in the Link Testing screen rather than being sent back to the Dashboard with no explanation. (#239)
- **[Feature]** **Protection against two people overwriting each other's edits** — When someone else is already editing a record (an offer, flow, placement, advertiser, and so on), you'll see a clear "locked by" banner, and the system will warn you before your save can wipe out changes another user just made. This works consistently across every entity screen. (#267)
- **[Feature]** **Searchable history of who changed what and when** — A new admin Audit Log will record every manual and automated change across the platform, so you can look up exactly who paused an offer, edited a placement, or updated a record, and when. Each entity's detail page will also show its own history. (#276)
- **[Feature]** **Clean up admin controls that don't actually do anything** — Several settings that are saved but have no real effect (such as the Advertiser Web Presence fields, certain user permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden so the screens only show controls that truly work. (#296)

## Surveys
- **[Feature]** **Make sure every Design-tab option actually changes the survey** — A full audit will confirm that each customization you set on the Design tab is reflected in the live survey visitors see, with no "dead" settings that appear to work but don't. (#288)
- **[Bug]** **Most survey styling settings will finally take effect** — Today only a couple of the roughly 30 Design-tab options (colors, buttons, headers, legal text, and more) actually reach the live survey widget. This work wires the rest through so what you configure is what visitors see. (#290)
- **[Bug]** **Voucher codes and info links will show on the live survey again** — Configured items like the voucher code line and the privacy/terms/details links currently save correctly but don't appear on the new survey page. This restores them to match the legacy experience. (#291)
- **[Feature]** **Finish connecting the last few Placement Design settings** — Building on the earlier fix, the remaining survey settings (such as widget height and display format) will either be fully applied to the live widget or removed if they're not needed, so nothing on the form is misleading. (#293)

## Placements
- **[Feature]** **Manual offer order and a vertical filter for the offer picker** — New placements will be able to default to your hand-set offer order (so your drag-and-drop arrangement is actually used), and you'll be able to filter the available offers list by vertical instead of only searching by text. (#275)
- **[Feature]** **Preview your unsaved changes before saving** — The Preview button on placement and offer edit screens will show your current in-progress edits, so you no longer have to save first just to see how a change looks. (#292)

## Dashboard
- **[Task]** **Confirming report numbers match the legacy system** — An investigation into why some dashboard report figures differed from the old system, so you can trust that the new platform's numbers line up. (#271)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example as a spreadsheet) for your own analysis. This is a high-priority addition. (#286)

## Behind the Scenes
- **[Task]** **A read-only staging environment for safe testing** — Setting up a separate testing environment loaded with production-like data, locked to read-only so testers can validate the product without any risk of changing real records. (#270)
- **[Feature]** **Automatically turn Slack conversations into tracked tasks** — A helper that reads designated Slack channels, spots action items, and files them as tracked issues automatically, cutting out manual copy-and-paste and posting confirmation links back in Slack. (#272)

## Offers
- **[Bug]** **Saved offer options that never reached the live widget** — Several fields saved on the offer form (including the Modal-tab fields, Force More Info Visible, Display URL, and some data-client flags) currently get dropped before reaching visitors. Each will be properly connected or removed so the form only shows options that actually take effect. (#295)

## Modals
- **[Feature]** **Fix the Modal Design tab so its settings actually apply** — All six fields on the Modal Design tab currently save but have no effect on the modal visitors see. Each will either be wired up to work or removed so the tab isn't misleading. (#294)

## Flows
- **[Task]** **Tidy up the Flow form's appearance** — The Flow form has some styling gaps that leave text boxes, color pickers, checkboxes, and paired fields looking unpolished. This cleanup brings it in line with the Placement and Modal forms. Part of it is done, with the rest handled carefully to avoid disrupting other tabs. (#152)

## Campaigns
- **[Feature]** **Bring the Campaigns module into the new platform** — Campaign management doesn't yet exist in New Adsmith Frontend. This high-priority work adds the ability to view, create, edit, and configure campaigns and offer groups, matching what the legacy admin can do. (#200)

## Users
- **[Task]** **Comparing the Users screens against the legacy version** — A review documenting which Users features from the old system are still missing in New Adsmith Frontend (such as bulk actions and login/2FA details) so the team can prioritize closing the gaps. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
