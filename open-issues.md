# Open Issues — Plain-Language Overview

_Last updated 2026-07-04 17:23:12 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Match survey design options to what visitors actually see** — Every customization on a survey's Design tab will carry through to the live survey, and we're reviewing all entity forms to make sure no setting is a dead end. You'll be able to trust that the options you set take effect. (#288)
- **[Bug]** **Turn on the survey styling controls that don't yet do anything** — Roughly 30 look-and-feel settings (colors, buttons, answer styles, question text, header, legal text) are saved today but only two actually change the live survey. This fix connects the rest so your styling choices show up for visitors. (#290)
- **[Feature]** **Finish connecting the last few survey Design settings** — A follow-up to the styling work above, this ties in the remaining settings (like survey height and display format) and cleans up any options that still have no effect, either wiring them up or removing them. (#293)
- **[Bug]** **Restore missing voucher codes and info links on the live survey** — For affected data clients, the voucher-code line and the privacy/terms/details links are configured but not showing on the new survey page the way they did in the old system. This brings them back, which matters for passing leads and staying compliant. (#291)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit it, others will see it's locked and by whom, and you'll be warned if someone changed it while you had it open. This stops one person's save from silently wiping out another's work. (#267)
- **[Feature]** **A searchable history of who changed what** — Every manual and automated change to your records will be recorded with a timestamp and the person or system responsible, viewable in a new Audit Log and on each record's history. This makes it easy to answer "who changed this and when." (#276)
- **[Feature]** **Remove settings that don't actually do anything** — Some admin controls (Advertiser Web Presence fields, certain user permission and data-client options, a pre-ping setting) are saved but have no effect. These will be hidden or removed so the screens only show controls that truly work. (#296)
- **[Bug]** **Show a clear error when a tested link is invalid** — Testing an invalid link currently dumps you back on the Dashboard with no explanation. After this fix you'll see a proper error message instead. (#239)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example as a spreadsheet) for your own analysis. (#286)
- **[Task]** **Confirm dashboard numbers match the old system** — We're investigating why some dashboard report figures differed from the legacy system during testing, so you can rely on the numbers being accurate and consistent. (#271)

## Placements

- **[Feature]** **Better control over the offer list on Placements** — Building on the recent drag-to-reorder work, this makes manually arranged offers actually serve in that order by default and adds a filter so you can narrow the available offers by category. (#275)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — The Preview button will show your in-progress edits instead of only the last saved version, so you can check how a change looks without having to save first. (#292)

## Offers

- **[Bug]** **Stop losing offer settings before they reach the live widget** — Several saved offer options (including the Modal-tab fields and a number of backend flags) never make it to the live experience today. Each will be properly connected or cleaned up, so what you configure is what runs. (#295)

## Modals

- **[Feature]** **Make the Modal Design tab do something — or remove it** — All six fields on the Modal Design tab are saved but currently have no effect on the visitor-facing modal. They'll either be wired up to display or removed to avoid confusion. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or misaligned, with fields stacking oddly and controls like color pickers and text boxes not matching the rest of the app. This clean-up brings the Flow form in line with the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns area to the new platform** — The Campaigns module from the old admin isn't in New Adsmith Frontend yet. This adds it back so you can view, create, edit, and configure campaigns and their offer groups, matching the old workflow. (#200)

## Users

- **[Task]** **Review what's missing from the new Users area** — We're comparing the new Users screens against the old system to catch anything that hasn't carried over yet (such as bulk role changes and certain columns and filters), so upcoming work closes those gaps. (#80)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging version of New Adsmith Frontend against a copy of real data, locked to read-only, so changes can be verified against realistic information without any risk to live data. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — An internal Slack helper that reads discussions and files or updates work items automatically, reducing manual note-taking so requests are less likely to slip through the cracks. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
