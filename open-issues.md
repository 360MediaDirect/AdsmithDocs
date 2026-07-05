# Open Issues — Plain-Language Overview

_Last updated 2026-07-05 23:23:17 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make every survey design option actually take effect** — We're reviewing all the customization options across the product to confirm each one is truly connected from the settings screen through to what visitors see, so nothing you set is quietly ignored. (#288)
- **[Bug]** **Connect the rest of the survey Design-tab settings to the live survey** — Today only a couple of the roughly 30 styling and behavior options (like the "does not qualify" text) actually change the live survey; the rest are saved but have no visible effect. This work makes colors, buttons, headers, question text, and legal text work as the screen implies. (#290)
- **[Bug]** **Show voucher codes and info links on the live survey** — For affected offers, the custom voucher-code line and the privacy/terms/details links are configured but don't appear on the live survey the way they do in the old system. This restores them, which matters for both the user experience and compliance. (#291)
- **[Feature]** **Finish wiring the remaining Placement design settings** — A handful of leftover survey design settings (such as height and display format) still don't reach the live widget. Each will be either made to work or removed so nothing on the screen is misleading. (#293)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record at once, you'll be warned instead of silently saving over someone else's changes, and a record being edited by someone else will clearly show who has it open. (#267)
- **[Feature]** **A searchable activity log of every change** — Administrators will be able to see who changed what and when across offers, placements, advertisers, and more — including automated changes — making it easy to answer "who changed this?" (#276)
- **[Feature]** **Remove controls that don't do anything** — Several admin fields (like the Advertiser Web Presence tab and some user-permission toggles) are saved but have no effect. They'll be hidden or removed so the interface only shows controls that actually work. (#296)
- **[Bug]** **Show a clear error for invalid links instead of bouncing to the Dashboard** — When you test a link that isn't valid, you'll get a proper failure message right where you're testing, rather than being unexpectedly sent to the Dashboard. (#239)

## Dashboard

- **[Task]** **Confirm Dashboard report numbers match the old system** — We're investigating why some Dashboard figures didn't line up with the legacy app during testing, so you can trust the numbers are consistent. (#271)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example, to a spreadsheet) instead of only viewing it on screen. This is a high-priority addition. (#286)

## Placements

- **[Feature]** **Better default sorting and offer filtering when building placements** — New placements would default to your manual offer order (so the order you arrange is actually used), and you'll be able to filter the available offers by category to find them faster. (#275)
- **[Feature]** **Preview your unsaved changes** — On placement and offer edit screens, Preview will reflect your current edits instead of only the last saved version, so you can check a change before committing it. (#292)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging environment that mirrors real data but can't be changed, so the team can verify the product against realistic information without any risk to live data. (#270)
- **[Feature]** **Turn conversations into tracked to-dos automatically** — A helper that reads team chat discussions and files the resulting action items for the team, reducing manual note-taking and follow-up. (#272)

## Flows

- **[Task]** **Fix the appearance of the Flow form** — Parts of the Flow form currently look unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacked instead of side by side). This tidies up the layout to match the other forms. (#152)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — The new platform doesn't yet have the Campaigns area found in the old admin. This adds the ability to view, create, edit, and configure campaigns and their offer groups. It's a high-priority, core capability. (#200)

## Offers

- **[Bug]** **Make sure saved offer settings reach the live experience** — Several saved offer options currently get lost before they appear on the live widget. Each will be either connected through so it works or clearly retired if it isn't needed. (#295)

## Modals

- **[Feature]** **Make the Modal Design tab do something — or remove it** — Every field on the Modal Design tab is saved but has no effect on what visitors see. Each will be either made to work or removed so the tab isn't misleading. (#294)

## Users

- **[Task]** **Review what's missing in the new Users area** — A comparison of the old and new Users management screens to identify gaps (like bulk actions and login/2FA details) and prioritize what to bring over. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
