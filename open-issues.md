# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 19:30:30 UTC · 17 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a proper start-and-end date picker, so you can look at any specific span of dates instead of only the built-in presets like Today or This Month. (#58)
- **[Feature]** **Pick report dates without touching the web address** — You'll get easy date controls right in the dashboard toolbar, so pulling a single day's or a specific range's report no longer means editing the address bar by hand. Links will still stay shareable. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example to a spreadsheet) for your own analysis or record-keeping. (#286)

## Surveys

- **[Feature]** **Design choices actually show up in surveys** — Every styling and behavior option on the design tab will be carried all the way through to what visitors see, and we're checking every entity's form options to make sure none are just for show. (#288)
- **[Bug]** **The rest of the survey Design settings will take effect** — Many survey styling and behavior settings (colors, header, continue button, question text, legal text, and more) are saved today but don't change the live survey. This work makes those settings genuinely control what visitors see. (#290)
- **[Bug]** **Voucher code and info links missing on live surveys** — A configured voucher code line and the privacy/terms/details links aren't appearing on the new survey page even though they show in the legacy app. This fixes the display so both appear as expected. (#291)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else already has a record open, you'll see a clear "locked by" notice, and if a record changes while you're editing, you'll be prompted to reload instead of silently wiping out their work. (#267)
- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every create, update, delete, pause, and automated change across the product, so administrators can look up exactly who or what changed a record and when. (#276)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently just dumps you on the dashboard with no explanation; instead you'll get a clear failure message right in the Link Testing screen. (#239)

## Placements

- **[Feature]** **Better offer ordering and filtering on Placements** — New placements can default to your manual offer order (so the order you set is actually used), and you'll be able to filter the available offers list by category to find offers faster. (#275)
- **[Feature]** **Preview your unsaved edits on Placements and Offers** — The Preview button will show your current in-progress changes rather than the last saved version, so you can check how an edit looks before committing to a save. (#292)

## Behind the Scenes

- **[Task]** **A safe testing environment with May and June data** — A separate staging area loaded with recent data lets the team validate reports and test changes without ever touching live information. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — A helper that reads team chat and files the resulting to-dos as tracked issues, cutting out manual copy-and-paste when capturing action items. (#272)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form currently appear plain or misaligned (plain text boxes, unstyled color pickers, fields stacking instead of sitting side by side). This work tidies up the layout to match the other forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — Campaign management from the legacy system isn't available yet in the new platform. This adds the ability to view, create, edit, and configure campaigns and their offer groups, a core piece of everyday work. (#200)

## Reports

- **[Task]** **Confirm report numbers match the legacy system** — An investigation into why some dashboard report totals differed from the old app, so we can pinpoint any discrepancy, explain it, and confirm the numbers you rely on are accurate. (#271)

## Users

- **[Task]** **Closing the gap between the old and new Users area** — A review comparing the legacy Users screens with the new ones to identify missing capabilities (like bulk role changes, last-login and two-factor status, and password setup) so the new Users area can catch up. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d0231655be532926a4b9e2437541c81760c4fd1892085e7d3d8d4324bb87f4b7 -->
