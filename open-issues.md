# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 18:30:55 UTC · 17 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Pick your own date range on the Dashboard** — Choosing "Custom" in the date filter will open a proper start-and-end date picker, so you can view results for any span you like instead of only the preset options. (#58)
- **[Feature]** **Change report dates without editing the web address** — New date controls will live right in the dashboard toolbar, so you can pull a specific day or range with a click. The address bar will still update so links stay shareable, but you'll never have to edit it by hand. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example to a spreadsheet) for your own reporting. This is a high-priority addition. (#286)

## Surveys

- **[Bug]** **Design settings will actually change the survey** — Many styling and behavior options on the survey Design tab currently save but don't affect what visitors see. This work connects those settings (colors, header text, continue button, progress bar, legal text, and more) so your choices show up on the live survey. (#290)
- **[Bug]** **Voucher code and info links will show on the live survey** — A configured voucher-code question and the privacy/terms/details links aren't appearing on the new survey page even though they're saved. This restores them to match the older system. (#291)
- **[Feature]** **Design tab options fully connected everywhere** — A thorough check will confirm every design and form option actually takes effect end to end across the survey and all entity screens, fixing or flagging any option that currently does nothing. (#288)

## General / Across the App

- **[Feature]** **Warning when two people edit the same record** — When someone else already has a record open, you'll see a clear "locked by" notice and be protected from accidentally overwriting their changes when you save. This protection will apply across all editable screens. (#267)
- **[Feature]** **A searchable history of every change** — A new audit log will record who changed what and when (both manual edits and automated updates) across offers, placements, advertisers, and more, with a searchable page and a history view on each record. This makes it easy to answer "who changed this?" (#276)
- **[Bug]** **Clear error for invalid link tests** — Testing an invalid link currently drops you on the dashboard with no explanation. Instead you'll get a clear failure message right where you tested it. This fix is nearly complete. (#239)

## Placements

- **[Feature]** **Preview your unsaved edits** — The Preview button on placement and offer edit screens will show your current in-progress changes, so you no longer have to save first just to see how a change looks. (#292)
- **[Feature]** **Better offer ordering and filtering on placements** — Building on recent drag-to-reorder work, this sets manual ordering to actually take effect and adds a category filter to the available-offers list so it's easier to find the offers you want. (#275)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — Campaign management (viewing, creating, editing campaigns and their offer groups) isn't yet available in New Adsmith Frontend. This high-priority work rebuilds that capability to match the older system. (#200)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned compared with other screens. This cleans up the layout and styling so paired fields, color pickers, and text boxes look consistent. Some of this is already done, with the rest handled carefully to avoid disrupting other tabs. (#152)

## Behind the Scenes

- **[Task]** **A safe staging area for testing** — A separate test environment loaded with May and June data lets the team validate reports without touching live information. (#270)
- **[Task]** **Confirming report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy system, to pin down the cause and confirm the numbers are accurate. (#271)
- **[Feature]** **Turning conversations into tracked work automatically** — An internal helper that reads team discussions and files them as tracked items, reducing manual follow-up. No visible change in the product. (#272)
- **[Task]** **Users screen feature review** — A documentation review comparing the Users area against the older system to identify anything still missing and prioritize it. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 70c57fa6f069885eca1042fa6bb276cea716c34265708264089a23e73462e681 -->
