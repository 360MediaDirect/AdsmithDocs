# Open Issues — Plain-Language Overview

_Last updated 2026-07-20 19:32:07 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — Conversion tracking pixels set up on offers currently never fire, so successful leads aren't being counted. This high-priority fix makes those pixels reliably fire when a conversion happens, restoring accurate attribution. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers are being served to visitors they should exclude (by age, gender, state, ZIP, or device). This fix ensures those offers respect the same targeting rules as regular offers. (#333)
- **[Bug]** **Some saved offer options never reach live offers** — Several options you can set on an offer (including Modal-tab settings, Display URL, and various delivery flags) are saved but silently dropped before they take effect. This work makes sure each option either actually works or is removed so nothing is misleading. (#295)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This offer setting saves your input but has no effect on which offers are shown. This will either make it work as intended or remove it so the form only shows controls that matter. (#351)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — The Preview button will show your current edits, even before you save, so you no longer have to save first just to see how a change looks. (#292)
- **[Feature]** **Predict how a new offer will perform** — Instead of a manual gut-check, New Adsmith Frontend will estimate a new offer's likely performance using your historical offer data, giving you a data-driven projection at intake time. (#322)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back custom pre-checks for data clients** — Legacy custom validation that ran before serving certain data clients (used by 448 clients) isn't running on the new platform yet. This high-priority work restores that per-client checking so leads are validated as they were before. (#338)
- **[Feature]** **Restore after-conversion delivery steps** — Legacy "after-success" delivery and redirect behaviors weren't carried over. This adds a general, configurable way to run those post-conversion steps again for the clients that still need them. (#327)

## Admin & Users

- **[Task]** **Compare old and new Users management** — A detailed review of the legacy Users area against the new one, identifying which features are still missing (like bulk role changes, last-login and 2FA visibility, and a password field on new users) so they can be prioritized. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings across Advertisers (Web Presence), user permissions, Data-Client, and Pre-Ping are saved but have no effect. These will be hidden or removed so the admin screens only show controls that actually work. (#296)

## Surveys

- **[Feature]** **Make every design option actually show up** — A full check to ensure each customization you set on the design tab is reflected in the live survey, with any settings that don't do anything either wired up or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Some Placement design-tab settings (like iFrame height and display format) are saved but not yet applied to the visitor-facing widget. This finishes hooking them up so your choices take effect. (#293)

## Behind the Scenes

- **[Task]** **Set up a safe testing environment** — A read-only staging copy of New Adsmith Frontend, wired to production-like data, so the team can verify behavior without any risk of changing real records. (#270)
- **[Feature]** **Automatically turn meeting notes into tracked tasks** — A helper that reads team conversations and files them as tracked work items, reducing manual copy-and-paste and helping nothing slip through the cracks. (#272)

## Modals

- **[Feature]** **Make the Modal design tab work or remove it** — Every field on the Modal design tab currently saves but has no effect on what visitors see. This will either build out the header and progress-bar styling for real, or remove the tab if it isn't needed. (#294)

## Properties

- **[Bug]** **Enforce the domain allowlist on Properties** — Today a Property's list of allowed domains is saved but not enforced, so ads can serve from any website. This fix makes the allowlist actually block requests from hostnames you haven't approved. (#350)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or awkwardly laid out (plain textareas, unstyled color pickers, fields stacking instead of sitting side-by-side). This tidies up the form to match the polish of other screens. (#152)

## Reports & Dashboard

- **[Task]** **Confirm Dashboard report numbers match the old system** — An investigation into why some Dashboard report figures differed from the legacy system, to pin down the cause and confirm the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
