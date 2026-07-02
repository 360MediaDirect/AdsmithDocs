# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 11:47:58 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" will finally open a proper date picker so you can set your own start and end dates, see the selected range on the filter button, and have the Dashboard update to match. (#58)
- **[Feature]** **Pick report dates without editing the web address** — You'll get date controls built right into the Dashboard toolbar, so you can pull a specific day or range with a click instead of typing into the address bar. Shareable links still update automatically. (#268)
- **[Task]** **Polish for the Dashboard header and tables** — The header will show the logo in place of the "Adsmith" text, long offer names will no longer be cut off, and table rows will get cleaner alternating shading for easier reading. (#283)
- **[Task]** **Separate table for update notes** — Update notes will get their own dedicated table instead of being mixed in with optimizations and general notes, so they're easier to spot. (#284)
- **[Task]** **Cleaner offer names on the Dashboard** — Offer names will drop the repetitive text before the first colon and show only the meaningful part, while names without a colon stay as they are. (#285)
- **[Feature]** **Export the day-by-day breakdown** — A high-priority addition: an export button on the breakdown-by-day view lets you download that data for use in a spreadsheet. (#286)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit it, the app will hold it for you and warn if someone else already has it open, so changes are never silently lost. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will get an Audit Log showing who changed what and when across offers, placements, advertisers and more, plus automated system changes, making it easy to answer "who changed this?" (#276)
- **[Feature]** **Bring back the Campaigns module** — A critical, high-priority addition to restore campaign management in New Adsmith Frontend, letting you create, edit, and configure campaigns and their offer groups just like the legacy system. (#200)
- **[Task]** **Closing the gaps in the Users area** — A review comparing the old and new Users screens to make sure important tools (like bulk actions and additional user details) carry over. Much of this is already underway. (#80)
- **[Bug]** **Clear error when testing a bad link** — Testing an invalid link will now show a proper failure message instead of quietly sending you back to the Dashboard. This fix is nearly complete. (#239)

## Survey

- **[Task]** **Show full survey images without cropping** — Survey images will be sized to fit so the whole image is visible instead of being cut off at the edges. (#287)
- **[Feature]** **Make design settings actually take effect** — A full check across every entity's design options to ensure the choices you make in the Design tab are truly reflected in the live survey, with any unused settings fixed. (#288)
- **[Bug]** **Connect the remaining survey styling controls** — Many Design-tab settings (colors, continue button, question text, header, legal text) are saved but don't yet change what visitors see. This work wires them through so your customizations really appear in the survey. (#290)

## Behind the Scenes

- **[Task]** **A safe staging area with May and June data** — Setting up a separate testing environment loaded with recent data so reports and features can be checked without touching live information. (#270)
- **[Task]** **Making report numbers match the legacy system** — Investigating why some Dashboard report figures differ from the old system so we can confirm the numbers are accurate and consistent. (#271)
- **[Feature]** **Automatic issue logging from team chats** — An internal helper that turns action items from team conversations into tracked tasks automatically, speeding up how requests get captured. (#272)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on Placements** — Follow-up improvements so new placements can default to your manual order and you can filter the available offers list by category, making offer selection faster. (#275)
- **[Feature]** **Preview placements and offers before saving** — A preview button on the placement and offer add/edit pages will let you see how things will look based on your current, unsaved entries. (#289)

## Reports

- **[Task]** **Sortable Offer Audit tables** — You'll be able to click column headers in the Offer Performance Audit to re-sort results by leads, conversions, or rates, making outliers easier to spot. (#281)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Cleaning up styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields display neatly and consistently, like the other forms. Partly done, with a careful final pass remaining. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 7cf2416479c6a006663477450a87c48f16726c5f92d204cab5941b3f0ca4624c -->
