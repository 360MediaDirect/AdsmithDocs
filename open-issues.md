# Open Issues — Plain-Language Overview

_Last updated 2026-07-04 19:28:46 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Survey

- **[Feature]** **Make survey design settings actually change the survey** — Today many of the customization options on the Design tab are saved but don't affect what visitors see. This work confirms every design option is fully connected from the form through to the live survey, so what you set is what shows. (#288)
- **[Bug]** **Bring the rest of the survey Design-tab styling to life** — Only a couple of the roughly 30 survey styling and behavior settings (colors, buttons, header, question text, legal text, progress bar) currently reach the live widget. This connects the remaining ones so publishers' choices show up on the real survey page. (#290)
- **[Feature]** **Finish connecting the last few survey Design settings** — A handful of settings left over from earlier work (including survey height and question display format) still don't reach the widget. Each will either be made to work or removed from the form so nothing misleads you. (#293)
- **[Bug]** **Show voucher codes and info links on the live survey** — A custom question (like a voucher code) and the privacy/terms/details links configured for a data client aren't appearing on the new survey page, though they show in the legacy app. This restores them, which matters for both the visitor experience and compliance. (#291)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record, one could unknowingly wipe out the other's changes. This adds an editing lock and a save-time check so you'll see a clear "someone else is editing this" message instead of silently losing work. (#267)
- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every change to offers, placements, advertisers, and other records — including automated changes — with who did it and when. You'll be able to search this history and view it right from an entity's detail page. (#276)
- **[Feature]** **Clean up settings that don't do anything** — Several admin controls (an advertiser's Web Presence fields, some user permission toggles, and a few data-client and pre-ping options) are saved but have no effect. These will be removed, hidden, or properly built so the screens only show controls that actually work. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Right now, entering an invalid link in Link Testing quietly sends you to the dashboard. Once fixed, you'll get a clear failure message so you know the link didn't work. (#239)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (for example as a spreadsheet) for your own reporting. This is a high-priority addition. (#286)
- **[Task]** **Check that dashboard numbers match the legacy system** — Some dashboard report figures didn't line up with the older system during testing. This investigation pins down where the difference comes from and confirms the numbers can be trusted. (#271)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on placements** — Building on the recent drag-to-reorder work, this makes a manually set offer order actually take effect and adds a way to filter the available offers list by category, so it's faster to find and arrange the right offers. (#275)
- **[Feature]** **Preview your unsaved changes on placements and offers** — Today the Preview button shows the last saved version, so you have to save before you can see edits. This updates it to preview your current, in-progress changes without saving first. (#292)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — A separate environment mirrored on real-world data is being prepared for testing and verification, with safeguards that prevent any accidental changes to the data. (#270)
- **[Feature]** **Turn Slack conversations into tracked to-dos automatically** — An internal assistant will read designated Slack channels and file the action items as tracked work items, cutting out manual copy-and-paste. (#272)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — The Campaigns area from the legacy system isn't in the new platform yet, so campaigns and offer groups can't be managed here. This adds it back with the ability to view, create, edit, and configure campaigns. It's a high-priority, core feature. (#200)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned — plain textareas, unstyled color pickers, and paired fields stacking instead of sitting side by side. This tidies up the layout so it matches the polished look of the Placement and Modal forms. (#152)

## Offers

- **[Bug]** **Make sure saved offer options reach the live experience** — Several offer settings (including the Modal-tab fields, Display URL, and some data-client flags) are saved but never make it to the live widget. Each will be either connected end to end or clearly removed, so no setting silently does nothing. (#295)

## Modals

- **[Feature]** **Fix or remove the Modal Design tab** — All six fields on the Modal Design tab are currently saved but have no effect on what visitors see. They'll either be wired up to actually control the modal's header and progress bar, or removed if the modal is meant to be header-less. (#294)

## Users

- **[Task]** **Compare the Users area to the legacy system** — A review of the Users screens against the older system to spot missing features (like bulk actions, last-login and two-factor status, and password options) and prioritize what to add next. This is documentation and planning to guide upcoming improvements. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
