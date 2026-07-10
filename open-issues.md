# Open Issues — Plain-Language Overview

_Last updated 2026-07-10 23:20:10 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Bring back full campaign management** — You'll be able to create, edit, and manage campaigns and their offer groups directly in New Adsmith Frontend, just like the old system. This is a high-priority gap since campaign management currently can't be done at all in the new platform. (#200)
- **[Feature]** **Preview your unsaved edits on placements and offers** — When you click Preview while editing a placement or offer, you'll see how your current changes will look without having to save first. (#292)
- **[Bug]** **Saved offer options now reach the live experience** — Several offer settings were being saved but never actually applied to what visitors see. This fix makes sure each option either takes effect or is removed if it isn't needed. (#295)
- **[Bug]** **Success tracking pixels will fire correctly** — Conversion pixels configured on offers weren't firing, quietly losing tracking data. Once fixed, the pixels you set up will fire as expected. (#297)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, new offers could get an estimated performance projection based on your historical offer data, helping you gauge a new offer at intake. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently ignore age, gender, state, zip, and device targeting, so they can show to people they shouldn't. This work makes their targeting behave consistently with regular offers. (#333)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — If someone else is already editing a record, you'll see a clear "locked by" notice, and you'll be warned before saving over a change made while your screen was open. This protects against accidental lost work across every entity screen. (#267)
- **[Feature]** **Searchable activity log** — Administrators will be able to see who changed what and when across offers, placements, advertisers, and more, including automated changes, making it far easier to answer "who changed this?". (#276)
- **[Feature]** **Remove settings that don't actually do anything** — Several controls (such as the Advertiser Web Presence fields and a few user, data-client, and pre-ping options) are shown but have no effect. They'll be hidden or removed so screens only show controls that work. (#296)
- **[Task]** **Review the Users area against the old system** — A detailed comparison of the old and new Users screens to make sure important capabilities (like bulk actions and login details) aren't missing. This is a documentation and planning step. (#80)
- **[Bug]** **Clear error when testing an invalid link** — Testing an invalid link currently drops you back on the Dashboard with no explanation. Instead, you'll get a clear failure message so you know the link didn't work. (#239)
- **[Task]** **Decide the future of the file-share page** — The old file-share page has no equivalent yet. This is a quick decision on whether to rebuild it or retire it for good. (#328)

## Surveys

- **[Feature]** **Design customizations will actually show up** — A full check to make sure every design-tab option you set is reflected in the survey visitors see, with any dead options fixed or removed. (#288)
- **[Feature]** **Finish connecting placement Design settings** — A handful of placement design settings (like survey height and display format) are saved but not yet applied. This finishes wiring them through so they take effect. (#293)
- **[Feature]** **Make the Modal Design tab work (or remove it)** — The entire Modal Design tab is currently saved but never displayed. This work will either make those header and progress-bar settings appear in the visitor modal or remove the tab if it isn't needed. (#294)

## Behind the Scenes

- **[Task]** **Set up a read-only staging environment** — A safe, look-but-don't-touch copy of the platform loaded with realistic data, so testing can happen against production-like information without any risk of changing it. (#270)
- **[Task]** **Investigate report numbers not matching the old system** — Dashboard report totals didn't line up with the legacy app during testing. This looks into why and confirms the numbers can be trusted. (#271)
- **[Feature]** **Turn Slack discussions into tracked work items** — A helper that reads designated Slack conversations and files them as tracked issues automatically, reducing manual note-taking and follow-up. (#272)

## Data Clients & Pre-Pings

- **[Feature]** **Restore post-conversion delivery behavior** — Certain after-success delivery steps from the old system weren't carried over. This brings them back in a flexible, configurable way for the clients that still need them. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients rely on custom serve-time validation that isn't running on the new platform yet. This work ports those checks so the right leads are accepted or rejected as before. (#338)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Some parts of the Flow form appear unstyled or misaligned compared to other screens. This cleans up the layout so text boxes, color pickers, and paired fields display neatly. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
