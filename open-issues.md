# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 23:27:44 UTC · 11 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range option that actually works** — When you choose "Custom" on the Dashboard's date filter, you'll get a proper start- and end-date picker with Apply and Cancel buttons, so you can view data for any range you like instead of only the preset options. (#58)
- **[Feature]** **Pick report dates right from the Dashboard** — You'll be able to choose a day or date range using controls built into the Dashboard toolbar, so you no longer have to edit the web address by hand to pull a specific day's report. Your selection still shows in the link so it stays easy to share. (#268)
- **[Task]** **Make sure report numbers match the old system** — We're checking the Dashboard report figures against the legacy system to find and explain any differences, so you can trust that the numbers you see are accurate and consistent. (#271)

## Behind the Scenes

- **[Task]** **A safe testing environment with real sample data** — We're setting up a separate practice environment loaded with May and June data so report checks can be done thoroughly without ever touching live information. (#270)
- **[Feature]** **Turn Slack chats into tracked work automatically** — We're building a helper that reads team conversations and files the resulting to-dos for us, so requests raised in discussion are captured reliably and nothing falls through the cracks. (#272)

## Campaigns

- **[Feature]** **Bring back the Campaigns area** — The Campaigns section from the older admin isn't in New Adsmith Frontend yet. This high-priority work will let you view, create, edit, and configure campaigns — including offer groups, offer handling, CTA text, and marketing partners — just as you could before. (#200)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on Placements** — Building on recent improvements to the offer list, new placements will default to your manually arranged order so the sequence you set is actually used, and you'll be able to filter the available offers by category to find what you need faster. (#275)

## Users

- **[Task]** **Closing the gaps in the Users area** — A detailed review compared the new Users screens against the older system and flagged missing pieces such as bulk actions (like changing several users' roles at once), select-all checkboxes, last-login and two-factor details, and a password field on the new-user form. This guides the work to bring Users up to full strength. (#80)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned, with fields stacking awkwardly instead of sitting side by side. This fix smartens up the form's appearance so it matches the polished look of the Placement and Modal forms. (#152)

## Link Testing

- **[Bug]** **Clear error when a tested link is invalid** — Right now, testing an invalid link quietly sends you to the Dashboard with no explanation. After this fix, you'll see a clear failure message so you know the link didn't work and why. (#239)

## General / Across the App

- **[Feature]** **A searchable history of who changed what** — A new platform-wide Audit Log will record every change to offers, placements, advertisers, modals, flows, properties, publishers, users, and more — including automated changes — along with who made it and when. Administrators will be able to search and filter this history and view a change history on each item's detail page, making it easy to answer "who changed this, and when?" (#276)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 18c895dd2d51d67625ab25b86c398b76285d058485c5365f84641d856758854b -->
