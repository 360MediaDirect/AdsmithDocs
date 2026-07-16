# Open Issues — Plain-Language Overview

_Last updated 2026-07-16 05:01:44 UTC · 19 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers to confirm a successful sign-up currently never fire, so you may be losing credit for results without any warning. This fix makes configured success pixels fire reliably. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers can currently reach visitors who should be excluded by age, gender, state, ZIP, or device rules. This work makes those offers respect the same targeting as regular offers (or clearly documents the intended behavior). (#333)
- **[Bug]** **Some saved offer settings never reach the live experience** — A number of options you can set on an offer (including modal settings, "Force More Info Visible," Display URL, and several data-client flags) are saved but never actually used. This clean-up either wires each one through or removes options that do nothing. (#295)
- **[Feature]** **Preview shows your unsaved edits** — On the placement and offer edit screens, the Preview button will reflect the changes you're currently making, so you can check your work without having to save first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, as a data-driven replacement for the manual gut-check review. (#322)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When two admins open the same record, you'll see a clear "locked by" notice and a warning if someone else changed it while you had it open, so edits can't be silently lost. (#267)
- **[Feature]** **Remove admin controls that don't actually do anything** — Several settings that look active but have no effect (Advertiser Web Presence fields, certain user-permission toggles, and some Data-Client and Pre-Ping options) will be hidden or removed so the admin screens only show controls that work. (#296)
- **[Task]** **Users screen review against the legacy system** — A documentation review comparing the old Users area with the new one to spot missing capabilities (like bulk actions, last-login, and 2FA status) and plan what to add. (#80)
- **[Bug]** **Invalid link test lands you on the dashboard** — Testing an invalid link currently bounces you to the dashboard instead of telling you it failed. This fix shows a clear error result in the Link Testing screen. (#239)
- **[Task]** **Decide the future of the old file-share page** — A quick keep-or-retire decision on the legacy file-share page, which has no equivalent in New Adsmith Frontend and may no longer be needed. (#328)

## Surveys

- **[Feature]** **Design tab settings show up in the live survey** — An end-to-end review to make sure every option on the Design tab actually appears in the survey visitors see, with any unused options fixed or removed across all screens. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey** — A few placement Design-tab settings (like iFrame height and display format) aren't yet reflected in the live survey widget. This work wires them through or removes the ones that aren't used. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back after-success delivery steps for clients** — Post-conversion delivery and redirect behavior from the old system hasn't been carried over. This adds a configurable step so those client hand-offs happen again on the new platform. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients rely on custom serve-time validation from the legacy system that currently doesn't run. This work brings those checks back so leads are validated as expected. (#338)

## Behind the Scenes

- **[Task]** **A read-only staging environment for testing** — Setting up a safe, look-but-don't-change copy of the product wired to production-like data, so testing and verification can happen without touching live records. (#270)
- **[Feature]** **Automatic issue creation from team chat** — A helper that reads designated chat conversations and turns action items into tracked tasks automatically, reducing manual copy-and-paste. (#272)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or stack awkwardly compared to other forms. This work brings its layout and styling in line with the rest of the app. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The Modal Design tab's settings are saved but never shown to visitors. This will either display them in the visitor modal or remove the tab so it isn't misleading. (#294)

## Reports & Dashboard

- **[Task]** **Confirm dashboard numbers match the legacy system** — An investigation into why some dashboard report figures didn't line up with the old system, so you can trust the numbers you see. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: d541cdec2d7ef7e80b16585fe689f12231c8b31406080f26d5421cd3a156890a -->
