# Open Issues — Plain-Language Overview

_Last updated 2026-07-19 12:16:59 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — When an advertiser sets up conversion tracking pixels to fire when an offer succeeds, those pixels currently never fire, so completed conversions go unrecorded. This high-priority fix makes configured success pixels actually fire, restoring accurate attribution. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Some offers that count automatically on page load are skipping the age, gender, state, ZIP, and device rules that normally decide who's eligible. This fix ensures those offers respect the same targeting as every other offer, so they only count for the right visitors. (#333)
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of offer options you can fill in today (including modal settings, Display URL, and several delivery flags) are saved but quietly dropped before they reach visitors. This work makes those options take effect or removes the ones that aren't needed, so the form matches reality. (#295)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This offer field can be filled in but has no effect on what visitors see. This work clarifies its intended purpose and either makes it work or removes it, so you're not relying on a setting that isn't applied. (#351)
- **[Feature]** **Preview shows your unsaved changes** — On the Placement and Offer edit screens, Preview will reflect the edits you've just made instead of the last saved version, so you can check your work without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool to estimate how a new offer is likely to perform based on your historical offer data, giving a data-driven gut-check in place of a manual review. (#322)

## Surveys

- **[Feature]** **Design settings that actually show up in the survey** — A thorough check to make sure every option on the Design tab (across all entity screens) truly changes what visitors see, with any options that do nothing getting wired up or removed. (#288)
- **[Feature]** **Finish connecting Placement design options to the live widget** — Several Placement Design-tab settings, such as widget height and display format, are saved but not yet reflected in the survey. This finishes hooking them up so your choices appear as expected. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back after-success client behaviors** — Post-conversion delivery and redirect steps used by certain clients weren't carried over to New Adsmith Frontend. This work restores them as a reusable, configurable option so those clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-serve validation for data clients** — A large set of data clients relied on custom checks that ran before an ad was served, and those checks aren't running on the new platform yet. This high-priority effort brings that validation back so the right visitors are screened as intended. (#338)

## General / Across the App

- **[Feature]** **Remove admin controls that don't do anything** — Several settings across screens (Advertiser Web Presence, some user permission toggles, and a few data-client and pre-ping options) are saved but never actually applied. Hiding or removing them prevents confusion and false expectations about what they control. (#296)
- **[Task]** **Users screen gap review** — A detailed comparison between the older Users management and the new one, highlighting missing capabilities (like bulk actions and last-login info) to guide what's added next. This is groundwork that shapes upcoming Users improvements. (#80)

## Behind the Scenes

- **[Task]** **Safe test environment against real-world data** — Setting up a read-only copy of the app wired to production-like data so the team can verify behavior without any risk of changing live records. (#270)
- **[Feature]** **Auto-create tasks from team conversations** — An internal helper that turns action items from team chats into tracked work items automatically, reducing manual note-taking. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab count** — The Modal Design tab's settings (header text, colors, progress bar) currently don't appear in the visitor-facing modal. This work either connects them so they take effect or removes the tab if it isn't needed. (#294)

## Properties

- **[Bug]** **Enforce the domain allowlist on Properties** — A property's list of approved domains is saved but not currently enforced, so ads can serve from any website. This fix makes the allowlist actually block unapproved domains, while properties without a list keep working exactly as before. (#350)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with paired fields stacking instead of sitting side by side. This cleanup brings the Flow form in line with the polished look of the Placement and Modal forms. (#152)

## Reports

- **[Task]** **Confirm dashboard numbers match the legacy system** — Review found dashboard report figures that didn't line up with the old system, making them hard to trust. This investigation pins down the cause and confirms the numbers are consistent. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
