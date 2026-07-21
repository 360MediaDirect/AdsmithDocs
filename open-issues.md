# Open Issues — Plain-Language Overview

_Last updated 2026-07-21 05:03:23 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels now fire on conversions** — High priority. Right now, the conversion pixels admins set up under "Pixels to Fire on Success" silently never fire, so successful conversions aren't being tracked. Once fixed, those pixels will fire reliably and you'll stop losing attribution and revenue signal. (#297)
- **[Task]** **Auto-register offers will respect visitor targeting** — High priority. Auto-register offers currently ignore all targeting rules (age, gender, state, zip, device) and can fire for visitors who should be excluded. This work makes them honor the same targeting as regular offers, so they only fire for the right people. (#333)
- **[Bug]** **Saved offer settings will reach the live ad** — Several options you save on an offer are being dropped before they reach what visitors actually see (including some Modal-tab settings, Display URL, and the "Force More Info Visible" option). This fixes the gap so the settings you configure take effect. (#295)
- **[Bug]** **"Conflicting Referrals" field will actually work** — Today this Delivery-tab field saves but has no effect on which offers get shown. It's being reviewed and wired up (pending confirmation of the intended rule) so the exclusions you enter are honored. (#351)
- **[Feature]** **Preview your unsaved edits on placements and offers** — Currently the Preview button only shows the last-saved version, so you must save before you can see a change. This lets Preview reflect your in-progress edits without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Exploratory work to estimate how a new offer is likely to perform, based on your own historical offer data, replacing the informal manual gut-check. It's meant as a decision aid at offer intake. (#322)

## Surveys

- **[Feature]** **Design customizations will show up in the live survey** — An end-to-end check to make sure every option on the Design tab (and form options across all entity screens) actually takes effect in the survey visitors see, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey widget** — Some Placement Design-tab settings (like iFrame height and display format) don't currently reach the live widget. This wires up the remaining options so they work, or removes any that aren't needed. (#293)

## Admin & Users

- **[Task]** **Review of missing features in the Users area** — A documentation review comparing the new Users management screens against the older system to flag gaps (such as bulk actions, last-login and two-factor status, and password fields) and prioritize what to add next. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings that save but have no effect are being hidden or removed (for example the Advertiser Web Presence fields, certain user-permission toggles, and some Data-Client and Pre-Ping options), so the screens only show controls that actually work. (#296)

## Data Clients

- **[Feature]** **Restore custom pre-ping validation for data clients** — High priority. Legacy per-client checks that run at serve time (used by 448 published data clients) aren't running on the new platform yet. This ports them so those clients' custom validation applies again before ads are served. (#338)
- **[Feature]** **Restore after-success delivery behaviors** — The legacy post-conversion delivery/redirect steps for certain clients weren't carried over. This adds them back as a configurable option so those clients keep working as before. (#327)

## Modals

- **[Feature]** **Wire up or remove the Modal Design tab** — All six fields on the Modal Design tab currently save but have no effect on the modal visitors see. This either makes them work (header text, colors, progress bar) or removes them if they aren't needed. (#294)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form look unfinished — plain text boxes, unstyled color pickers, and paired fields stacking vertically instead of side by side. This cleans up the appearance to match the other forms. (#152)

## Properties

- **[Bug]** **Domain allowlist will actually block unapproved sites** — The allowed-domains list on a Property is saved but never enforced, so ads serve on any website today. This makes the platform honor the list, so requests from sites you haven't approved are withheld. (#350)

## Reports

- **[Task]** **Confirm dashboard report numbers match the older system** — During testing, some dashboard figures didn't line up with the legacy app. This investigation compares the two over a fixed date range to find any discrepancy, explain it, and confirm the numbers are trustworthy. (#271)

## Behind the Scenes

- **[Task]** **Safe, read-only test environment** — Setting up a staging copy of the product against realistic data for verification, locked to read-only so testing can't change anything. No impact on your day-to-day use. (#270)
- **[Feature]** **Auto-create tasks from team conversations** — An internal helper that turns action items from team chat into tracked work items automatically, reducing manual copy-paste. This is an internal workflow tool. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
