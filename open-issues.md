# Open Issues — Plain-Language Overview

_Last updated 2026-07-19 06:50:09 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview reflects your unsaved edits** — When editing a placement or offer, the Preview button will show the changes you're currently working on, so you no longer have to save first just to see how something looks. (#292)
- **[Bug]** **Saved offer settings that never reached the live ad** — Several options you fill in on an offer aren't currently making it through to what visitors actually see. This fix makes those saved settings take effect (or removes any that were never meant to do anything). (#295)
- **[Bug]** **Success tracking pixels now fire correctly** — A high-priority fix for conversion pixels set up on offers that were silently never firing, which meant lost tracking and revenue signal. Once fixed, configured success pixels will fire as expected. (#297)
- **[Feature]** **Automatic performance projection for new offers** — Instead of relying on a manual gut-check, new offers could get a data-driven estimate of how they're likely to perform, based on your own historical offer data. An exploratory feature to help at offer intake. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — A high-priority fix: auto-register offers currently fire for every visitor, even ones that should be excluded by age, gender, state, zip, or device. This aligns them with the targeting rules that regular offers already follow. (#333)
- **[Bug]** **"Conflicting Referrals" field will actually do something** — This offer setting is saved today but has no effect. The team is confirming its intended purpose before making it work as expected (or removing it to avoid confusion). (#351)

## General / Across the App

- **[Task]** **Users screen catching up to the old system** — A review of what the new Users area still needs compared to the legacy version, covering things like bulk actions, extra filters, and login details, so nothing important is missing. (#80)
- **[Feature]** **Removing controls that don't do anything** — Some admin settings (such as the Advertiser Web Presence tab and a couple of user permission toggles) currently look active but have no effect. These will be hidden or removed so the screens only show controls that truly work. (#296)

## Surveys

- **[Feature]** **Design choices fully reflected in the live survey** — A thorough check to make sure every option on the Design tab actually changes what visitors see, across all entity types, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finishing the Placement Design settings** — Several Placement design options (like survey height and display format) aren't yet applied to the live survey. This work connects them end-to-end so they take effect. (#293)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery behaviors** — Certain "after success" delivery and redirect steps from the old system weren't carried over. This brings them back for the data clients that rely on them. (#327)
- **[Feature]** **Bringing back custom pre-ping checks** — A high-priority effort to restore the per-client validation checks (used by hundreds of data clients) that ran in the old system but aren't yet active on New Adsmith Frontend. (#338)

## Modals

- **[Feature]** **Making the Modal Design tab count** — The Modal Design tab settings (header text, colors, progress bar) don't currently appear in the modal visitors see. This work will either wire them up or remove them if the modal is meant to stay header-free. (#294)

## Properties

- **[Bug]** **Domain allowlist will actually block other sites** — Publishers can set which domains are allowed to show their ads, but today that list isn't enforced and any site can serve. This fix makes the allowlist work so only approved domains display offers. (#350)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned, with fields stacking oddly instead of sitting side by side. This cleans up the layout to match the other forms. (#152)

## Dashboard

- **[Task]** **Checking Dashboard report numbers against the old system** — During testing, some Dashboard figures didn't match the legacy app. This investigation pins down why and confirms the numbers can be trusted. (#271)

## Behind the Scenes

- **[Task]** **A safe, read-only testing environment** — Setting up a copy of the app with production-like data for review and verification, where nothing can be accidentally changed. (#270)
- **[Feature]** **Automatic issue capture from team chats** — Groundwork for a helper that turns action items raised in team conversations into tracked to-do items automatically, reducing manual copying. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
