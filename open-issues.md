# Open Issues — Plain-Language Overview

_Last updated 2026-07-18 06:37:58 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved edits before saving** — On the placement and offer edit screens, the Preview will show the changes you're currently making instead of the last saved version, so you can check your work without having to save first. (#292)
- **[Bug]** **Some saved offer settings weren't reaching live ads** — A number of offer options you fill in (including Modal-tab fields, Display URL, and several data-client settings) were being saved but never actually applied to the live experience. This work makes sure each one either takes effect or is removed so it's not misleading. (#295)
- **[Bug]** **Success pixels weren't firing** — High priority. Conversion tracking pixels set up on offers were silently never firing, meaning lost tracking of successful conversions. This fixes them so configured pixels reliably fire. (#297)
- **[Bug]** **Auto-register offers ignored visitor targeting** — High priority. Auto-register offers were being shown to visitors even when age, gender, state, ZIP, or device targeting should have excluded them. This makes them respect the same targeting rules as other offers. (#333)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This offer field is saved but has no effect on what's served. The team is confirming its intended purpose so it can either be made to work or removed to avoid confusion. (#351)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool that estimates a new offer's likely performance based on your historical offer data, replacing an informal manual gut-check. It would give a data-backed projection at intake time. (#322)

## Data Clients & Pre-Pings

- **[Feature]** **Carry over post-conversion client behaviors** — High priority. Custom actions that run after a successful conversion for certain clients weren't yet available on New Adsmith Frontend. This brings them back so those clients keep working as before. (#338 relates; #327)
- **[Feature]** **Restore custom pre-checks for data clients** — High priority. Hundreds of data clients rely on custom serve-time validation checks that hadn't been carried over yet, so their rules weren't running. This work brings that validation back and applies it when ads are served. (#338)

## Surveys

- **[Feature]** **Make sure every Design option actually does something** — A thorough review across all entity screens to confirm each customization option you set is genuinely reflected in what visitors see, with any options that do nothing either wired up or removed. (#288)
- **[Feature]** **Finish connecting Placement Design settings** — Several Placement Design-tab settings (like survey height and display format) either weren't applied or had no effect. This finishes wiring them so your choices show up in the live survey. (#293)

## Admin

- **[Task]** **Users screen comparison with the old system** — A detailed review comparing the old Users management with New Adsmith Frontend to spot missing capabilities (like bulk role changes, password entry, and last-login info) and plan what to add next. (#80)
- **[Feature]** **Remove controls that don't do anything** — Several admin settings (Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) are saved but have no effect. Hiding or removing them prevents confusion and false expectations. (#296)

## Behind the Scenes

- **[Task]** **A safe testing environment against real-like data** — Setting up a read-only staging copy of New Adsmith Frontend so the team can verify behavior against production-like data without any risk of changing it. (#270)
- **[Feature]** **Automatic issue creation from team chats** — A helper that turns action items mentioned in team conversations into tracked work items automatically, reducing manual copying. (#272)

## Dashboard

- **[Task]** **Investigate report numbers that don't match the old system** — Reviewers noticed dashboard report figures differing from the legacy app. This work traces where the difference comes from and confirms the numbers can be trusted. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The entire Modal Design tab currently has no effect on the visitor-facing modal. This will either wire up its header and progress-bar settings or remove the tab so it isn't misleading. (#294)

## Properties

- **[Bug]** **Enforce the domain allowlist** — A property's list of allowed domains was saved but never actually enforced, so ads could serve on any website. This makes the allowlist block requests from domains you haven't approved. (#350)

## Flows

- **[Task]** **Fix the appearance of the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other screens, with fields stacking instead of sitting side by side. This tidies up the layout to match the rest of the product. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
