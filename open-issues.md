# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 17:31:50 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against two people editing the same record** — When two admins open the same record at once, New Adsmith Frontend will warn you and stop one person's changes from silently wiping out the other's. A high-priority safeguard against lost edits. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will let administrators see who changed what and when — across offers, placements, advertisers, and more — including automated changes, so troubleshooting "who touched this?" becomes easy. (#276)
- **[Feature]** **Clean up settings that don't actually do anything** — Several admin controls (parts of Advertiser Web Presence, some user permissions, and a few Data Client and Pre-Ping options) currently look editable but have no effect. They'll be removed or hidden so the screens only show controls that truly work. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Instead of being dropped back on the Dashboard, you'll get a proper failure message when a link test doesn't pass. Nearly finished. (#239)
- **[Task]** **Review of the Users area against the old system** — A side-by-side check of the old and new Users screens to catch missing features (like bulk actions, two-factor status, and last-login info) so nothing important is left behind. (#80)
- **[Task]** **Decide the future of the old file-share page** — Confirm whether the legacy file-share page is still used and either rebuild it in the new admin or formally retire it. (#328)

## Surveys

- **[Bug]** **Make survey Design settings actually take effect** — Many Design-tab options (colors, buttons, question text, header, and more) are saved today but never change what visitors see. This wires them through so your styling choices show up on the live survey. Nearly finished. (#290)
- **[Feature]** **Finish the remaining survey Design settings** — The last few Design-tab options (such as widget height and question display format) will either start working or be removed if they're no longer needed, so nothing on the tab is a dead end. (#293)
- **[Feature]** **Confirm every design option works from start to finish** — A thorough check across the product to ensure each customization you set is reflected in the live survey, with any non-working options fixed or cleared out. (#288)
- **[Bug]** **Voucher code and info links missing on the live survey** — The voucher code line and the privacy/terms/details links are configured but not showing on the new survey page. They'll display again as they did before — important for both the visitor experience and compliance. High priority. (#291)

## Offers

- **[Bug]** **Saved offer options that never reach visitors** — Some offer settings (including Modal options and Display URL) are saved but dropped before the live experience loads. Each will be properly connected or tidied up so what you configure is what visitors get. (#295)
- **[Feature]** **Preview your unsaved changes** — The Preview button on Offer and Placement edit screens will show your current edits without forcing you to save first, so you can check your work as you go. (#292)
- **[Task]** **Auto-register offers should respect visitor targeting** — These offers currently fire regardless of age, gender, state, ZIP, or device rules. This confirms and corrects that behavior so they only show for the right visitors. High priority. (#333)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical offer data, replacing the old manual gut-check review. (#322)

## Behind the Scenes

- **[Task]** **A safe, read-only testing environment** — A staging setup using production-like data for verification and testing, with safeguards so it can only read data, never change it. Nearly finished. (#270)
- **[Feature]** **A Slack helper that turns conversations into tracked tasks** — An internal tool to capture action items from Slack and file them automatically, cutting out manual copy-and-paste. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — All six Design-tab fields for modals (header title/subtitle, colors, progress bar) currently have no effect. They'll either be connected to the visitor modal or removed so the tab isn't misleading. (#294)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behaviors** — The legacy "after-success" behaviors that run once a visitor converts haven't been carried over yet. They'll return as a configurable option so affected clients keep working as before. Nearly finished. (#327)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unfinished (plain textareas, unstyled color pickers, and fields that stack instead of sitting side by side). This tidies up the layout to match the other forms. (#152)

## Campaigns

- **[Feature]** **Bring back the Campaigns area** — Campaign management exists in the old system but isn't in New Adsmith Frontend yet. This adds the ability to view, create, edit, and configure campaigns and offer groups. A critical, high-priority gap. (#200)

## Reports

- **[Task]** **Investigate mismatched Dashboard report numbers** — Testing found the new Dashboard figures didn't match the old system. This digs into where the difference comes from and confirms the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: c82faaa1fe39ccba682c940053c6ade31550c238f2b2a648582c71c424468a53 -->
