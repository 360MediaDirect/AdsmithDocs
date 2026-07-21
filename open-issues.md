# Open Issues — Plain-Language Overview

_Last updated 2026-07-21 01:33:48 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — When an offer is set up to fire a pixel on a successful conversion, those pixels currently never fire, which means conversions can go unrecorded. This high-priority fix makes configured success pixels fire reliably so your attribution and revenue tracking stay accurate. (#297)
- **[Bug]** **Auto-register offers ignore audience targeting** — Auto-register offers currently show to every visitor, even ones outside the intended age, gender, state, ZIP, or device targeting. This high-priority fix ensures these offers respect the same targeting rules as regular offers so they only reach the right people. (#333)
- **[Bug]** **Some saved offer settings never reach live offers** — A number of offer options you can fill in today (including offer-level modal fields, Display URL, and several data-client settings) aren't actually being carried through to what visitors see. This work makes each option either take effect or be cleaned up, so what you configure matches what runs. (#295)
- **[Bug]** **"Conflicting Referrals" field has no effect** — The Conflicting Referrals box on an offer's Delivery tab is saved but currently does nothing to exclude offers. This will confirm the intended rule and either make the field work or remove it, so you're not relying on a setting that has no impact. (#351)
- **[Feature]** **Preview shows your unsaved edits** — On placement and offer edit pages, the Preview button will reflect the changes you've made in the form even before you save, so you can check your work without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, new offers could be scored against your historical offer data to estimate how they're likely to perform. This is an exploratory feature that would give you a data-driven read on a new offer at intake. (#322)

## Surveys

- **[Feature]** **Design settings actually change the survey** — Every option on the Design tab will be checked to make sure it truly affects the live survey, across all entity types. Any options that currently do nothing will be fixed or removed, so what you customize is what visitors see. (#288)
- **[Feature]** **Finish connecting Placement design settings** — Several placement Design-tab settings (like survey height and display format) aren't fully reflected in the live survey yet. This finishes wiring them up so your placement design choices take effect. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore file-based pre-ping checks for data clients** — Custom pre-delivery validation used by hundreds of data clients in the older system isn't running on New Adsmith Frontend yet. This brings that checking back so leads are properly validated before delivery. (#338)
- **[Feature]** **Restore after-success delivery behaviors** — Post-conversion delivery and redirect steps from the older system are being carried over as a flexible, configurable option, so data clients keep working the way they did after a successful conversion. (#327)

## Admin

- **[Feature]** **Remove settings that don't do anything** — Several admin controls (Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) currently have no effect. These will be hidden or removed so the admin area only shows settings that actually work. (#296)
- **[Task]** **Users area review against the older system** — A side-by-side comparison of the older Users management and the new one is underway to spot missing features (like bulk actions and last-login details) and plan what to add, so the new Users area reaches full parity. (#80)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — A staging copy of the product is being set up against production-like data for review and verification, locked to read-only so testing can't change real records. (#270)
- **[Feature]** **Turn Slack conversations into tracked tasks** — A helper that reads designated Slack channels and automatically files action items as tracked issues, cutting out manual copy-and-paste when capturing to-dos from meetings. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — The Modal Design tab (header text, colors, progress bar, and more) currently has no effect on what visitors see. These fields will either be made to work in the visitor modal or removed, so the tab is honest about what it does. (#294)

## Properties

- **[Bug]** **Domain allowlist will actually block other sites** — A property's allowed-domains list is saved but isn't enforced today, so ads can serve from any website. This fix makes the allowlist work: if you set approved domains, ads won't serve from hostnames you didn't approve, while properties with no list set are unaffected. (#350)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly and plain-looking inputs. This cleanup brings the form's appearance in line with the Placement and Modal forms for a consistent, polished look. (#152)

## Reports

- **[Task]** **Confirm dashboard numbers match the older system** — Reviewers noticed dashboard report figures didn't line up with the older system. This investigation compares the two over a fixed date range to find any differences, explain them, and confirm the numbers you rely on are correct. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
