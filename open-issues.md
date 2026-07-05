# Open Issues — Plain-Language Overview

_Last updated 2026-07-05 05:19:12 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Bring survey design settings fully to life** — Right now some customization options in the design tab don't actually change what visitors see. This work makes sure every design choice flows through to the live survey, and reviews options across all screens to catch any that aren't wired up. (#288)
- **[Bug]** **Survey styling options that currently do nothing** — Publishers can set around 30 look-and-feel options (colors, buttons, headers, legal text) on the Placement Design tab, but only a couple actually reach the live survey today. This fix makes the rest take effect so your settings are respected on the page visitors see. (#290)
- **[Bug]** **Voucher codes and info links missing on the live survey** — A custom voucher-code question and the privacy/terms/details links configured for a data client aren't showing on the new survey page, even though they appear in the older system. This restores them so visitors see the required voucher code and compliance links. (#291)
- **[Feature]** **Finish connecting the remaining Placement design settings** — A handful of design options are still saved but ignored (like survey height and display format). This completes the work so each option either changes the widget or is cleanly removed if unused. (#293)

## General / Across the App

- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you back on the dashboard with no explanation. After this fix, you'll get a clear failure message so you know the link didn't work. (#239)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record, one person's changes can silently wipe out the other's. This adds a gentle "someone else is editing this" lock and a save-time check, so your work is protected across every entity screen. (#267)
- **[Feature]** **A searchable history of every change** — This introduces a full audit trail that records who changed what and when, across offers, placements, advertisers, and more — plus an admin page to search and review that history. It makes troubleshooting "who changed this?" simple. (#276)
- **[Feature]** **Clean up controls that don't do anything** — Some admin fields (like Advertiser Web Presence, certain user permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no effect. These will be hidden or removed so the screens only show controls that actually work. (#296)

## Offers & Placements

- **[Feature]** **Better offer ordering and filtering on Placements** — Following earlier drag-and-drop improvements, this sets manual ordering as the default so your arranged order is actually used, and adds a way to filter the available offers list by vertical to find offers faster. (#275)
- **[Feature]** **Preview your unsaved changes** — Today the preview on placement and offer edit pages only shows the last saved version. This upgrade lets the preview reflect your current, unsaved edits, so you can check a change before committing to it. (#292)
- **[Bug]** **Saved offer options not reaching the live widget** — Several offer settings (including Modal-tab fields, Display URL, and Force More Info Visible) are saved but never make it to what visitors see. This ensures each of those options either takes effect or is cleanly retired. (#295)

## Dashboard

- **[Task]** **Confirm dashboard numbers match the older system** — Reviewers noticed report figures didn't line up with the legacy app. This investigation pins down where any differences come from and confirms the numbers are consistent, so you can trust the dashboard. (#271)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example as a spreadsheet) for your own analysis and sharing. High priority. (#286)

## Behind the Scenes

- **[Task]** **A safe, read-only testing environment** — Setting up a testing version of New Adsmith Frontend that runs against realistic data but can't change anything, so the team can verify behavior without any risk to live information. (#270)
- **[Feature]** **Automatically turn team conversations into tracked work** — A helper that reads discussion notes and files them as tracked to-dos automatically, reducing manual copying and helping make sure requests don't slip through the cracks. (#272)

## Campaigns

- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — Campaign management from the older admin system isn't available yet in the new platform. This adds it back, letting you view, create, and edit campaigns and manage offer groups. High priority. (#200)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned, with fields stacking oddly and pickers looking plain. This cleans up the layout so the Flow form looks polished and consistent with the other forms. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab actually work** — The Modal Design tab's settings (header text, colors, progress bar) are saved but currently have no effect on what visitors see. This work either wires them up so they take effect or removes them if the modal is meant to be header-free. (#294)

## Users

- **[Task]** **Review what's missing on the Users screen** — A comparison between the older Users area and the new one to identify gaps (like bulk actions and login/2FA details) and prioritize what to bring over, so the new Users experience is complete. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
