# Open Issues — Plain-Language Overview

_Last updated 2026-08-27 09:00:32 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on placements and offers** — When editing a placement or offer, the Preview button will show the exact changes you've made even before you save, so you can check your work without saving first. (#292)
- **[Bug]** **Some saved offer settings weren't reaching the live offer** — Several offer options (including the Modal-tab fields, Display URL, and a few data-client settings) were being saved but never actually used where visitors see them. This fix ensures each option is either applied or cleaned up so nothing looks active when it isn't. (#295)
- **[Feature]** **Automatic performance projection for new offers** — Instead of relying on a manual gut-check, new offers could be scored against your own historical offer performance to estimate how they're likely to do. This is an early exploration to give a helpful, data-based preview at intake. (#322)
- **[Bug]** **Manually selected offers now carry over correctly** — On placements set to Manual delivery, the specific offers you hand-picked (and their order) weren't coming across to New Adsmith Frontend, so the wrong offers displayed. This fix makes the new app show the same selected offers as before. High priority; nearly complete. (#370)
- **[Feature]** **Filters for the Conflicting Offers section** — You'll be able to narrow the Conflicting Offers list by status, type, vertical, and group, just like you already can on the Display Offers tab, making it much easier to manage. (#385)

## Dashboard

- **[Task]** **Making dashboard report numbers match the old system** — During testing, some dashboard report totals didn't line up with the legacy app. This high-priority review pins down exactly where the numbers diverge and confirms the new reports can be trusted. (#271)
- **[Feature]** **Add and view notes on Placements, Advertisers, and Offers** — Bringing back the ability to attach short, categorized notes (with a topic and priority) to a placement, advertiser, or offer from its detail screen, plus a recent-notes roll-up on the main Dashboard. Notes will appear right away without needing a page reload. (#382)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery steps** — Certain after-conversion delivery and redirect behaviors from the old system hadn't been carried over yet. This brings them back as a flexible, configurable option so those clients keep working as expected. Nearly complete. (#327)
- **[Feature]** **Restoring custom pre-check validation for data clients** — Many data clients relied on custom serve-time checks that weren't yet active in New Adsmith Frontend. This high-priority, large effort re-establishes those checks so leads are validated the same way they were before, with safe fallbacks if anything errors. (#338)

## Surveys

- **[Feature]** **Design settings will fully show up in the survey view** — Every customization on the Design tab will be reflected in what visitors actually see, and a full check across all entity forms will confirm no option is left doing nothing. (#288)
- **[Feature]** **Finishing the Placement Design-tab settings** — A handful of placement design options (like survey height and display format) weren't yet influencing the live widget. This wires them up so your choices take effect, and cleans up any options that were purely decorative. (#293)

## General / Across the App

- **[Task]** **Closing the gap between the old and new Users area** — A detailed comparison of the legacy Users management screen against the new one, identifying missing capabilities (like bulk actions and login/2FA info) so the new Users area can catch up. Mostly done. (#80)
- **[Feature]** **Removing admin controls that don't do anything** — Several settings across Advertisers, Users, Data Clients, and Pre-Pings were saved but never actually used, which is confusing and misleading. These will be hidden or removed (or properly implemented) so every control you see does what it appears to do. (#296)

## Modals

- **[Feature]** **Making the Modal Design tab actually work** — The Modal Design tab's header and progress-bar settings weren't affecting the modal visitors see. This either wires those six fields through so they take effect, or removes them if the modal is intentionally header-less. (#294)

## Flows

- **[Task]** **Tidying up the Flow form's appearance** — Parts of the Flow form looked unstyled or broken, with plain text boxes and fields stacked awkwardly instead of side by side. This clean-up brings its look in line with the Placement and Modal forms. Partially done. (#152)

## Publishers

- **[Bug]** **Pausing a publisher or property will reliably stop delivery** — A pause could be ignored on one of the serving paths, so a paused publisher or property might still serve. This high-priority fix makes the pause take effect consistently everywhere. (#299)

## Behind the Scenes

- **[Feature]** **A helper that turns Slack conversations into tracked tasks** — An assistant that reads designated Slack channels, spots action items, and files them as tracked issues automatically, cutting out manual copy-and-paste. (#272)
- **[Task]** **Strengthening the automated testing suite** — An internal review of the app's automated tests found gaps (some tests silently skipping, tests not running automatically, and occasional flakiness). Addressing these makes future releases more reliable. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
