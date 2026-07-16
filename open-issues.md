# Open Issues — Plain-Language Overview

_Last updated 2026-07-16 19:27:48 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Right now, when a visitor successfully completes an offer, the conversion pixels set up by admins silently fail to fire, meaning credit for those conversions is being lost. This high-priority fix makes sure configured success pixels actually fire every time. (#297)
- **[Bug]** **Some offer settings never reach visitors** — Several options you can set on an offer (including its Modal-tab fields, Display URL, and various delivery flags) are saved but not carried through to the live experience. Once fixed, each of these settings will either work as expected or be cleaned up if it's no longer needed. (#295)
- **[Task]** **Auto-register offers now respect visitor targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting, so they can fire for people who should be excluded. This high-priority fix brings them in line with your targeting rules. (#333)
- **[Feature]** **Preview your unsaved offer and placement changes** — The Preview button will show the edits you're currently making instead of only the last saved version, so you can check your work before committing it. (#292)
- **[Feature]** **Performance projections for new offers** — We're exploring an automated way to estimate how a new offer is likely to perform based on your historical offer data, giving you a data-driven gut-check at intake. (#322)

## Admin / Across the App

- **[Feature]** **Cleaning up admin controls that don't do anything** — Some settings (like the Advertiser Web Presence tab, certain user permission toggles, and a few Data-Client and Pre-Ping options) are saved but currently have no effect. They'll be hidden or removed so the admin screens only show controls that actually work. (#296)
- **[Task]** **Review of the Users area against the old system** — A detailed comparison of the legacy Users management screens versus the new ones, to catch missing capabilities (such as bulk actions, last-login info, and two-factor status) and plan what to bring over. This is a planning/documentation effort. (#80)

## Surveys

- **[Feature]** **Design tab customizations fully reflected in the survey** — A thorough check across all entities to make sure every option you set on a Design tab actually shows up in the survey visitors see, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — A handful of placement Design-tab settings (like iFrame height, display format, and a few display options) are saved but not yet applied to the live widget. Each will be wired up to work or removed if unused. (#293)

## Data Clients

- **[Feature]** **Bringing back post-conversion delivery behavior** — Certain after-success delivery and redirect behaviors from the old system haven't been carried over yet. This work restores them for the clients that still rely on them. (#327)

- **[Feature]** **Restoring custom pre-ping checks for data clients** — Legacy per-client validation checks that run before serving aren't active on the new platform yet, affecting hundreds of published data clients. This high-priority effort maps and re-enables those checks so the right leads are accepted or rejected. (#338)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging environment loaded with production-like data for verification, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — A helper that reads team conversations and files the action items as tracked issues, reducing manual copying and keeping requests from slipping through the cracks. (#272)

## Modals

- **[Feature]** **Making the Modal Design tab do something (or removing it)** — All six fields on the Modal Design tab currently have no effect on the modal visitors see. Each will either be wired up to display properly or removed from the form. (#294)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form don't match the styling of other forms, with plain-looking text boxes, color pickers, and fields that stack vertically instead of sitting side by side. This tidies up the form's appearance. (#152)

## Reports & Dashboard

- **[Task]** **Confirming Dashboard report numbers match the old system** — During testing, some Dashboard report figures didn't line up with the legacy app. This investigation compares the two over a fixed date range to find any discrepancies, explain them, and confirm the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->
