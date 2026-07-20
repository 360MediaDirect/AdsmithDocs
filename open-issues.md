# Open Issues — Plain-Language Overview

_Last updated 2026-07-20 13:34:00 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Bug]** **Some saved offer options never reach live ads** — Certain settings you configure on an offer (like its modal-tab fields, Display URL, and several data-client options) currently don't take effect on live surfaces. This fix makes sure each of those options either works as expected or is removed so it isn't misleading. (#295)
- **[Bug]** **Success pixels aren't firing** — Conversion tracking pixels set up under "Pixels to Fire on Success" silently never fire, which means lost tracking and attribution with no visible error. This high-priority fix ensures a configured success pixel actually fires. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Offers that fire automatically are skipping the age, gender, state, zip, and device rules you set, so they can reach visitors they should exclude. This high-priority fix makes them honor targeting (or documents the behavior clearly). (#333)
- **[Bug]** **"Conflicting Referrals" field doesn't do anything yet** — The Conflicting Referrals box on the offer Delivery tab is saved but has no effect when serving. We'll confirm the intended rule and either make it work or clarify its status. (#351)
- **[Feature]** **Preview your unsaved changes on placements and offers** — The Preview button will show the edits you've made right now, so you no longer have to save first just to see how a change looks. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, new offers could be scored against your historical offer data to estimate likely performance, giving a data-driven read at intake. This is exploratory. (#322)

## Surveys
- **[Feature]** **Every design option actually shows in the survey** — We're checking that each customization on the Design tab is reflected in the live survey, and auditing options across all entity screens so nothing is a dead setting. (#288)
- **[Feature]** **Placement design settings connected to the live survey** — Settings like iFrame Height and Display Format, plus a few other Placement design options, will properly carry through to what visitors see (or be removed if not needed). (#293)

## Data Clients
- **[Feature]** **Restore after-success delivery behaviors** — Post-conversion delivery and redirect steps from the previous system are being brought over so affected clients keep working as before. (#327)
- **[Feature]** **Bring legacy pre-ping checks to the new platform** — Many data clients rely on custom serve-time validation that currently doesn't run. This high-priority work restores those checks so the right visitors are accepted or rejected as intended. (#338)

## Admin / Users
- **[Task]** **Review of the Users area against the old system** — A detailed comparison of the previous Users management screens versus the new ones, so we know which features are still missing and can plan them. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Some settings (Advertiser Web Presence fields, certain user permission toggles, and a few others) are saved but have no effect. Hiding or removing them prevents confusion and false expectations, especially around access control. (#296)

## Behind the Scenes
- **[Task]** **A safe, read-only testing environment** — Sets up a staging copy wired to production-like data for verification, with writing disabled so testing can't change anything. (#270)
- **[Feature]** **Auto-create tickets from team conversations** — A helper that turns discussion notes into tracked work items automatically, reducing manual copy-paste. (#272)

## Modals
- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The Modal Design tab's fields currently don't change what visitors see. We'll either wire them into the visitor modal or remove them so the tab isn't misleading. (#294)

## Properties
- **[Bug]** **Enforce the domain allowlist on Properties** — Today an allowlist can be set but ads still serve from any website. This fix makes ads serve only from the domains you've approved, with no change for properties that leave the list empty. (#350)

## Reports / Dashboard
- **[Task]** **Investigate mismatched dashboard report numbers** — Report totals didn't line up with the old system during testing. This work pins down where the difference comes from and confirms the numbers can be trusted. (#271)

## Flows
- **[Task]** **Fix the look of the Flow form** — Some parts of the Flow form appear unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacking oddly). This cleanup brings it in line with the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
