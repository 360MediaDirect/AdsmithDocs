# Open Issues — Plain-Language Overview

_Last updated 2026-07-21 17:30:01 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success conversion pixels aren't firing** — Tracking pixels that admins set to fire when an offer converts are being saved but never actually run, so conversions can go uncounted with no visible error. Fixing this restores accurate attribution and revenue tracking. High priority. (#297)
- **[Task]** **Auto-register offers ignore visitor targeting rules** — Auto-register offers currently fire for every visitor even when age, gender, state, ZIP, or device targeting should exclude them. Once resolved, these offers will respect the same targeting rules as regular offers so they only reach the intended audience. High priority. (#333)
- **[Bug]** **Saved offer options getting dropped before they reach visitors** — Several options you set on an offer (including its Modal-tab settings, Display URL, and certain data-client flags) aren't making it through to what visitors actually see. This work confirms each option either takes effect or is cleanly removed so the form only shows settings that do something. (#295)
- **[Bug]** **"Conflicting Referrals" field has no effect** — The Conflicting Referrals box on an offer's Delivery tab is saved but never actually excludes anything at serve time. This will be clarified and either wired up to work as intended or removed so it doesn't mislead. (#351)
- **[Feature]** **Preview unsaved edits on Placements and Offers** — Today the Preview button only shows the last saved version, so you have to save before you can see a change. You'll soon be able to preview your in-progress edits without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Exploring a way to estimate how a new offer is likely to perform based on your own historical offer data, replacing an informal manual gut-check. This would give a data-driven forecast at intake time. Medium priority. (#322)

## Data Clients

- **[Feature]** **Restore per-client post-conversion behaviors** — Certain "after success" delivery and redirect steps from the legacy system weren't carried over. This work brings them back for the affected clients so post-conversion handling behaves as it did before. Nearly complete. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients relied on custom serve-time validation checks in the legacy system that currently don't run on New Adsmith Frontend. Once ported, those clients' checks will run again so eligibility is enforced as intended. High priority. (#338)

## Surveys

- **[Feature]** **Make every Design tab option actually take effect** — A review is under way to ensure each customization option across all entity forms flows through to what visitors see, with no settings that quietly do nothing. You'll be able to trust that the options you set are applied. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Some Placement Design tab settings (like survey height and display format) are saved but not yet reflected in the live survey. This finishes wiring them up so your design choices show through, and removes any options that aren't used. (#293)

## Admin Area

- **[Task]** **Users screen feature review against the legacy system** — A detailed comparison of the old Users management screen and the new one, identifying gaps like bulk actions and role-change tools that haven't been carried over yet. This guides bringing the Users area up to full parity. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings across Advertisers (Web Presence), user permissions, Data Clients, and Pre-Pings are saved but have no effect, which can be confusing and misleading. These will be hidden or removed (or properly implemented) so every control you see does what it says. (#296)

## Modals

- **[Feature]** **Fix or remove the Modal Design tab** — All six fields on the Modal Design tab are saved but never appear in the modal visitors see. This work will either make those header and progress-bar settings display properly or remove the tab so it isn't misleading. (#294)

## Properties

- **[Bug]** **Domain allowlist isn't being enforced** — When a property has an allowed-domains list, requests from other websites are currently served anyway instead of being blocked. This will make the allowlist actually restrict serving to approved domains, while properties without a list continue to work unchanged. (#350)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form look unstyled or misaligned compared to other forms — plain text boxes, unstyled color pickers, and fields stacked vertically instead of side by side. This cleanup makes the Flow form look consistent with the rest of the app. Partly done. (#152)

## Dashboard & Reports

- **[Task]** **Investigate mismatched dashboard report numbers** — During testing, some dashboard report totals didn't match the legacy system, making it hard to confirm the new figures. This investigation pins down where the difference comes from and confirms the numbers can be trusted. (#271)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only testing environment** — Standing up a test copy of the product using production-like data that can't be changed, so the team can verify behavior without any risk to live data. No user-facing change. (#270)
- **[Feature]** **Automatically turn meeting discussions into tracked work items** — A tool to capture action items from team conversations and file them as tracked issues automatically, reducing manual effort in triaging requests. Internal workflow improvement. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
