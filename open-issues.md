# Open Issues — Plain-Language Overview

_Last updated 2026-07-06 18:39:37 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Warn when two people edit the same record** — When someone opens a record you're already editing, the app will keep your changes from being silently overwritten and will show a clear "locked by" or "reload" message. This prevents lost edits across all entity screens. (#267)
- **[Feature]** **Full history of who changed what** — A new searchable Audit Log will record every manual and automated change to your entities (offers, placements, advertisers, and more), so you can always see who changed something and when, right down to per-record history. (#276)
- **[Feature]** **Clean up controls that don't do anything** — Several settings that look active but have no effect (Advertiser Web Presence links, certain user-permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Bug]** **Invalid links now show a real error** — When you test a link that isn't valid, you'll get a clear failure message instead of being unexpectedly sent to the dashboard. (#239)
- **[Task]** **Review of the Users area vs. the old system** — A documentation review comparing the new Users screens to the legacy version, identifying gaps like bulk actions, last-login, and 2FA status so future updates can close them. (#80)

## Surveys

- **[Feature]** **Make every design option actually work** — An across-the-board check to ensure each customization on the Design tab is reflected on the live survey, so nothing you set is quietly ignored. (#288)
- **[Bug]** **Connect the remaining survey styling options** — Many Design-tab settings (colors, continue button, question text, header, legal text) are saved but don't yet change what visitors see; this work makes them take effect on the live survey. (#290)
- **[Feature]** **Finish wiring the last few survey settings** — Follow-up work to connect the remaining Design-tab options (like survey height and display format) or remove any that aren't needed, so nothing on the form is misleading. (#293)
- **[Bug]** **Voucher codes and info links missing on live surveys** — Custom questions (such as a voucher code) and privacy/terms/details links are set up in the admin but not showing on the live survey; this restores them to match the older app. High priority, as these affect compliance and lead handling. (#291)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button lets you download the breakdown-by-day data (for example to a spreadsheet). High priority. (#286)
- **[Bug]** **Offer Detail fails on "Last Month"** — The Offer Detail page currently times out and shows a load error when filtered to "Last Month"; this fix lets that date range load normally. (#318)
- **[Task]** **Check dashboard numbers against the old system** — An investigation into why some dashboard report figures differ from the legacy app, to pinpoint the cause and confirm the numbers can be trusted. (#271)

## Placements

- **[Feature]** **Better offer ordering and filtering on placements** — Follow-up work so new placements can default to your manual offer order (instead of random) and so you can filter the available offers list by category. (#275)
- **[Feature]** **Preview your unsaved changes** — On placement and offer edit pages, the Preview button will show your current, unsaved edits instead of the last-saved version, so you don't have to save just to see how a change looks. (#292)

## Offers

- **[Bug]** **Some saved offer settings never reach the live page** — A number of saved offer options (including Modal-tab fields and several backend flags) currently get dropped before they display; this ensures each one is either shown where expected or clearly removed. (#295)

## Modals

- **[Feature]** **Fix or remove the Modal Design tab** — All six fields on the Modal Design tab are currently saved but have no effect on what visitors see; this work will make them display properly or remove the tab if it isn't needed. (#294)

## Campaigns

- **[Feature]** **Bring the Campaigns area to the new platform** — The Campaigns module from the old admin isn't in the new one yet. This adds the ability to view, create, edit, and configure campaigns and offer groups. Critical, high priority, since campaign management is a core task. (#200)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or awkwardly laid out compared to other forms; this cleanup gives it consistent, polished styling. Partly done already. (#152)

## Behind the Scenes

- **[Task]** **Staging environment for safe testing** — Setting up a read-only test environment that mirrors real data, so the team can verify the product against realistic information without risk of changing anything. (#270)
- **[Feature]** **Turn conversations into tracked work items** — An internal helper that reads team discussions and automatically files them as issues, reducing manual note-taking and follow-up. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6c27af732f3641fd9b535e157afcb427a79ad241cf9415444c675c49de3c7588 -->
