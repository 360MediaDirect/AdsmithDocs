# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 01:41:01 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Picking "Custom" in the date filter will open a proper start/end date picker so you can view Dashboard data for any range you choose, not just the preset options. (#58)
- **[Feature]** **Change report dates without touching the web address** — New date controls in the Dashboard toolbar let you pull daily or custom-range reports directly, instead of hand-editing the address bar. Links will still update so you can bookmark and share them. (#268)
- **[Task]** **Cleaner Dashboard header and tables** — The header will show the logo instead of the "Adsmith" text, full offer names will no longer be cut off, and table rows will get tidy alternating background shading for easier reading. (#283)
- **[Task]** **Update notes get their own table** — Update notes will be separated from optimizations and general notes into a dedicated table so they're easy to spot and don't get lost. (#284)
- **[Task]** **Shorter, cleaner offer names** — Offer names that contain a colon will show only the meaningful part after it, trimming redundant prefix text. Names without a colon stay exactly as they are. (#285)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (for example, to a spreadsheet). This is a high-priority addition. (#286)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit, it will be locked so a second person can't accidentally save over your work. If someone else already has it open, you'll see a clear "locked by" message, and you'll be warned if a record changes while you have it open. This works across all editable screens. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when across the app, including automated changes, so you can always trace how a record got to its current state. (#276)
- **[Task]** **Review of the Users area for missing features** — A comparison of the old and new Users screens to catch anything the new version is still missing, guiding what gets built next. This is a documentation and planning task. (#80)
- **[Bug]** **Clearer result when testing an invalid link** — Testing a bad link currently drops you on the Dashboard with no explanation. It will instead show a clear error so you know the link failed. This fix is nearly complete. (#239)

## Surveys

- **[Task]** **Survey images show in full** — Survey images will fit within their space instead of being cropped, so the whole image is always visible. (#287)
- **[Feature]** **Design settings that actually take effect** — Every option on the Design tab will be connected to what visitors see, and all entity forms will be reviewed to confirm no setting is a dead end. (#288)
- **[Bug]** **Design tab styling reaches the live survey** — Most Design-tab settings (colors, continue button, header text, legal text, and more) are saved but currently have no effect on the live survey. This connects them so your styling choices actually appear to visitors. (#290)

## Reports

- **[Task]** **Sortable Offer Audit tables** — You'll be able to click any column header in the Offer Performance Audit tables to re-sort the results, making it easier to spot standout numbers instead of being stuck with a single fixed order. (#281)
- **[Task]** **Confirming report numbers match the old system** — An investigation into why some Dashboard report figures differ from the legacy system, so we can pinpoint the cause and confirm the numbers are trustworthy. (#271)

## Placements

- **[Feature]** **Better control of offer order and selection** — Follow-up work so manually reordered offers are respected by default, plus a new filter to narrow the available offers list by category when building a placement. (#275)
- **[Feature]** **Preview placements and offers before saving** — A new preview button on the placement and offer add/edit screens will show how your changes will look based on the current form, before you save. (#289)

## Behind the Scenes

- **[Task]** **A safe testing environment with real sample data** — Setting up a separate staging area loaded with May and June data so reports and features can be validated without touching live information. (#270)
- **[Feature]** **Turning conversations into tracked work items** — A helper that reads team chat and automatically files action items as tracked issues, reducing manual copy-and-paste and keeping requests from slipping through. (#272)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — The Campaigns area from the old admin isn't in New Adsmith Frontend yet. This adds it back so you can view, create, edit, and configure campaigns and offer groups. This is a critical, high-priority addition. (#200)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned (plain text boxes, stacked fields, unstyled color pickers). This tidies up the layout so it matches the polished look of other forms. Partly done, with a careful final pass remaining. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 7cf2416479c6a006663477450a87c48f16726c5f92d204cab5941b3f0ca4624c -->
