# Open Issues — Plain-Language Overview

_Last updated 2026-06-28 00:34:43 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open start and end date pickers so you can view dashboard data for any period you like, instead of only the preset options. (#58)
- **[Feature]** **Light mode option for the Admin** — A new theme switcher lets you toggle between the current dark mode and a brand-new light mode, and your choice is remembered between visits. (#59)
- **[Task]** **Bring back the missing Dashboard sections** — A high-priority fix to restore campaign stats, top offers, and watch lists, with the date range properly updating them. (#240)
- **[Feature]** **New "Other Dashboard" views and an activity log** — Adds "Offers with Legs" and "CLP Performance" views (highlighting offers converting under 30%), plus a searchable log of offer and system changes for easy auditing. (#256)
- **[Task]** **Consistent Dashboard colors** — A defined color palette will be applied across dashboard views for cleaner, more readable screens. (#263)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Fixes styling and layout problems so text boxes, color pickers, and paired fields display correctly and match the look of other forms. (#152)
- **[Feature]** **Make the "Step order" setting easy to understand** — A clearer label and inline help will explain what Step order controls and what its values do, so you don't have to guess. (#226)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone else is already editing a record, you'll see a clear "locked by" notice, and you'll be warned before saving over changes made while your screen was open. (#267)
- **[Bug]** **Show an error for invalid links instead of jumping to the Dashboard** — Testing an invalid link will return a clear failure message rather than quietly sending you back to the dashboard. (#239)
- **[Task]** **Use detailed brand guidelines to guide AI output** — A canonical brand-guidelines document will be created and used as the main input to improve the quality of AI-generated content. (#264)

## Campaigns

- **[Feature]** **Add the Campaigns module to New Adsmith Frontend** — A high-priority addition to recreate campaign management from the legacy system, so you can view, create, edit, and configure campaigns and their offer groups. (#200)

## Pre-Pings

- **[Feature]** **Enforce required fields before a lead is sent** — When a pre-ping is set to run before pushing data, leads missing required fields will be stopped up front rather than being sent and relying on the advertiser to catch them. (#218)

## Placements

- **[Feature]** **Better control over selected offers** — You'll be able to set a manual order by default, drag offers to reorder them, remove an offer with an "X" button, and filter the offer list by taxonomy. (#235)

## Users

- **[Task]** **Review of the Users screen versus the legacy version** — A documentation review identifying what's still missing on the new Users screen (such as bulk actions, last-login info, and 2FA status) to guide upcoming improvements. (#80)

## Behind the Scenes

- **[Feature]** **Up-to-date "today" stats** — Behind-the-scenes work so current-day numbers (impressions, clicks, leads, revenue) display accurately on the dashboard. (#34)
- **[Feature]** **Reliable historical stats** — Rolls daily numbers into long-term totals so historical reports stay accurate and fast. (#35)
- **[Task]** **Review an old stats job** — Checking whether an older scheduled stats process is still needed or can be retired. (#33)
- **[Task]** **Safety testing for pre-pings** — Running the new pre-ping system alongside the old one to confirm results match before switching over. (#40)
- **[Feature]** **Per-advertiser pre-ping checks** — Validating each advertiser's pre-ping setup so leads are handled correctly after the switch. (#41)
- **[Task]** **Faster surveys and offers** — High-priority groundwork to add a caching layer that speeds up survey and offer loading. (#42)
- **[Task]** **Roll out new scheduled jobs in parallel** — Running the new automated background jobs alongside the existing ones and watching for differences. (#43)
- **[Task]** **Gradual switch-over of background jobs (lower priority set)** — Retiring older survey-stats jobs once their replacements are proven stable. (#44)
- **[Task]** **Gradual switch-over of background jobs (mid-tier set)** — Retiring additional stats jobs after a monitoring period. (#45)
- **[Task]** **Gradual switch-over of the most critical background jobs** — Carefully retiring the highest-stakes lead-processing and offer-cap jobs, with rollback ready. (#46)
- **[Task]** **Document how to roll things back** — Writing and testing rollback steps for each system in case a change needs to be undone quickly. (#48)
- **[Task]** **Create troubleshooting guides** — Step-by-step guides for the support team to resolve common issues like lead-processing or stats problems. (#49)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 86eeab0d162aa51487d4c3bc27ce14f71ef489b75b1540799dab45fe94fae026 -->
