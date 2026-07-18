# Open Issues — Plain-Language Overview

_Last updated 2026-07-18 22:16:38 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels weren't firing** — When an offer is set up to fire a pixel on a successful conversion, that pixel was silently never firing, so conversions weren't being recorded. This fix makes those success pixels fire reliably again, restoring accurate conversion tracking. High priority. (#297)
- **[Task]** **Auto-register offers ignored visitor targeting rules** — Auto-register offers were being shown to everyone, even when age, gender, state, ZIP, or device targeting should have excluded them. Once resolved, these offers will respect the same targeting rules as regular offers so they only reach the intended audience. High priority. (#333)
- **[Bug]** **Some saved offer settings never reached live offers** — Several options you can set on an offer (including Modal-tab settings, Display URL, and certain delivery flags) were being dropped and never applied to the live offer. This work makes sure each saved setting is either actually used or cleaned up so the form only shows options that do something. (#295)
- **[Bug]** **"Conflicting Referrals" field had no effect** — The Conflicting Referrals box on the offer Delivery tab saved what you typed but never actually excluded any offers. This is being reviewed to confirm what the field should do and then make it work as expected (or remove it if it's no longer needed). (#351)
- **[Feature]** **Preview your unsaved offer and placement edits** — Today the Preview button shows the last saved version, so you have to save before you can see a change. After this update, Preview will reflect your current in-progress edits, so you can check your work before saving. (#292)
- **[Feature]** **Predict how a new offer might perform** — An early exploration to automatically estimate how a new offer is likely to perform based on your existing offers and their history, replacing today's manual gut-check review. This would give a helpful data-based projection at intake time. (#322)

## General / Across the App

- **[Task]** **Review of the Users area against the older system** — A detailed comparison of the Users screens in New Adsmith Frontend against the legacy system, identifying features that still need to be added (like bulk role changes, last-login and two-factor status, and password setup). This guides upcoming improvements to bring the Users area up to par. (#80)
- **[Feature]** **Remove admin settings that don't actually do anything** — Some controls (such as Advertiser Web Presence fields, certain user permission toggles, and a few Data Client and Pre-Ping options) are saved but have no effect. These will be hidden or removed so the admin screens only show settings that truly work, avoiding confusion. (#296)

## Surveys

- **[Feature]** **Make every Design tab setting actually change the survey** — A thorough review across all entities to confirm that each option you set on a Design tab is fully reflected in the live survey. Any settings that don't currently take effect will be fixed or removed so what you configure is what visitors see. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live widget** — Certain Placement Design-tab options (like survey height and display format) are saved but not yet applied when the survey runs. This work wires them through so they take effect, and cleans up any that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring post-conversion delivery behaviors to the new platform** — Some clients relied on special actions that ran after a successful conversion (like delivery and redirect steps) that weren't yet available in New Adsmith Frontend. These are being carried over so those clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-check validation for data clients** — Hundreds of data clients used custom pre-checks that ran before serving, and these weren't carried into the new platform. This work brings that validation back so those clients' serve-time checks run correctly again. High priority. (#338)

## Behind the Scenes

- **[Task]** **A safe, view-only testing environment** — Setting up a separate environment that mirrors real data but can't change it, so the team can verify New Adsmith Frontend against realistic information without any risk to live data. (#270)
- **[Feature]** **Turn team conversations into tracked work automatically** — A helper that reads designated team chat channels and files action items as tracked tasks, so requests raised in conversation don't get lost. This is an internal productivity tool. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — Every field on the Modal Design tab currently saves but has no effect on what visitors see. This work will either connect these settings (header text, colors, progress bar) to the visitor modal or remove the tab if it isn't needed. (#294)

## Properties

- **[Bug]** **Enforce the domain allowlist on Properties** — A Property's list of allowed domains was saved but never actually enforced, so ads could serve from any website. This fix makes the allowlist work: if a site isn't on the list, the offer simply won't serve there, while properties without a list are unaffected. (#350)

## Dashboard

- **[Task]** **Confirm Dashboard report numbers match the older system** — During testing, some Dashboard report totals didn't line up with the legacy system. This investigation compares the two over a fixed period to find and explain any differences, so you can trust the numbers you see. (#271)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned — plain textareas, unstyled color pickers, and paired fields stacking vertically instead of side by side. This cleanup brings the Flow form in line with the polished look of the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
