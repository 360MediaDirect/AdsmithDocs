# Open Issues — Plain-Language Overview

_Last updated 2026-07-04 03:02:56 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit it, the system will hold it for you so another user can't unknowingly save over your changes. If someone else already has it open, you'll see a clear "Locked by [name]" note, and you'll be warned if a record changed while you had it open. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when — across offers, placements, advertisers, modals, flows, and more — including automatic system changes. You'll be able to search by record, person, action, or date, and see a history on each record's page, making it easy to answer "who changed this?" (#276)
- **[Feature]** **Clean up buttons and options that don't actually do anything** — Some admin controls (such as the Advertiser Web Presence fields, certain user permission toggles, and a few Data Client and Pre-Ping options) are saved but have no effect. These will be removed or hidden so the screens only show settings that truly work. (#296)
- **[Bug]** **Invalid links should show an error, not send you to the Dashboard** — When you test a bad link, you'll get a clear failure message right in the Link Testing area instead of being unexpectedly dropped onto the Dashboard. (#239)
- **[Task]** **Review of the Users area against the old system** — A behind-the-scenes comparison of the new Users screens against the legacy version to spot missing pieces (like bulk actions, last-login and two-factor details, and password/notification options) and prioritize what to add next. (#80)

## Surveys

- **[Feature]** **Make sure every Design tab setting actually changes the survey** — A full review across all entity forms to confirm each customization option truly flows through from the form to what visitors see, fixing or removing any option that currently does nothing. (#288)
- **[Bug]** **Design settings that don't reach the live survey widget** — Publishers configure roughly 30 look-and-feel settings (colors, buttons, headers, legal text, and more), but only a couple currently affect the live survey. This work connects the rest so your styling choices actually appear to visitors. (#290)
- **[Feature]** **Finish connecting the last few survey Design settings** — Wraps up the remaining styling options (such as widget height and question display format) so they take effect on the live survey, and cleans up any that won't be used. (#293)
- **[Bug]** **Voucher code and info links missing on the live survey page** — Custom questions (like a voucher code) and the privacy/terms/details links set up in the admin will once again show on the survey page, matching the old system. These are important for passing leads and staying compliant. (#291)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (for example, to a spreadsheet) for your own reporting and analysis. (#286)
- **[Task]** **Confirm dashboard report numbers match the old system** — An investigation into why some dashboard report figures differed from the legacy app, so we can pinpoint the cause and make sure the numbers you see are accurate and trustworthy. (#271)

## Placements

- **[Feature]** **Better control over the offers in a placement** — Follow-up improvements to the offer selection list: making manually arranged offer order actually take effect, and adding a way to filter the available offers by vertical so the right offers are easier to find. (#275)
- **[Feature]** **Preview your unsaved changes on Placements and Offers** — The Preview button will show the edits you're currently making, so you no longer have to save first just to see how a change looks. (#292)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the product using production-like data for testing and verification, locked to read-only so nothing there can be accidentally changed. (#270)
- **[Feature]** **Turn conversations into tracked to-dos automatically** — An internal helper that reads team discussions and files the resulting action items for us, so requests and issues are captured without manual copy-paste. (#272)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Fixing styling gaps so the Flow form's text boxes, color pickers, checkboxes, and paired fields display neatly and consistently, matching the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bring back the Campaigns area** — A high-priority addition of the Campaigns module so you can view, create, edit, and configure campaigns and offer groups in the new platform, just as you could in the old admin system. (#200)

## Offers

- **[Bug]** **Some saved Offer settings never reach the live widget** — Certain offer options (including several modal-related fields and display settings) are saved but aren't being carried through to what visitors see. This fixes the gap so saved settings take effect, and removes any options that aren't actually used. (#295)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The Modal Design tab's settings currently have no effect on the modal visitors see. This work either connects those settings so they display properly or removes the tab if it isn't needed. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
