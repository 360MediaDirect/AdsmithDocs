# Open Issues — Plain-Language Overview

_Last updated 2026-07-18 12:17:11 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — When an offer converts, the tracking pixels set up by your team currently do nothing, so successful leads may go unrecorded. This high-priority fix makes those success pixels fire reliably again, protecting your conversion tracking. (#297)
- **[Task]** **Auto-register offers ignore audience targeting** — Certain "auto-register" offers are being shown to visitors regardless of the age, gender, state, ZIP, or device rules you've set. This high-priority fix will make those offers respect your targeting so they only reach the right people. (#333)
- **[Bug]** **Some saved offer settings never reach the live ad** — A number of options you can fill in on an offer (including its Modal-tab fields, Display URL, and several delivery flags) are saved but quietly dropped before the offer goes live. This work makes each of those settings either take effect or be removed so nothing is misleading. (#295)
- **[Bug]** **"Conflicting Referrals" field has no effect yet** — The Conflicting Referrals box on an offer's Delivery tab is saved but never actually excludes anyone. This is being reviewed with the business to confirm what it should do before it's wired up or removed. (#351)
- **[Feature]** **Preview shows your unsaved changes** — On placement and offer edit pages, the Preview button currently shows the last saved version, not your in-progress edits. Once done, Preview will reflect exactly what you're working on right now, so you can check changes before saving. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Exploring a way to estimate how a new offer is likely to perform based on your own historical offer data, replacing today's manual gut-check review. Aimed at giving your team a data-driven read at offer intake. (#322)

## Behind the Scenes

- **[Task]** **A test environment that mirrors real data** — Setting up a safe, look-but-don't-touch copy of the product loaded with production-like data, so the team can verify things against realistic numbers without any risk of changing live records. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — Building an assistant that reads team discussions and files the resulting to-dos as tracked issues, so action items don't get lost in chat. This is an internal workflow improvement. (#272)

## Surveys

- **[Feature]** **Design settings that truly show up in the survey** — A thorough check to make sure every option on the Design tab actually changes what visitors see, with no settings that quietly do nothing. Any options that aren't connected will be fixed or removed. (#288)
- **[Feature]** **Finishing placement Design-tab settings** — A handful of placement Design options (like survey height and display format) are saved but don't yet affect the live survey. This connects the remaining settings so they take effect, and cleans up any that shouldn't be there. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bringing over the file-based pre-checks for 448 clients** — Legacy per-client validation that runs before an ad is served hasn't been carried over yet, meaning that custom logic isn't running for hundreds of clients. This high-priority work restores those checks on the new platform. (#338)
- **[Feature]** **Restoring after-success delivery steps** — The post-conversion redirect and delivery steps used by certain clients weren't carried over from the old system. This work brings that behavior back in a flexible, reusable way. (#327)

## Modals

- **[Feature]** **Fixing the Modal Design tab** — Right now every option on the Modal Design tab (header text, colors, progress bar, and more) is saved but has no effect on what visitors see. This work will either make those settings work or remove the tab so it's no longer misleading. (#294)

## Properties

- **[Bug]** **Domain allowlist will actually block other sites** — The allowed-domains list on a Property is saved but never enforced, so ads can currently serve from any website. This fix makes the allowlist do its job: sites you haven't approved won't be served, while properties without a list are unaffected. (#350)

## Reports

- **[Task]** **Checking dashboard report numbers against the old system** — Reviewers noticed some dashboard report figures didn't match the legacy app. This investigation pins down where the difference comes from and confirms the numbers can be trusted. (#271)

## Users

- **[Task]** **Comparing the old and new Users area** — A detailed review of what the previous Users screens could do versus the new one, so any missing capabilities (like bulk actions or last-login details) can be prioritized and added. (#80)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly instead of sitting side by side. This clean-up brings the Flow form's appearance in line with the Placement and Modal forms. (#152)

## General / Across the App

- **[Feature]** **Removing settings that don't do anything** — Several admin controls (an Advertiser Web Presence tab, some user permission toggles, and a few data-client and pre-ping options) are saved but currently have no effect. Hiding or removing them prevents confusion and avoids implying access controls that don't exist. (#296)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
