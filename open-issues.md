# Open Issues — Plain-Language Overview

_Last updated 2026-07-17 11:28:57 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers & Placements
- **[Feature]** **Preview edits before saving** — On placement and offer edit pages, the Preview will show your current in-progress changes instead of only the last saved version, so you can check your work without saving first. (#292)
- **[Feature]** **Placement design settings that actually take effect** — Several placement Design-tab options (like survey height and display format) will finally show up in the live survey, so the choices you make there are reflected for visitors. (#293)
- **[Bug]** **Offer settings reaching the live widget** — Some saved offer options currently get dropped before they reach visitors. This fix ensures the options you configure either work as expected or are cleaned up if they do nothing. (#295)
- **[Bug]** **Success pixels will fire correctly** — A high-priority fix so that conversion tracking pixels set on offers actually fire on success, restoring accurate attribution and revenue tracking that's currently being lost silently. (#297)
- **[Feature]** **Performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, giving Kurt a data-driven gut-check at intake instead of relying on a manual review. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — A high-priority fix so auto-register offers honor age, gender, state, zip, and device targeting rules, preventing them from firing for visitors who should be excluded. (#333)

## Data Clients
- **[Feature]** **Post-conversion delivery steps restored** — Legacy after-success behaviors for certain clients are being brought over to New Adsmith Frontend, so redirects and delivery steps continue working for those data clients. Nearly complete. (#327)
- **[Feature]** **Custom pre-ping checks brought forward** — A high-priority effort to port legacy per-client validation checks (used by hundreds of data clients) so they run again at serve time on the new platform, restoring checks that currently don't fire. (#338)

## Admin & Users
- **[Task]** **Users area review against the old system** — A documentation review comparing the old Users area to the new one, identifying missing pieces (like bulk actions and 2FA status) so nothing important is left behind. (#80)
- **[Feature]** **Removing controls that don't do anything** — Admin settings that look active but currently have no effect (certain Advertiser Web Presence fields, some user permission toggles, and a few data-client options) will be hidden or removed to avoid confusion. (#296)

## Behind the Scenes
- **[Task]** **Safe test environment for verification** — Setting up a read-only staging copy of the product against realistic data, so the team can validate behavior without any risk of changing live records. (#270)
- **[Feature]** **Automatic issue creation from chat** — A helper that turns discussion notes into tracked work items automatically, reducing manual follow-up. This is an internal workflow tool with no effect on the product itself. (#272)

## Surveys
- **[Feature]** **Design choices carry through to the survey** — Every customization option on the Design tab will be checked end-to-end so it reliably shows up in the survey view, with any unused options cleaned up across all screens. (#288)

## Modals
- **[Feature]** **Modal Design tab that works** — The Modal Design tab settings (header title, colors, progress bar) currently don't affect what visitors see. They'll either be wired up to display properly or removed if not needed. (#294)

## Flows
- **[Task]** **Cleaner-looking Flow forms** — Styling fixes for the Flow form so text boxes, color pickers, checkboxes, and paired fields display neatly instead of appearing plain or misaligned. Partially done. (#152)

## Dashboard
- **[Task]** **Making dashboard report numbers match** — An investigation into why some dashboard report figures differ from the old system, so the numbers you rely on are consistent and trustworthy. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->
