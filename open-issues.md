# Open Issues — Plain-Language Overview

_Last updated 2026-07-31 06:56:05 UTC · 17 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes before saving** — On placement and offer edit pages, the Preview button will show exactly what you've just changed, instead of only the last saved version. You'll be able to check your work before committing it. (#292)
- **[Bug]** **Some saved offer options weren't reaching live campaigns** — A behind-the-scenes gap was dropping certain offer settings (like the modal-tab fields, Display URL, and several delivery flags) before they went live. This fix makes sure the options you set actually take effect, or clearly removes ones that were never used. (#295)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool that estimates how a new offer is likely to perform, based on your own historical offer data, replacing the old manual gut-check review. It would give you a data-grounded read on an offer at intake time. (#322)
- **[Bug]** **Manually selected offers now carry over correctly** — For placements set to Manual delivery, the specific offers you chose weren't being brought into New Adsmith Frontend, so the wrong offers displayed. This fix ensures your selected offers (and their order) match what you configured. (#370)
- **[Bug]** **Restoring Display/AR controls on offer delivery** — On the Offer Details Delivery tab, the buttons to set a survey to Display or AR were missing, so you couldn't assign a delivery mode. This brings those controls back so you can configure delivery without switching to the old app. (#371)

## Surveys

- **[Feature]** **Design tab settings will show up in the live survey** — A full check to make sure every customization option on the Design tab actually changes what visitors see, with no dead options that appear to do something but don't. (#288)
- **[Feature]** **Placement design settings will affect the live widget** — Several Placement Design-tab settings (like survey height and display format) weren't being applied to what visitors see. Each one will either be wired up to work or removed so nothing on the form is misleading. (#293)

## Data Clients

- **[Feature]** **Post-conversion delivery steps brought over from the old system** — The "after success" behaviors that run once a visitor converts weren't carried into New Adsmith Frontend. This restores that functionality for the clients that rely on it. (#327)
- **[Feature]** **Restoring custom pre-check validation for data clients** — Hundreds of data clients used custom serve-time checks in the old system that currently don't run on the new platform. This high-priority work reconnects those checks so pausing and validation behave consistently. (#338)

## Admin / Users

- **[Task]** **Reviewing what's still missing in the Users area** — A detailed comparison between the old Users management and the new one, highlighting gaps like bulk actions, extra columns, and filters, so the team knows what to add next. (#80)
- **[Feature]** **Cleaning up admin controls that don't do anything** — Some settings (certain Advertiser web-presence fields, a couple of user permission toggles, and a few data-client and pre-ping options) are shown but currently have no effect. They'll be hidden or removed so nothing implies control it doesn't have. (#296)

## Behind the Scenes

- **[Feature]** **Turning team conversations into tracked work automatically** — A helper that reads designated chat channels and files the action items as tracked issues, so requests raised in conversation don't get lost. (#272)
- **[Task]** **Strengthening our automated testing** — A review of the automated checks that guard the app turned up several ways to make them more reliable and to run them more consistently, reducing the chance of issues slipping through. (#379)

## Modals

- **[Feature]** **Making the Modal Design tab actually work** — The entire Design tab for Modals currently saves settings that never appear to visitors. Each field will either be built into the visitor-facing modal or removed so the tab isn't misleading. (#294)

## Publishers

- **[Bug]** **Pausing a publisher or property will reliably take effect** — A pause check wasn't matching correctly, so pausing didn't always stop serving on one of the paths. This makes pause enforcement consistent everywhere. (#299)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Parts of the Flow form appear unstyled, with plain textareas and fields stacking awkwardly instead of sitting side by side. This work brings the form in line with the cleaner look of the Placement and Modal forms. (#152)

## Reports

- **[Task]** **Confirming dashboard numbers match the old system** — During testing, some dashboard report figures didn't line up with the old app. This investigation pins down where the difference comes from and confirms the numbers you see are accurate. (#271)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
