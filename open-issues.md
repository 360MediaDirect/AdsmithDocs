# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 14:45:33 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker on the Dashboard** — Choosing "Custom" in the date filter will open a proper start-and-end-date picker so you can view Dashboard data for exactly the range you want, instead of only the preset options. (#58)
- **[Feature]** **Change report dates without editing the web address** — You'll get date controls right in the Dashboard toolbar to pull daily or custom-range reports, so you no longer have to hand-edit the URL. Shareable links still reflect your selection. (#268)
- **[Task]** **Confirming report numbers match the legacy system** — We're checking why some Dashboard report totals differ from the old system and pinpointing the cause, so you can trust the numbers you see. (#271)
- **[Task]** **Logo, offer-name width, and cleaner table rows** — The header will show the logo, long offer names will no longer be cut off, and table rows will get subtle alternating shading for easier reading. (#283)
- **[Task]** **Update notes in their own table** — Update notes will be split out from optimizations and general notes so they're easy to spot and don't get lost. (#284)
- **[Task]** **Cleaner offer names on the Dashboard** — Offer names will drop the repetitive text before the first colon, showing only the meaningful part. (#285)
- **[Feature]** **Export the breakdown-by-day view** — A new export button will let you download the day-level breakdown data (for example, to a spreadsheet). This is high priority. (#286)

## Survey

- **[Task]** **Survey images show in full** — Images in surveys will fit within their space and display completely instead of being cropped. (#287)
- **[Feature]** **Design settings that actually take effect** — We're making sure every design-tab option is reflected in the live survey and reviewing all entity forms so no setting is a dead end. (#288)
- **[Bug]** **Survey styling options now work end-to-end** — Many survey appearance settings (colors, buttons, header text, legal text, and more) were being saved but not applied to what visitors see. This fix connects those settings to the live survey widget. (#290)

## Behind the Scenes

- **[Task]** **Review of the Users area vs. the old system** — A documentation effort comparing the new Users area to the legacy version to flag missing capabilities (like bulk actions and login/2FA details) and prioritize what to build next. (#80)
- **[Task]** **A safe testing environment with May & June data** — Setting up a separate practice environment loaded with real historical data so testing and report checks can happen without touching live information. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — A Slack assistant that reads discussions and files or updates work items automatically, reducing manual copy-paste when capturing action items. (#272)

## General / Across the App

- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper error message instead of unexpectedly sending you to the Dashboard. (#239)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else is already editing a record, you'll see a clear "locked by" notice, and the app will warn you if a record changed since you opened it — protecting everyone's work from being silently overwritten. (#267)
- **[Feature]** **A searchable history of every change** — A new activity log will record who changed what and when across the platform (both manual and automated changes), with a searchable view and per-record history, making "who changed this?" easy to answer. (#276)

## Placements

- **[Feature]** **Better control over the offer list on placements** — Following up on earlier reordering work, we're looking at making new placements default to your manual offer order and adding a way to filter the available-offers list by category. (#275)
- **[Feature]** **Preview button for placements and offers** — You'll be able to preview how a placement or offer will look based on your current, unsaved changes before saving. (#289)

## Reports

- **[Task]** **Sortable Offer Audit tables** — The Offer Performance Audit breakdowns (sources, gender, age, states, email domains) will let you click column headers to sort, making it easier to spot outliers instead of being stuck on one fixed order. (#281)

## Flows

- **[Task]** **Consistent styling on the Flow form** — Cleaning up remaining visual issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields look polished and match the rest of the app. (#152)

## Campaigns

- **[Feature]** **Campaigns module coming to New Adsmith Frontend** — The Campaigns feature from the old system is being rebuilt so you can create, edit, and manage campaigns and offer groups directly in the new platform. This is a critical, high-priority addition. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f8abb2b365a088a6055638bcd665d24f8ba73e8997f377f6f92744d3ec2abfad -->
