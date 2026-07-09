# Open Issues — Plain-Language Overview

_Last updated 2026-07-09 17:38:10 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Admin & General

- **[Task]** **Bring the Users area up to par with the old system** — A review comparing the old and new user-management screens is underway to close gaps, so features like bulk role changes, last-login, and two-factor status eventually return. (#80)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else already has a record open, you'll see who's editing it and be blocked from accidentally saving over their changes. This safeguard will apply across every editable screen. (#267)
- **[Feature]** **Remove settings that don't actually do anything** — Certain controls (like the Advertiser Web Presence tab and some user-permission and data-client options) currently have no effect. They'll be removed or hidden so screens only show options that truly work. (#296)
- **[Bug]** **Clear error when testing an invalid link** — Instead of being bounced to the Dashboard, you'll now get a proper failure message when a tested link is invalid. This is a nearly-finished fix. (#239)
- **[Task]** **Decide the future of the legacy file-share page** — A quick review to confirm whether the old file-share page is still needed or can be retired. (#328)
- **[Task]** **Consistent look for alerts and banners** — Warning, info, success, and error banners will render the same way on every screen instead of drifting slightly from page to page. (#341)

## Offers

- **[Feature]** **Preview your unsaved changes** — On Placements and Offers, the Preview button will show your current in-progress edits instead of only the last saved version, so you can check changes before committing them. (#292)
- **[Feature]** **Automatic performance projections for new offers** — New offers could get a data-driven estimate of how they're likely to perform, based on your historical offer data, replacing today's manual gut-check. (#322)
- **[Bug]** **Auto-register offers should respect targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting and can fire for visitors they should exclude. This high-priority fix makes them honor the same rules as other offers. (#333)
- **[Bug]** **Saved offer settings not reaching the live page** — Several fields you save on an offer never make it to the live experience. This fix ensures those settings either take effect or are cleaned up if unused. (#295)
- **[Bug]** **bPerx voucher code missing from offer preview** — The voucher code line isn't showing in the offer preview on the test environment. This fix restores it so previews match the live/legacy experience. (#344)

## Surveys

- **[Bug]** **Voucher code and info links missing on the live survey** — Configured items like the voucher code and the privacy/terms/details links aren't appearing on the live survey page even though they're saved. This high-priority fix restores them, since they're needed for lead handling and compliance. (#291)
- **[Feature]** **Design settings that actually change the survey** — A thorough check across all entities to confirm every design/customization option you set is truly reflected in what visitors see, with any dead options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings** — Remaining Placement Design-tab options (like survey height and display format) will be wired through so they take effect on the live survey. (#293)
- **[Feature]** **Make the Modal design tab work — or remove it** — The Modal Design tab's six fields currently have no effect. They'll either be made to change the visitor modal or removed so the screen isn't misleading. (#294)

## Behind the Scenes

- **[Task]** **A safe testing environment against realistic data** — Setting up a read-only staging area so the team can verify the product against production-like data without risk of changing anything. (#270)
- **[Feature]** **Turn Slack conversations into tracked work automatically** — A helper that reads designated Slack channels and files action items as tracked issues, cutting out manual copy-paste. (#272)
- **[Task]** **More reliable edit-conflict protection** — Behind-the-scenes hardening of the safeguard that prevents overlapping edits, closing rare edge cases. (#342)

## Pre-Pings & Data Clients

- **[Feature]** **Bring legacy per-client eligibility checks to the new platform** — Hundreds of data clients rely on custom validation checks that aren't running yet on the new platform. This restores them so offers are correctly allowed or blocked. This is high priority. (#338)
- **[Feature]** **Real eligibility check when an offer is shown** — The display-time pre-ping will actually perform its check and hide an offer that's rejected, matching the old system, instead of only checking that a field is present. This is high priority. (#337)
- **[Feature]** **Restore post-conversion delivery behavior** — The old "after-success" client delivery/redirect steps are being brought over so post-conversion handling works as it did before. (#327)

## Reports

- **[Task]** **Investigate mismatched dashboard numbers** — Testers found dashboard report figures didn't match the legacy system. This investigation pinpoints where the difference comes from and confirms the numbers can be trusted. (#271)
- **[Feature]** **Fix offer impressions showing as zero** — Historical placement reports currently show offer impressions as 0. This fills in that number so those reports are complete. (#339)

## Flows

- **[Task]** **Fix styling glitches on the Flow form** — Parts of the Flow form look unstyled and some paired fields stack awkwardly instead of sitting side by side. This tidies up the form's appearance. Partially done. (#152)

## Campaigns

- **[Feature]** **Add the missing Campaigns module** — The Campaigns area from the old admin isn't in New Adsmith Frontend yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups. This is a critical, high-priority gap. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 72540624e535d3919fd77d9fe303c83f136dbb2b7ca301364f9323720c202039 -->
