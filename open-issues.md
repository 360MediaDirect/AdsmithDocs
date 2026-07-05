# Open Issues — Plain-Language Overview

_Last updated 2026-07-05 11:31:42 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Bug]** **Publisher survey styling options that don't actually change anything** — Right now the survey widget only honors two of the roughly 30 design settings publishers can configure (colors, buttons, question text, headers, legal text, and more). This work connects the rest so the choices made in the Design tab actually show up for visitors, instead of quietly doing nothing. (#290)
- **[Feature]** **Finishing the remaining survey Design-tab settings** — A follow-up that wires up the last few survey styling and behavior options (such as widget height, display format, and skip/answer settings) so every option in the Design tab either works as expected or is removed if it's not needed. (#293)
- **[Bug]** **Missing voucher code and info links on live surveys** — For certain partners, the voucher code line and the privacy/terms/details links are set up in the admin but aren't appearing on the live survey page (they do show in the older system). This fixes that so visitors see the required voucher code and compliance links. (#291)
- **[Feature]** **Making sure design customizations reach the live survey** — A broader review to confirm every customization option across the app is fully connected from the setup screen all the way through to what visitors actually see, with any dead or disconnected options fixed or removed. (#288)

## General / Across the App

- **[Feature]** **Warning when two people edit the same record** — When two admins open the same offer, flow, placement, or other record, this prevents one person from accidentally overwriting the other's changes. You'll see a clear "locked by someone else" or "this was just changed — please reload" message instead of silently losing work. (#267)
- **[Feature]** **A searchable history of who changed what** — A new Audit Log will record every change to your entities (manual or automated) with a timestamp and who made it, and let administrators search and filter that history — making it easy to answer "who changed this and when." (#276)
- **[Feature]** **Cleaning up admin controls that do nothing** — Several settings currently appear in the admin but have no real effect (some Advertiser web-presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping options). These will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you back on the Dashboard with no explanation. After this fix, you'll get a clear failure message right in the Link Testing screen. (#239)

## Placements

- **[Feature]** **Better default ordering and filtering when picking offers** — On placements, the selected-offers list will default to manual order (so the order you set is actually used), and you'll be able to filter the available offers by category to find them faster. (#275)
- **[Feature]** **Preview reflects your unsaved edits** — On placement and offer edit screens, the Preview button will show your current in-progress changes rather than the last-saved version, so you can check your work without having to save first. (#292)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (for example as a spreadsheet) for your own reporting and analysis. (#286)
- **[Task]** **Checking dashboard report numbers against the old system** — An investigation into why some dashboard report figures didn't match the legacy system, so we can pinpoint any differences and confirm the numbers you see are accurate. (#271)

## Offers

- **[Bug]** **Saved offer options that never reach the live widget** — Several saved offer settings (including the offer's Modal-tab fields, Display URL, and some data-handling flags) aren't making it through to the live experience. This work ensures each of those either takes effect or is cleaned up if it's not needed. (#295)

## Modals

- **[Feature]** **Making the Modal Design tab work — or removing it** — Every field on the Modal Design tab (header title, subtitle, colors, progress bar, and more) is currently saved but has no visible effect. This will either connect those settings to what visitors see or remove the tab if it isn't needed. (#294)

## Campaigns

- **[Feature]** **Bringing back the Campaigns module** — The Campaigns area from the old admin isn't yet available in New Adsmith Frontend. This high-priority work rebuilds it so you can view, create, edit, and manage campaigns and their offer groups, matching the legacy workflow. (#200)

## Flows

- **[Task]** **Fixing the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned compared to the Placement and Modal forms (plain text boxes, unstyled color pickers, fields stacking oddly). This tidies up the layout so the form looks consistent and polished. (#152)

## Users

- **[Task]** **Comparing the old and new Users screens** — A review of the legacy Users management against the new one to spot missing pieces (such as bulk actions, extra columns, and filters) and prioritize what to add, so the new Users area matches what people relied on before. (#80)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the product using production-like data for verification and testing, locked to read-only so no real data can be changed. (#270)
- **[Feature]** **Turning Slack conversations into tracked to-dos** — An internal helper that reads designated Slack discussions and automatically files the action items as tracked work, reducing manual copy-and-paste when capturing follow-ups. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
