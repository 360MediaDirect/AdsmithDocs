# Open Issues — Plain-Language Overview

_Last updated 2026-07-18 14:25:48 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Bug]** **Success pixels aren't firing** — When an offer is set up to fire a tracking pixel on a successful conversion, that pixel currently never fires, so conversions can go unrecorded. This high-priority fix makes those success pixels fire reliably again. (#297)
- **[Bug]** **Auto-register offers ignore audience targeting** — Auto-register offers are being shown to visitors even when they fall outside the set age, gender, state, ZIP, or device targeting. This high-priority fix will make these offers respect the same targeting rules as regular offers. (#333)
- **[Bug]** **Some saved offer settings never reach live ads** — A number of offer options you can set today (including the Modal tab fields, Display URL, and several delivery flags) aren't actually being carried through to what visitors see. This work makes each of those settings either take effect or be cleaned up so nothing is misleading. (#295)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This field on the offer Delivery tab is saved but has no effect on which offers are shown. The team is confirming its intended behavior so it either works as expected or is removed. (#351)
- **[Feature]** **Preview offers and placements with your unsaved edits** — Today the Preview button shows the last saved version, so you have to save before you can see a change. Soon Preview will reflect your current in-progress edits without forcing you to save first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, giving a data-driven gut-check at intake instead of a manual review. (#322)

## Data Clients
- **[Feature]** **Bring back post-conversion delivery steps** — Certain "after success" behaviors from the legacy system (post-conversion delivery and redirects) weren't carried over yet. This work restores them so affected clients behave as they did before. This is nearly complete. (#327)
- **[Feature]** **Restore custom serve-time pre-ping checks** — Many data clients rely on custom validation that runs before an ad is served, and that logic isn't running on the new platform yet. This high-priority effort ports those checks so the affected clients get the screening they expect. (#338)

## General / Across the App
- **[Feature]** **Remove settings that don't actually do anything** — Several admin controls (such as the Advertiser Web Presence fields, certain user permission toggles, and some Data-Client and Pre-Ping options) are shown but currently have no effect. These will be hidden or removed so the settings you see are ones that genuinely work. (#296)
- **[Task]** **Users area: comparison with the previous system** — A review comparing the Users management screens against the older system to catch any missing capabilities (like bulk actions or extra columns) and prioritize what to add. This is a documentation and planning effort. (#80)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a separate environment that mirrors real data for testing and verification, locked to read-only so nothing can be changed by accident. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels and automatically files action items so requests don't get lost in manual note-taking. (#272)

## Surveys
- **[Feature]** **Make sure every design option actually shows up** — A review across all entities to confirm that each customization option on the design settings is genuinely reflected in what visitors see, with any options that go nowhere fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Some Placement design options (like iFrame height and display format) are saved but not yet applied to the survey visitors see. This work wires them through so they take effect. (#293)

## Modals
- **[Feature]** **Make the Modal Design tab actually work — or remove it** — The Modal Design tab's header and progress-bar settings are saved but never appear in the visitor-facing modal. This work either makes those settings display or removes the tab so it isn't misleading. (#294)

## Flows
- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with some paired fields stacking instead of sitting side by side. This is a careful cleanup to bring the Flow form's appearance in line with the Placement and Modal forms. (#152)

## Dashboard
- **[Task]** **Look into report numbers not matching the old system** — During testing, some dashboard report figures didn't line up with the previous system. This investigation pins down where the difference comes from and confirms the numbers can be trusted. (#271)

## Properties
- **[Bug]** **Enforce the domain allowlist on Properties** — A Property's allowed-domains list is saved but isn't actually blocking anything, so ads can serve on hostnames that aren't on the list. This fix makes the allowlist do what it says: only approved domains will serve, while properties without a list are unaffected. (#350)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
