# Open Issues — Plain-Language Overview

_Last updated 2026-07-10 15:47:36 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Safeguard against two people overwriting each other's work** — When you open a record to edit, others will see it's being worked on and by whom, and you'll be warned if someone changed it while you had it open — so edits no longer get silently wiped out. (#267)
- **[Feature]** **A searchable history of every change** — A new admin activity log will record who changed what and when — for both people and automated processes — so you can always trace a change back to its source. (#276)
- **[Feature]** **Remove admin settings that don't actually do anything** — Several controls that look active but have no effect (like the Advertiser Web Presence fields and certain user-permission toggles) will be hidden or removed to prevent confusion. (#296)
- **[Task]** **Decide the future of the old file-share page** — A leftover file-sharing page from the previous system will be reviewed to confirm whether it's still needed or can be retired. (#328)
- **[Task]** **Compare the old and new Users area** — A review of the legacy Users screen against the new one to spot any missing features and plan what still needs building. (#80)
- **[Bug]** **Clear error when testing an invalid link** — Testing a broken link will show a proper failure message instead of quietly sending you back to the Dashboard. (#239)

## Offers
- **[Bug]** **Saved offer settings that never reached the live page** — Several configured offer options weren't being carried through to what visitors actually see; these will either be delivered properly or removed if unused. (#295)
- **[Bug]** **Success tracking pixels weren't firing** — Conversion pixels set on offers were silently never firing, causing lost tracking; this high-priority fix makes them work as configured. (#297)
- **[Feature]** **Automatic performance estimate for new offers** — Instead of a manual gut-check, new offers could get a data-driven projection of likely performance based on your historical offer data. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — High-priority fix so auto-registered offers honor age, gender, state, zip, and device targeting instead of firing for everyone. (#333)
- **[Bug]** **bPerx voucher code missing from offer preview** — The "Your Voucher Code" line isn't showing in the offer preview on the test environment; this will restore it to match the old system. (#344)

## Surveys
- **[Feature]** **Design tab choices will show up in the survey** — Every customization option on the Design tab will be reflected in the live survey view, with a full check that no option is left disconnected. (#288)
- **[Bug]** **Voucher code and info links now appear on the survey page** — High-priority fix so the configured voucher code and the privacy/terms/details links render on the live survey, as they did in the old system. (#291)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Remaining Placement Design-tab options (like survey height and display format) will either be applied to the live survey or removed if unused. (#293)

## Placements & Reports
- **[Feature]** **Preview your unsaved changes before saving** — The Preview button on Placement and Offer edit screens will show your in-progress edits, so you no longer have to save first just to see how a change looks. (#292)
- **[Feature]** **Offer impressions in historical placement reports** — Older placement reports currently show zero offer impressions; this improvement fills in the real numbers. (#339)
- **[Task]** **Investigate dashboard numbers that don't match the old system** — A review to find why some report figures differ from the legacy app, so you can trust the data during testing. (#271)

## Pre-Pings & Data Clients
- **[Feature]** **Real pre-ping check before showing certain offers** — High-priority work so display-triggered pre-pings actually verify with the advertiser at serve time and hide the offer if rejected, matching the old system. (#337)
- **[Feature]** **Bring over the legacy per-client pre-ping checks** — Hundreds of data clients rely on custom pre-ping validation that isn't running on the new platform yet; this restores those checks. (#338)
- **[Feature]** **Restore post-conversion delivery for data clients** — The old "after success" scripts that run after a conversion will be rebuilt as a configurable option so nothing is lost in the move. (#327)

## Behind the Scenes
- **[Task]** **Set up a safe, read-only test environment** — A staging copy of New Adsmith Frontend using production-like data, locked to read-only so testing can't change real records. (#270)
- **[Feature]** **A helper that turns Slack chats into tracked tasks** — An internal tool to automatically capture action items from team conversations, reducing manual note-taking. (#272)

## Modals
- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — The Modal Design tab's settings currently have no effect on what visitors see; they'll either be applied to the modal or removed to avoid confusion. (#294)

## Flows
- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form look unstyled or misaligned; this cleanup makes fields, text boxes, and color pickers match the rest of the app. (#152)

## Campaigns
- **[Feature]** **Bring the Campaigns area into New Adsmith Frontend** — The Campaigns module from the old system is missing; this adds the ability to create, edit, and manage campaigns and offer groups as before. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 20c05265760e30b087db164aa9ffb7701fea9cb19d23bb2497ef9c503a36041b -->
