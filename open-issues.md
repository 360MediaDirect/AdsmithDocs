# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 09:48:26 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's changes** — When you and a colleague have the same record open, New Adsmith Frontend will warn you and prevent one person's save from silently wiping out the other's edits. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will be able to see who changed what and when across offers, placements, and other records, with a filterable log and per-record history — making "who touched this?" easy to answer. (#276)
- **[Feature]** **Clean-up of settings that do nothing** — Several admin controls (an Advertiser Web Presence tab, some user permission toggles, and a few Data Client and Pre-Ping fields) currently save but have no effect. They'll be hidden or removed so the screens only show controls that actually work. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Entering an invalid link during Link Testing currently dumps you back on the Dashboard. This fix (nearly done) will show a proper failure message instead. (#239)

## Surveys

- **[Feature]** **Design choices that actually show up in the survey** — Every customization option on the Design tab will be reflected in what visitors see, and all entity forms will be checked so no setting is left disconnected. (#288)
- **[Bug]** **Survey styling settings that currently do nothing will start working** — Around 30 Design-tab options (colors, continue button, headers, question text, legal text) are saved today but never reach the live survey widget. This connects them so your choices take effect. (#290)
- **[Bug]** **Voucher code and info links restored on the live survey** — A configured voucher code line and the privacy/terms/details links aren't showing on the new survey page even though they're set in the admin. This brings them back to match the old system. (#291)
- **[Feature]** **Finishing the remaining Design-tab settings** — A handful of leftover survey settings will either be wired up to the live widget or removed from the form so nothing misleading remains. (#293)

## Offers & Placements

- **[Bug]** **Saved offer options that never reached the live page** — Several offer settings are saved but dropped before they reach visitors. Each will be either connected so it works or cleaned up if it's no longer needed. (#295)
- **[Feature]** **Preview your unsaved edits** — The Preview button on Placement and Offer edit pages will show your current, in-progress changes instead of only the last saved version, so you can check your work before saving. (#292)
- **[Task]** **Auto-register offers will respect visitor targeting** — Certain auto-firing offers currently ignore age, gender, state, zip, and device targeting. This ensures they only fire for the visitors they're meant for. (#333)
- **[Feature]** **Automatic performance estimate for new offers** — Instead of a manual gut-check, new offers could get a data-driven projection of likely performance based on your historical offer data, helping you judge them at intake. (#322)

## Bringing Legacy Features Across

- **[Feature]** **The Campaigns module is coming** — A high-priority gap: you'll be able to view, create, edit, and configure campaigns and offer groups in New Adsmith Frontend, just as you can in the old admin. (#200)
- **[Feature]** **Post-conversion delivery steps brought over** — The old system's "after success" client delivery/redirect behavior will be reviewed and either rebuilt for the affected clients or documented as retired. (#327)
- **[Task]** **Deciding the future of the old file-share page** — This legacy page has no equivalent yet; the team will confirm whether it's still needed and rebuild or retire it accordingly. (#328)
- **[Feature]** **Legacy pre-ping checks brought over** — A high-priority gap where older per-client pre-ping behavior isn't yet covered in the new platform. This ensures offers relying on it keep working. (#330)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging version of New Adsmith Frontend that mirrors real production data for verification, with writes blocked so testing can't affect live records. (#270)
- **[Feature]** **Turning conversations into tracked tasks automatically** — An internal helper that reads team conversations and files or updates work items, cutting out manual copy-and-paste. (#272)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned compared to other forms. This work makes sections, text boxes, color pickers, and paired fields display consistently. (#152)

## Reports & Dashboard

- **[Task]** **Making sure report numbers match the old system** — Testing found Dashboard report figures didn't line up with the legacy app. This investigation pins down where the difference comes from and confirms the numbers can be trusted. (#271)

## Admin & Users

- **[Task]** **Comparing the old and new Users area to close gaps** — A documentation review of what the Users screen offered before versus now, flagging missing pieces like bulk actions, last-login, and 2FA status so they can be prioritized. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: db2e2e32afdf249c2931b9305c5b4e9f6e133e4b3e0fdf0fc98b37cd3f75c917 -->
