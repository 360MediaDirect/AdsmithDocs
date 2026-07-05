# Open Issues — Plain-Language Overview

_Last updated 2026-07-05 13:31:21 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys
- **[Feature]** **Make every survey design setting actually work** — Today many of the customization options you set on a survey's design don't change what visitors see. This work makes sure each design choice flows all the way through to the live survey, and audits every form option across the product so nothing is left with no effect. (#288)
- **[Bug]** **Turn on the rest of the survey styling controls** — The Placement Design tab offers around 30 styling and behavior options (colors, buttons, answer styles, header, legal text), but only a couple currently reach the live survey. This fixes the remaining ones so your settings show up for visitors as expected. (#290)
- **[Feature]** **Finish the last few survey design settings** — A handful of design options left over from earlier work (iFrame height, display format, and a few behavior toggles) will either be made to work on the live survey or removed if they aren't needed, so nothing on the form is misleading. (#293)
- **[Bug]** **Show voucher codes and info links on the live survey** — For certain Data Clients, the configured custom question (like a voucher code) and the privacy/terms/details links aren't appearing on the survey page even though they're set up in the admin. This restores them to match how they showed in the old system. (#291)

## General / Across the App
- **[Feature]** **Prevent two people from overwriting each other's edits** — When two users open the same record, a warning and an editing lock will keep one person's changes from silently wiping out the other's, with a clear "locked by someone else" message so you know when to wait. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will get an Audit Log showing who changed what and when across offers, placements, and other records — including automated changes — making it much easier to answer "who changed this?" (#276)
- **[Feature]** **Clean up controls that don't do anything** — Some admin settings (like Advertiser Web Presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no real effect. These will be removed or hidden so the interface only shows controls that actually work. (#296)
- **[Task]** **Compare the old and new Users area** — A behind-the-scenes review of the Users section that lists what the legacy system offered versus the new one, so missing capabilities (like bulk actions and login/2FA details) can be prioritized and added. (#80)

## Placements & Offers
- **[Feature]** **Smarter offer ordering and filtering on Placements** — Building on recent drag-to-reorder work, new placements will default to Manual order so your arrangement is actually used, and you'll be able to filter the available offers list by category to find offers faster. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show the changes you're currently making, so you no longer have to save first just to see how an edit looks. (#292)
- **[Bug]** **Stop offer settings from getting lost before they reach visitors** — Several saved offer options (including Modal-tab fields and a few others) never make it to the live widget. Each will be wired up properly or clearly removed, so what you configure is what visitors get. (#295)

## Dashboard
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (for example to a spreadsheet) instead of only viewing it on screen. This is a high-priority addition. (#286)
- **[Task]** **Make sure new dashboard numbers match the old system** — An investigation into why some dashboard report totals differed from the legacy system, so we can confirm the numbers are accurate and consistent. (#271)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the product against realistic data for testing and verification, locked to read-only so testing can't accidentally change anything. (#270)
- **[Feature]** **Automatic issue-tracking from team chats** — A helper that reads team conversations and files action items automatically, reducing manual note-taking and follow-up. This won't change anything you see in the product. (#272)

## Modals
- **[Feature]** **Make the Modal Design tab do something** — Every field on the Modal Design tab is currently saved but has no effect on the modal visitors see. These will either be wired up to actually display or removed so the tab isn't misleading. (#294)

## Campaigns
- **[Feature]** **Bring back Campaigns in the new admin** — The Campaigns area from the old system isn't available yet in New Adsmith Frontend. This high-priority work adds it back so you can create, edit, and manage campaigns and their offer groups. (#200)

## Flows
- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned, with fields stacking oddly and elements like color pickers and text boxes looking out of place. This tidies up the layout to match other forms. (#152)

## Link Testing
- **[Bug]** **Show a clear error for invalid links** — Testing a bad link currently dumps you back on the dashboard with no explanation. Instead, you'll see a clear failure message so you know the link didn't work. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
