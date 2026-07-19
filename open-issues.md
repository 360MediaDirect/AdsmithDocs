# Open Issues — Plain-Language Overview

_Last updated 2026-07-19 10:30:56 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — This is a high-priority fix. Right now, conversion pixels set up on an offer's success step silently never fire, which means completed conversions can go unrecorded. Once resolved, the pixels you configure will fire reliably and attribution won't be lost. (#297)
- **[Task]** **Auto-register offers will respect visitor targeting** — A high-priority fix. Auto-register offers currently ignore age, gender, state, zip, and device targeting, so they can show to visitors who should be excluded. This work makes them honor the same targeting rules as regular offers. (#333)
- **[Bug]** **Saved offer settings that never reach live ads** — Several offer options you can fill in today (including Modal-tab fields, Display URL, and various delivery flags) are saved but quietly dropped before they reach the live widget. This audit ensures each setting either takes effect or is cleaned up so the form only shows options that actually do something. (#295)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — The Conflicting Referrals box on an offer's Delivery tab is saved but has no effect when ads are served. This work confirms the intended behavior and either makes the field work or removes it, so what you enter matches what happens. (#351)
- **[Feature]** **Preview shows your unsaved edits** — On placement and offer edit pages, the Preview button currently shows the last-saved version, so you have to save before seeing a change. Once done, Preview will reflect your in-progress edits without forcing a save first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, giving you a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Surveys

- **[Feature]** **Design settings that actually change the survey** — A full check across every entity to make sure each design-tab option you set is genuinely reflected in the live survey. Any options that don't connect to anything will be fixed or removed, so the form only offers settings that work. (#288)
- **[Feature]** **Placement design options wired into the live widget** — Several placement Design-tab settings (like iFrame height and display format) are saved but don't yet affect what visitors see. This work connects those settings end-to-end or removes the ones that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery behavior** — Certain "after success" delivery and redirect behaviors from the previous system weren't carried over. This work brings those behaviors back for the clients that still rely on them, so post-conversion handling works as before. (#327)
- **[Feature]** **Bringing back custom pre-ping validation** — A high-priority gap: custom serve-time validation used by hundreds of data clients in the old system doesn't run on the new platform yet. This work restores that validation so those clients are checked the way they used to be before an offer is served. (#338)

## Admin & Users

- **[Task]** **Filling the gaps in the Users area** — A detailed comparison of the older Users management screen against the new one, identifying missing capabilities (like bulk actions and select-all) so the new Users area can reach full parity. (#80)
- **[Feature]** **Removing controls that don't do anything** — Some admin settings (such as the Advertiser Web Presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping options) are saved but currently have no effect. These will be hidden or removed so the admin screens only show controls that genuinely work, avoiding confusion. (#296)

## Modals

- **[Feature]** **Making the Modal Design tab work — or removing it** — Every field on the Modal Design tab is currently saved but has no effect on what visitors see. This work either connects those header and progress-bar settings to the live modal or removes the tab so it isn't misleading. (#294)

## Properties

- **[Bug]** **Domain allowlist will actually block other sites** — A property's allowed-domains list is stored and editable but isn't enforced today, so ads serve on any site regardless of the list. This fix makes the allowlist do what it promises: only approved domains will serve the offer. (#350)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form don't match the polished styling of other forms, with some fields appearing plain or stacked awkwardly. This work tidies up the layout so the Flow form looks consistent and professional. (#152)

## Reports

- **[Task]** **Making dashboard numbers match the old system** — Reviewers noticed Dashboard report figures didn't line up with the previous system. This investigation pinpoints where the numbers diverge so reports can be trusted and validated with confidence. (#271)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a separate environment loaded with realistic data for verification and testing, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Turning conversations into tracked to-dos automatically** — An internal helper that reads team discussions and files the resulting action items automatically, reducing manual note-taking so nothing slips through the cracks. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
