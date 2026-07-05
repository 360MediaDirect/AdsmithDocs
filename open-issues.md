# Open Issues — Plain-Language Overview

_Last updated 2026-07-05 15:27:09 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make every survey Design-tab option actually work** — Once complete, the styling and behavior choices you set in a survey's Design tab will be reliably reflected in the live survey, and we'll review form options across all entity screens so none are dead ends. (#288)
- **[Bug]** **Survey styling settings not reaching visitors** — Today only a couple of the ~30 Design-tab options change the live survey. This fix makes your configured colors, continue button, answer style, headers, and legal text actually appear to visitors. (#290)
- **[Bug]** **Voucher code and info links missing on the live survey** — Restores the voucher code line and the privacy/terms/details links that are set up in the admin but currently don't show on the new survey page. (#291)
- **[Feature]** **Finish wiring the remaining placement survey settings** — Completes the last few Design-tab settings (like widget height and display format) so they take effect, and clears out any options that do nothing. (#293)

## General / Across the App

- **[Feature]** **Warn when two people edit the same record** — When someone else already has a record open, you'll see who's editing it and be protected from accidentally overwriting each other's changes. (#267)
- **[Feature]** **Searchable history of changes** — A new admin audit log will let you see who changed what and when across the platform, making it much easier to track down and troubleshoot changes. (#276)
- **[Feature]** **Remove admin controls that do nothing** — Settings that are saved but have no effect (such as the Advertiser Web Presence fields and certain user-permission toggles) will be hidden or removed, so screens only show controls that actually work. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Testing an invalid link will now return a clear failure message instead of quietly sending you back to the dashboard. (#239)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — You'll be able to download the breakdown-by-day data with a new export button. This is a high-priority addition. (#286)
- **[Task]** **Confirm dashboard numbers match the legacy system** — An investigation to compare report figures between the old and new platforms, pin down any differences, and confirm the numbers line up. (#271)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on placements** — Manual offer order will be respected by default, and you'll be able to filter the available-offers list by vertical instead of only searching by text. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show your current, in-progress edits rather than the last saved version, so you can check changes before saving. (#292)

## Offers

- **[Bug]** **Saved offer options not reaching the live widget** — Several offer settings that are saved in the admin currently never make it to what visitors see. This fixes them so your choices take effect (or removes any that are intentionally unused). (#295)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The modal's Design-tab settings (header text, colors, progress bar) currently have no effect. They'll either be wired up to the visitor modal or removed so the screen isn't misleading. (#294)

## Campaigns

- **[Feature]** **Bring Campaigns to the new platform** — The Campaigns module from the old admin isn't in New Adsmith Frontend yet. This high-priority work adds it back so you can create, edit, and manage campaigns and their offer groups. (#200)

## Flows

- **[Task]** **Fix the look of the Flow form** — Cleans up unstyled and misaligned areas of the Flow form (text boxes, color pickers, checkboxes, and side-by-side fields) so it matches the polished look of the other forms. (#152)

## Users

- **[Task]** **Compare the old and new Users screens** — A documentation review that maps what the legacy Users area could do against the new one, so any missing capabilities can be prioritized and planned. (#80)

## Behind the Scenes

- **[Task]** **Set up a safe testing environment** — Behind-the-scenes work to run a read-only copy of the platform against production-like data for verification, with no risk of changing real records. (#270)
- **[Feature]** **Turn team conversations into tracked tasks automatically** — An internal tool that captures action items from team chats and files them as tracked work items, reducing manual copy-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
