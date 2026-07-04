# Open Issues — Plain-Language Overview

_Last updated 2026-07-04 09:42:55 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make all survey design settings actually work** — Right now many of the customization options on the survey Design tab are saved but don't change what visitors see. This work confirms every option is fully connected from the settings screen through to the live survey, so nothing on the form is a dead end. (#288)
- **[Bug]** **Connect the remaining survey styling controls to the live widget** — Publishers can set roughly 30 survey styling and behavior options (colors, buttons, headers, legal text, and more), but today only a couple take effect. This fixes the rest so your configured look and behavior actually appear to visitors. (#290)
- **[Feature]** **Finish the last few survey Design-tab settings** — A follow-up that wires up the remaining survey settings (such as widget height and question display format) and cleans up any options that still do nothing, so the Design tab is fully trustworthy. (#293)
- **[Bug]** **Show voucher codes and info links on the live survey again** — For certain data clients, the voucher code line and the privacy/terms/details links are set up in the admin but don't appear on the live survey (they do in the old app). This restores them, which matters for both the visitor experience and compliance. (#291)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two users open the same record, one person's save could silently wipe out the other's changes. This adds a clear "someone else is editing this" indicator and a safeguard so nobody's work is lost. (#267)
- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every change across the platform — by whom, when, and what changed — including automated updates. Administrators will be able to search this history and see it from each record, making it far easier to answer "who changed this?" (#276)
- **[Feature]** **Clean up admin controls that don't do anything** — Some settings (like the Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) are shown but have no effect. These will be removed, hidden, or properly built so the admin only shows controls that actually work. (#296)
- **[Bug]** **Show a clear error for invalid links instead of the dashboard** — When testing a link that isn't valid, you're currently dropped onto the dashboard with no explanation. This will show a proper error message so you know the link failed. (#239)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example as a spreadsheet) for your own analysis and reporting. High priority. (#286)
- **[Task]** **Confirm dashboard report numbers match the legacy system** — During testing, some dashboard figures didn't line up with the old app. This investigation compares the two over the same dates to find and explain any differences, so you can trust the numbers. (#271)

## Placements

- **[Feature]** **Better offer ordering and filtering when building placements** — Builds on the recent drag-to-reorder work by making manual order the default (so your arrangement is actually used) and adding a way to filter the available offers list by category, making it easier to find the right offers. (#275)
- **[Feature]** **Preview your unsaved changes on placements and offers** — Today the Preview button shows the last saved version, so you have to save before you can see a change. This will let the preview reflect your current, unsaved edits. (#292)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging version of New Adsmith Frontend that uses production-like data but can't change anything, so the team can verify behavior without any risk to live data. (#270)
- **[Feature]** **Turn meeting notes into tracked work automatically** — An internal helper that reads team conversations and files the resulting to-dos automatically, reducing manual copy-and-paste and keeping the work list up to date. (#272)

## Offers

- **[Bug]** **Make sure saved offer settings reach the live widget** — Several saved offer options (including certain Modal-tab fields and display settings) aren't making it through to what visitors actually see. This ensures each saved field is either delivered and used, or cleaned up if it isn't needed. (#295)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — Every field on the Modal Design tab currently has no effect on the visitor-facing modal. This will either connect those fields (headers, progress bar, and text) so they display, or remove the tab if it isn't meant to be there. (#294)

## Flows

- **[Task]** **Fix the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned — plain textareas, unstyled color pickers, and paired fields stacking instead of sitting side by side. This tidies up the layout to match the other forms. Partly done, with the remaining polish being handled carefully to avoid new issues. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns area into New Adsmith Frontend** — The Campaigns management area from the older system isn't in the new platform yet. This adds it back so you can create, edit, and manage campaigns and their offer groups. A critical, high-priority addition. (#200)

## Admin / Users

- **[Task]** **Review what's missing from the new Users area** — A detailed comparison of the old and new Users screens to identify gaps (like bulk actions, extra columns, and filters) and prioritize what to add next, guiding upcoming improvements to user management. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
