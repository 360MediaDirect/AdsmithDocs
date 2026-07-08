# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 01:34:17 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Legacy Feature Parity

- **[Feature]** **Bring the Campaigns module to the new platform** — Campaign management from the old system isn't available yet in New Adsmith Frontend. Once complete, you'll be able to view, create, edit, and configure campaigns and their offer groups just like the legacy admin. This is a high-priority gap. (#200)
- **[Feature]** **Restore legacy pre-ping behavior for older offers** — Some offers relied on a legacy pre-ping check that hasn't carried over. This work confirms which offers still need it and ensures they're fully covered so nothing is silently missed. A high-priority item. (#330)
- **[Feature]** **Carry over post-conversion delivery for Data Clients** — Certain "after success" behaviors (delivery and redirect steps that run once a lead converts) exist in the old system but not the new one. This restores those for the clients that still need them. (#327)
- **[Task]** **Compare the Users screen against the old system** — A review of the legacy Users area versus the new one to spot missing capabilities (like bulk role changes, last-login, and two-factor status) so the team knows what still needs building. (#80)
- **[Task]** **Decide the future of the legacy file-share page** — The old file-share page has no equivalent yet. This confirms whether anyone still uses it, then either rebuilds it or formally retires it. (#328)

## Surveys

- **[Bug]** **Make all survey design settings actually take effect** — Today the survey design options let you set around 30 styling and behavior choices (colors, buttons, header, legal text), but only a couple currently change what visitors see. This connects the rest so your customizations truly appear on the live survey. (#290)
- **[Bug]** **Show the voucher code and info links on the live survey** — For affected data clients, the voucher code line and the privacy/terms/details links are configured but aren't appearing to visitors, even though they show in the old system. This fixes that display gap. A high-priority fix. (#291)
- **[Feature]** **Confirm every design option is wired end to end** — A full audit to guarantee that each customization you set in the design tab is reflected in the survey visitors actually see, with no "dead" options that appear to work but don't. (#288)
- **[Feature]** **Finish connecting the remaining placement design settings** — A handful of placement design options (such as height and display format) still don't reach the live survey widget. Each will either be made to work or removed from the form so nothing is misleading. (#293)

## Offers

- **[Task]** **Apply visitor targeting to auto-register offers** — Auto-register offers currently skip the age, gender, state, ZIP, and device targeting rules that normal offers follow, so they can fire for visitors who should be excluded. This makes them respect the same targeting. A high-priority fix. (#333)
- **[Bug]** **Ensure saved offer settings reach live pages** — Several offer options are saved in the admin but never actually used by the live experience. Each will be connected so it works, or cleaned up if it's not needed, so the form reflects reality. (#295)
- **[Feature]** **Preview your unsaved offer and placement edits** — The Preview button will show the changes you're currently making, without forcing you to save first, for both offers and placements. (#292)
- **[Feature]** **Estimate how a new offer will perform** — Explore an automated, data-driven projection that uses your historical offer performance to forecast how a new offer is likely to do, replacing an informal manual gut-check. A helpful decision aid at offer intake. (#322)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record for editing, others will see it's locked and by whom, and the app will warn you if a record changed since you opened it — so no one's changes get silently lost. (#276 companion; see below) (#267)
- **[Feature]** **A searchable history of every change** — A new admin activity log that records who changed what and when, across offers, placements, advertisers, and more (including automated changes), making it easy to answer "who changed this and why." (#276)
- **[Feature]** **Remove settings that don't actually do anything** — Several admin controls (like the Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) are saved but have no effect. These will be hidden or removed so the admin only shows controls that truly work — important since some imply access controls that don't exist. (#296)
- **[Bug]** **Show a clear error when testing an invalid link** — Testing an invalid link currently drops you on the dashboard with no explanation. Instead you'll get a clear failure message right in the Link Testing screen. Nearly complete. (#239)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only testing environment** — Stand up a staging copy of the app using production-like data that can be reviewed without any risk of changing real records. (#270)
- **[Feature]** **Turn Slack conversations into tracked to-dos automatically** — A helper that reads designated Slack channels, picks out action items, and files or updates issues automatically, removing manual copy-and-paste from the team's workflow. (#272)

## Flows

- **[Task]** **Tidy up the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other forms, with some paired fields stacking awkwardly. This cleans up the layout for a consistent, polished look. (#152)

## Modals

- **[Feature]** **Make the Modal design settings work — or remove them** — The entire Modal design tab currently has no effect on what visitors see. Each setting will either be connected so it works or removed from the form to avoid confusion. (#294)

## Dashboard / Reports

- **[Task]** **Investigate why dashboard numbers differ from the old system** — During testing, some dashboard report figures didn't match the legacy app. This digs into where the difference comes from and either fixes it or confirms the numbers are correct, so you can trust the reports. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: db2e2e32afdf249c2931b9305c5b4e9f6e133e4b3e0fdf0fc98b37cd3f75c917 -->
