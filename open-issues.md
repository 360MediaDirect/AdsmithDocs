# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 05:18:32 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — When you pick "Custom" on the date filter, you'll get a proper start-and-end date picker so you can view Dashboard data for any range you choose, not just the preset options. (#58)
- **[Feature]** **Pick report dates right from the Dashboard** — You'll be able to pull daily or custom-range reports using controls built into the Dashboard toolbar, so there's no more editing the web address by hand. Links still stay shareable. (#268)
- **[Task]** **Cleaner Dashboard header and tables** — The header will show the brand logo instead of the "Adsmith" text, long offer names will no longer be cut off, and table rows will use tidy alternating shading for easier reading. (#283)
- **[Task]** **Update notes get their own table** — Update notes will be split out from optimizations and general notes so they're easy to spot instead of getting lost in the mix. (#284)
- **[Task]** **Shorter, clearer offer names** — Offer names will drop the repetitive text before the first colon and show only the meaningful part. Names without a colon stay exactly as they are. (#285)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data for your own reporting. This is a high-priority addition. (#286)

## General / Across the App

- **[Feature]** **Prevent overwriting each other's edits** — When two people open the same record, you'll see a clear "being edited by someone else" notice and a warning if the record changed since you opened it, so nobody's work gets silently wiped out. (#267)
- **[Feature]** **A searchable history of every change** — Every create, edit, pause, or automated change across the app will be recorded with who did it and when, viewable in a new searchable Audit Log and on each record's history. Great for answering "who changed this?" (#276)
- **[Bug]** **Invalid links show a real error** — When you test a link that isn't valid, you'll get a clear error message instead of being unexpectedly sent to the Dashboard. This fix is nearly complete. (#239)
- **[Task]** **Filling gaps in the Users area** — A review comparing the old and new Users screens is underway to bring back missing tools like bulk actions, role changes, and login/2FA details. (#80)
- **[Feature]** **Bring back the Campaigns module** — Campaign management from the old admin isn't in New Adsmith Frontend yet. This high-priority work will let you create, edit, and manage campaigns and offer groups again. (#200)

## Surveys

- **[Task]** **Survey images show in full** — Survey images will fit within their space instead of being cropped, so the whole image is always visible. (#287)
- **[Feature]** **Design settings that actually apply** — Every option on the Design tab will be checked end-to-end so your customizations reliably show up in the live survey, with no settings that quietly do nothing. (#288)
- **[Bug]** **Survey styling controls take effect** — Many survey appearance settings (colors, buttons, header text, legal text, and more) are saved but don't currently change what visitors see. This fix wires them all through so your choices are honored. (#290)

## Behind the Scenes

- **[Task]** **A safe testing environment** — A separate staging setup loaded with May and June data so reports and features can be tested thoroughly without touching live information. (#270)
- **[Task]** **Confirming report numbers match the old system** — An investigation into why some Dashboard report figures differed from the legacy system, to pinpoint the cause and confirm the numbers are trustworthy. (#271)
- **[Feature]** **Turning conversations into tracked tasks** — A helper that reads team chat messages and automatically files them as work items, cutting out manual copy-and-paste. (#272)

## Placements

- **[Feature]** **Better control over the offer list** — Follow-up improvements so new placements can default to your chosen manual offer order, and you can filter the available offers by category to find them faster. (#275)
- **[Feature]** **Preview before you save** — A preview button on the placement and offer add/edit pages will let you see how things will look using your current, unsaved changes. (#289)

## Reports

- **[Task]** **Sortable Offer Audit tables** — You'll be able to click column headers to sort the Offer Performance Audit results by any measure, making it easy to spot standout performers. (#281)

## Flows

- **[Task]** **Consistent styling on the Flow form** — Fixes so the Flow form's text boxes, color pickers, checkboxes, and paired fields look polished and match the other forms in the app. Partly done, with a careful final pass remaining. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 7cf2416479c6a006663477450a87c48f16726c5f92d204cab5941b3f0ca4624c -->
