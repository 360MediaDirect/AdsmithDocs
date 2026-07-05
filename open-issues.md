# Open Issues — Plain-Language Overview

_Last updated 2026-07-05 19:29:54 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make Survey design settings actually change the survey** — Every customization option on the survey Design tab will carry through to what visitors see, and we're auditing all entity forms to make sure no setting is quietly ignored. (#288)
- **[Bug]** **Design-tab styling options that don't take effect yet** — Many survey styling and behavior settings (colors, continue button, header, legal text, and more) are saved but don't yet change the live survey. This work connects them so your choices are honored. (#290)
- **[Feature]** **Finish connecting the remaining survey design settings** — A handful of survey Design-tab options are still not fully hooked up; each will either be made to work in the live survey or removed so the form only shows options that actually do something. (#293)
- **[Bug]** **Voucher code and info links missing on the live survey** — A configured custom question (like a voucher code) and the privacy/terms/details links aren't showing on the new survey page even though they're saved. This restores them to match the legacy experience. (#291)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record you're already editing, you'll see a clear "locked by" notice, and you'll be warned before saving over a change someone else made in the meantime. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will get an audit log that records who changed what and when across the whole platform, including automated changes, making it easy to answer "who edited this?" (#276)
- **[Feature]** **Clean up controls that don't do anything** — Several admin settings currently save but have no real effect (for example, Advertiser Web Presence fields and some user-permission toggles). These will be removed or hidden so the screens only show controls that work. (#296)
- **[Bug]** **Clear error for an invalid test link** — When you test a bad link, you'll get a proper error message instead of being sent to the dashboard. (#239)

## Placements

- **[Feature]** **Better offer ordering and filtering on Placements** — New placements can default to your manual offer order (so drag-to-reorder is respected), and you'll be able to filter the available offers list by category. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show your current, in-progress edits instead of the last saved version, so you don't have to save first just to check your work. (#292)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button lets you download the breakdown-by-day data (for example, as a spreadsheet). This is a high-priority addition. (#286)
- **[Task]** **Confirm dashboard numbers match the legacy system** — We're investigating why some dashboard report figures differed from the old system so we can pin down the cause and ensure the numbers you see are accurate. (#271)

## Offers

- **[Bug]** **Make sure saved offer options reach the live widget** — Several saved offer settings (including Modal-tab fields and display options) currently don't make it to what visitors see. Each will be connected properly or removed if it's not needed. (#295)

## Modals

- **[Feature]** **Fix or remove the Modal Design tab** — All six fields on the Modal Design tab currently save but have no effect on the visitor-facing modal. They'll either be made to work or removed so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form don't look right yet — text boxes, color pickers, and paired fields don't display cleanly. This continues the cleanup so the form matches the polished look of other screens. (#152)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — The new platform doesn't yet have a Campaigns area. This adds the ability to view, create, edit, and configure campaigns and offer groups, matching the legacy system. This is a high-priority, core feature. (#200)

## Users

- **[Task]** **Review what's missing from the new Users area** — We're comparing the new Users screens against the old system to spot gaps (like bulk actions and extra columns) and plan what to add so nothing important is lost. (#80)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the app using production-like data for verification, locked to read-only so testing can't change real records. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — A helper that reads team chat and files the resulting to-dos as tracked issues, reducing manual note-taking and follow-up. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
