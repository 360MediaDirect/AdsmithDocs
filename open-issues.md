# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 11:35:45 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record to edit it, others will see it's already being worked on, and the system will warn you if a record changed while you had it open — so no one's changes get silently wiped out. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will be able to see who changed what and when across offers, placements, advertisers, and more — including automated changes — making it far easier to answer "who touched this?" (#276)
- **[Feature]** **Clean up controls that don't actually do anything** — Several admin settings (like the Advertiser Web Presence fields, certain user permission toggles, and a few Data Client and Pre-Ping options) currently save but have no effect. These will be removed or hidden so the screens only show controls that truly work. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you back on the Dashboard with no explanation. Once fixed, you'll get a clear failure message instead. (#239)
- **[Task]** **Users area review against the old system** — A documentation review comparing the old and new Users screens, so we can plan which missing pieces (like bulk actions and last-login info) to bring over. (#80)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent yet. We'll confirm whether anyone still needs it and either rebuild it or officially retire it. (#328)

## Offers

- **[Feature]** **Preview your unsaved changes** — On the Placement and Offer edit screens, Preview will show the edits you're currently making, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of offer options (including Modal-tab settings and a few delivery flags) are saved but never actually applied. We'll wire each one through or remove it so what you set is what visitors get. (#295)
- **[Task]** **Auto-register offers should respect visitor targeting** — Certain automatic offers currently fire for everyone, ignoring age, gender, state, ZIP, and device targeting. We'll make them honor those rules (or confirm this is intentional) so offers only show to the right people. (#333)
- **[Feature]** **Bring back the older per-client pre-ping option** — A pre-ping method from the legacy system isn't available in the new platform yet. We'll port it (or confirm the new pre-ping fully covers it) so no offer loses coverage. (#330)
- **[Feature]** **Automatic performance estimate for new offers** — Instead of a manual gut-check, new offers could get a data-driven projection of likely performance based on your historical offers — a helpful decision aid at intake. (#322)

## Surveys

- **[Bug]** **Most survey Design settings will actually work** — Right now only a couple of the roughly 30 Design-tab options (colors, buttons, header, legal text, and more) affect the live survey. This fix makes the rest take effect so what you configure is what visitors see. (#290)
- **[Feature]** **Finish connecting the remaining Design-tab settings** — A handful of survey styling and behavior settings (like widget height and display format) still need to be wired up or removed, so nothing on the Design tab is misleading. (#293)
- **[Bug]** **Voucher codes and info links will show on the live survey** — Custom questions (such as a voucher code) and the privacy/terms/details links configured for a Data Client aren't appearing on the survey page even though they're saved. This restores them to match the old app. (#291)
- **[Feature]** **Full audit that every design option is connected end-to-end** — A sweep across all entities to confirm each form option truly flows through from the screen to what visitors see, with any dead options fixed or documented. (#288)

## Behind the Scenes

- **[Task]** **A safe test environment using real-world data** — Setting up a read-only staging environment against a copy of production data, so the team can verify the new platform against realistic numbers without any risk of changing live data. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels and automatically files or updates work items from action items discussed — reducing manual note-shuffling. (#272)

## Campaigns

- **[Feature]** **Bring the Campaigns area into the new platform** — The Campaigns module from the old admin isn't in New Adsmith Frontend yet. This high-priority work adds the ability to view, create, edit, and configure campaigns and offer groups just like before. (#200)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or stack awkwardly instead of sitting side by side. This cleanup makes it match the polished look of the Placement and Modal forms. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — All six fields on the Modal Design tab currently have no effect. We'll either connect them to the visitor-facing modal or remove the tab so it isn't misleading. (#294)

## Data Clients

- **[Feature]** **Bring over post-conversion delivery steps** — Certain "after success" behaviors from the old system (delivery and redirect steps for specific clients) haven't been carried over. We'll rebuild the ones still needed or document any that are being retired. (#327)

## Reports

- **[Task]** **Confirm report numbers match the old system** — During testing, some Dashboard report figures didn't line up with the legacy app. We'll compare the same date range across both, pinpoint any differences, and either fix them or confirm the numbers are correct. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: db2e2e32afdf249c2931b9305c5b4e9f6e133e4b3e0fdf0fc98b37cd3f75c917 -->
