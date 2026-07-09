# Open Issues — Plain-Language Overview

_Last updated 2026-07-09 20:34:37 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Feature]** **Bring campaign management into New Adsmith Frontend** — The Campaigns module from the older admin isn't in the new platform yet. Once added, you'll be able to view, create, edit, and configure campaigns (offer groups, offers, CTA text, and more) without going back to the legacy system. High priority. (#200)
- **[Bug]** **Conversion pixels now fire on success** — Success-tracking pixels set up on offers currently never fire, so conversions go unrecorded with no visible warning. This fix makes configured pixels fire as expected. High priority. (#297)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting and can fire for people they should exclude. This work makes them honor the same targeting rules as regular offers. High priority. (#333)
- **[Bug]** **Saved offer settings that weren't reaching the live offer** — Several options you can set on an offer weren't actually being carried through to the live experience. This fix ensures saved settings take effect (or are cleaned up if unused). (#295)
- **[Bug]** **bPerx voucher code missing from the offer preview** — On the preview page, the "Your Voucher Code" line isn't appearing the way it does in the legacy view. This fix restores the voucher code in preview and on the live survey. (#344)
- **[Feature]** **Preview your unsaved changes on placements and offers** — Today the Preview button only shows the last-saved version. This upgrade lets you preview edits you've made but not yet saved, so you can check changes before committing them. (#292)
- **[Feature]** **Automatic performance projection for new offers** — Instead of a manual gut-check, new offers could be scored against historical performance data to estimate how they're likely to do. Exploratory, no deadline. (#322)

## General / Across the App
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record for editing, others will see it's locked and by whom, and you'll be warned before accidentally saving over another person's changes. (#267)
- **[Feature]** **Searchable activity log** — A new admin log will record every change (manual or automated) with who did it and when, so you can answer "who changed this and when" and review history right from an entity's page. (#276)
- **[Feature]** **Clean up admin controls that don't actually do anything** — Some fields (like Advertiser Web Presence links, certain user-permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no effect. They'll be removed or hidden so the admin only shows controls that work. (#296)
- **[Task]** **Users area gap review** — A comparison of the older Users screen against the new one to spot missing capabilities (like bulk actions, last-login, and two-factor status) and plan what to add. Behind-the-scenes analysis. (#80)
- **[Task]** **Decide the future of the file-share page** — The legacy file-share page has no equivalent yet; this confirms whether it's still needed or can be retired. (#328)
- **[Task]** **Consistent alert and banner colors** — Warning, info, success, and error banners currently look slightly different from page to page. This standardizes their colors so they look the same everywhere. (#341)

## Survey & Modals
- **[Bug]** **Voucher code and info links missing on the live survey page** — Configured voucher codes and the privacy/terms/details links aren't showing on the new survey page even though they're saved. This fix restores them, matching the legacy display. High priority. (#291)
- **[Feature]** **Design choices fully reflected in the survey** — An end-to-end check to make sure every design-tab option you set actually shows up in the survey, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A few Placement Design-tab settings (like survey height and display format) are saved but not yet applied. This wires them up so they take effect (or removes any that aren't needed). (#293)
- **[Feature]** **Make the Modal Design tab work or remove it** — The Modal Design tab's fields are currently saved but never shown to visitors. This either builds them into the modal or removes the tab so it isn't misleading. (#294)

## Pre-Pings / Data Clients
- **[Feature]** **Port legacy per-client pre-ping checks** — Custom serve-time validation for 448 data clients isn't running on the new platform yet. This work restores those checks so offers are validated as they were in the legacy system. High priority. (#338)
- **[Feature]** **Display-trigger pre-ping runs a real check at serve time** — Currently this trigger only checks that fields exist rather than performing the actual validation. This makes it truly validate and hide offers that are rejected, matching legacy behavior. High priority. (#337)
- **[Feature]** **Restore after-success delivery for data clients** — Post-conversion delivery/redirect behavior from the legacy system hasn't been carried over. This brings it back as a configurable option for the affected clients. (#327)

## Reports & Dashboard
- **[Task]** **Investigate report numbers not matching the legacy system** — Dashboard report figures didn't line up with the old app during testing. This digs into where the difference comes from and confirms the numbers are trustworthy. (#271)
- **[Feature]** **Fix placement offer impressions showing zero** — Historical placement reports currently show zero offer impressions. This adds that figure so reports show real numbers. (#339)

## Flows
- **[Task]** **Fix the appearance of the Flow form** — Parts of the Flow form look unstyled or broken (plain text boxes, unstyled color pickers, fields stacking instead of sitting side by side). This tidies up the layout to match the other forms. (#152)

## Behind the Scenes
- **[Task]** **A safe testing environment using real-like data** — Setting up a staging version of the product connected to a read-only copy of production data, so testing can happen against realistic data without any risk of changing it. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A Slack helper that reads discussions and files the action items as tracked tasks, reducing manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d828ce4664fc9cba1564cd2695994a77b840ef6c24e2f97a6adfd64aeb2b6b7f -->
