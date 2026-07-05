# Open Issues — Plain-Language Overview

_Last updated 2026-07-05 01:34:30 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Surveys

- **[Feature]** **Make Design-tab choices actually change the survey** — Options you set on a survey's Design tab will be carried all the way through to what visitors see, and we'll check every entity's form options to make sure none are decorative-only. You'll be able to trust that the settings you pick take effect. (#288)
- **[Bug]** **Survey styling settings that don't do anything** — Around 30 look-and-behavior settings (colors, continue button, answer style, header, legal text) are saved today but never reach the live survey. This work wires them up so your customizations finally show on the page. (#290)
- **[Feature]** **Finish connecting the remaining survey Design settings** — A handful of survey settings left over from the earlier fix (such as survey height and display format) will either start working on the live widget or be removed if they're not needed, so nothing in the form is misleading. (#293)
- **[Bug]** **Missing voucher code and info links on live surveys** — A configured voucher-code question and the privacy/terms/details links aren't appearing on the new survey page even though they show in the old system. This restores both, which matter for passing leads and for compliance. (#291)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else is already editing a record, you'll see a clear "locked by" notice, and if a record changes while you had it open you'll be prompted to reload instead of accidentally wiping out their changes. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when across offers, placements, advertisers and more, including automated changes, so you can finally answer "who changed this?" and troubleshoot with confidence. (#276)
- **[Feature]** **Remove controls that don't actually do anything** — Several admin settings (like the Advertiser Web Presence fields, some user-permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no effect. They'll be hidden or removed so the screens only show controls that truly work. (#296)
- **[Bug]** **Testing an invalid link now shows a clear error** — Entering a bad link currently bounces you to the dashboard with no explanation. Instead you'll get a clear failure message so you know the link didn't pass. (#239)

## Placements & Offers

- **[Feature]** **Better control over the offer list on placements** — You'll be able to set new placements to use your manual offer order by default and filter the available-offers list by category, making it much faster to build the right offer lineup. (#275)
- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will show your current, in-progress edits rather than only the last saved version, so you can check changes before committing them. (#292)
- **[Bug]** **Some saved offer settings never reach the live page** — A number of offer options (including Modal-tab fields and several data-client flags) are saved but dropped before the live widget sees them. Each will be wired through or cleaned up so what you save is what runs. (#295)

## Dashboard

- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view lets you download that data (for example to a spreadsheet) for your own reporting and analysis. (#286)
- **[Task]** **Confirm dashboard numbers match the old system** — We're investigating why some dashboard report figures didn't line up with the legacy app, so we can pin down the cause and make sure the numbers you rely on are accurate. (#271)

## Behind the Scenes

- **[Task]** **A safe test environment using real-world data** — Setting up a read-only staging copy so the team can verify the product against production-like data without any risk of changing it. (#270)
- **[Feature]** **Turn meeting notes into tracked to-dos automatically** — An internal helper will read team conversations and file follow-up items for us, so requests are captured consistently and nothing slips through the cracks. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab meaningful** — Every field on the Modal Design tab is currently saved but ignored by the visitor modal. Each will either be made to work or removed, so the tab reflects reality. (#294)

## Campaigns

- **[Feature]** **Bring Campaigns into the new platform** — The Campaigns area from the old admin isn't available yet in New Adsmith Frontend. This adds it back so you can create, edit, and manage campaigns and their offer groups. High priority. (#200)

## Admin & Users

- **[Task]** **Closing the gaps in the Users area** — We're reviewing the old Users management against the new one to catch missing capabilities (like bulk actions and extra columns) and plan what to add, so the new Users area is as complete as the one it replaces. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 827fd33e19c2697dfbf133ab2ab5daf8bb780f98984318723fe9f847403fc4dc -->
