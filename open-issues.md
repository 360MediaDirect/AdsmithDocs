# Open Issues — Plain-Language Overview

_Last updated 2026-07-28 06:50:01 UTC · 15 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers & Placements

- **[Bug]** **Manually selected offers not carried over** — Placements set to show a hand-picked list of offers were coming up empty in New Adsmith Frontend and showing the wrong offers to visitors. This fix makes sure your chosen offers (and their order) match what you set. (#370)
- **[Bug]** **Missing Display/AR controls on the Offer Delivery tab** — On an offer's Delivery tab, you'll again be able to assign a survey to Display or AR mode. The buttons to make that choice were missing, so this restores the ability to set delivery mode without going back to the old system. (#371)
- **[Bug]** **Some saved offer settings weren't reaching visitors** — A number of options you can set on an offer (including its Modal-tab fields and Display URL) weren't actually being applied on the live experience. This ensures each saved setting either takes effect or is cleaned up if it's no longer needed. (#295)
- **[Feature]** **Preview shows your unsaved edits** — When you click Preview on a placement or offer you're editing, you'll see your in-progress changes right away instead of having to save first. (#292)
- **[Feature]** **Placement design settings applied to the live widget** — Design-tab choices on a placement (such as iFrame height and display format) will properly show up in the visitor experience, so what you set is what visitors get. (#293)
- **[Feature]** **Automatic performance estimates for new offers** — An exploratory feature to project how a new offer is likely to perform, based on your past offers and their results — giving you a data-driven gut-check at intake instead of a manual review. (#322)

## Admin / Users

- **[Feature]** **Cleaning up buttons and settings that do nothing** — Several admin controls (an Advertiser Web Presence tab, certain user permission toggles, and a few data-client and pre-ping options) currently look active but have no effect. They'll be hidden or removed so the screens only show settings that actually work. (#296)
- **[Task]** **Reviewing gaps in the Users area** — An ongoing comparison of the old Users management screens against the new ones, to make sure important features (like bulk actions and login details) are accounted for before the new version fully replaces the old. (#80)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery steps** — Behaviors that ran after a successful conversion for certain clients weren't carried over to New Adsmith Frontend. This brings them back in a flexible, configurable way so those clients keep working as before. High progress. (#327)
- **[Feature]** **Bringing over custom pre-check rules** — A large set of clients (hundreds) rely on custom validation that runs before a lead is served, which hasn't been active in the new platform. This is a high-priority effort to restore those checks so leads are validated as they were in the old system. (#338)

## Surveys

- **[Feature]** **Design choices reliably reflected in surveys** — A thorough review to make sure every customization option on the Design tab actually shows up in the survey visitors see, with no settings that quietly do nothing. (#288)

## Modals

- **[Feature]** **Making the Modal Design tab work (or removing it)** — The Modal Design tab's settings (header text, colors, progress bar, and more) don't currently affect the visitor modal. They'll either be wired up to take effect or removed so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear plain or misaligned compared with other screens — text boxes, color pickers, checkboxes, and side-by-side fields. This tidies up the styling so the form looks consistent and polished. (#152)

## Reports & Dashboard

- **[Task]** **Checking dashboard numbers against the old system** — Some Dashboard report figures didn't line up with the legacy system during testing. This investigation pins down where the difference comes from and confirms the numbers can be trusted. (#271)

## Behind the Scenes

- **[Feature]** **Turning conversations into tracked to-dos automatically** — An internal helper that reads team discussions and files the resulting action items for the team, reducing manual note-taking. This has no direct effect on the screens you use. (#272)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
