# Open Issues — Plain-Language Overview

_Last updated 2026-07-12 07:44:06 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit it, others will see it's locked and who has it, and you'll be warned if someone changed it while you had it open — so nobody's work gets silently wiped out. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when across offers, placements, advertisers, and more (including automated changes), so you can finally answer "who changed this and when?" (#276)
- **[Feature]** **Clean up settings that don't actually do anything** — Some controls (like the Advertiser Web Presence fields, certain user permission toggles, and a few Data Client and Pre-Ping options) are shown but currently have no effect. These will be removed or hidden so screens only show settings that work. (#296)
- **[Bug]** **Invalid links in Link Testing now show an error** — Instead of quietly dropping you back on the Dashboard, testing a bad link will give you a clear failure message so you know the link didn't work. (#239)
- **[Task]** **Compare old vs. new user management screens** — A behind-the-scenes review of the legacy Users area against the new one, so any missing capabilities (like bulk actions or last-login info) can be planned and added. (#80)
- **[Task]** **Decide the future of the old File Share page** — A quick review to confirm whether the legacy file-share page is still needed in the new platform or can be safely retired. (#328)

## Offers

- **[Bug]** **Success pixels will actually fire** — Conversion tracking pixels set up on offers currently never fire because of a formatting mismatch, quietly losing attribution. This fix makes configured success pixels work as expected. (#297)
- **[Bug]** **Saved offer settings will reach the live experience** — Several saved offer options (including Modal settings, Display URL, and some data-client flags) never make it to what visitors actually see. This ensures the settings you configure are honored or cleaned up if unused. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting and can fire for visitors who should be excluded. This aligns them with normal offer targeting rules. (#333)
- **[Feature]** **Preview offers and placements with your unsaved changes** — The Preview button will show your current in-progress edits instead of only the last saved version, so you can check changes before committing them. (#292)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool to estimate a new offer's likely performance from your historical offer data, replacing the current manual gut-check review. (#322)

## Surveys

- **[Feature]** **Make every survey design option actually take effect** — A full audit to confirm each Design tab customization is reflected in the live survey view, with no settings that look editable but do nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Several Placement Design tab settings (like iFrame height and display format) are saved but never applied. These will be wired through or removed so the tab is trustworthy. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back per-client after-success behavior** — Post-conversion delivery/redirect steps used by certain clients weren't carried over to the new platform. This restores them in a flexible, configurable way. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients rely on custom validation that runs before a lead is served; that logic isn't running on the new platform yet. This ports it so those checks work again. (#338)

## Campaigns

- **[Feature]** **Add the missing Campaigns module** — The Campaigns area from the old admin (creating and editing campaigns, offer groups, CTA text, offer handling, and more) isn't in the new platform yet. This rebuilds it so campaign management is possible again. (#200)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — The entire Modal Design tab (header text, colors, and progress bar) is currently saved but never shown to visitors. It will either be connected to the visitor modal or removed. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacking instead of sitting side by side). This tidies up the form's appearance. (#152)

## Reports

- **[Task]** **Confirm Dashboard report numbers match the old system** — During testing, some Dashboard figures didn't line up with the legacy app. This investigation pinpoints and resolves any differences so you can trust the numbers. (#271)

## Behind the Scenes

- **[Task]** **Stand up a read-only test environment** — A safe, prod-like environment for verifying the new platform against real-world data, with writing disabled so nothing can be accidentally changed. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items automatically** — A helper that reads designated Slack channels and files action items as tracked issues, reducing manual note-taking and follow-up. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
