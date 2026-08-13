# Open Issues — Plain-Language Overview

_Last updated 2026-08-13 06:27:53 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview edits before saving** — On placement and offer edit pages, the Preview button will show your current in-progress changes instead of the last-saved version, so you can check how something looks without saving first. (#292)
- **[Bug]** **Some saved offer settings never reach live pages** — Several offer options (including the Modal-tab fields, Display URL, and a handful of data-client settings) are saved but don't currently affect what visitors see. This fix makes each option either work as expected or be cleanly removed so nothing is misleading. (#295)
- **[Bug]** **Display vs. AR controls missing on the Delivery tab** — On an offer's Delivery tab, the DISP and AR columns show as headers only, with no way to actually set a survey to Display or AR. This restores those selectable controls so you can configure delivery mode without going back to the legacy app. (#371)
- **[Bug]** **Manually selected offers not carried over from the old app** — On Manual-delivery placements, the "Selected Offers" list is coming up empty in New Adsmith Frontend even though it's populated in the legacy app, causing the wrong offers to display. This restores the correct selected offers and their order. (#370)
- **[Bug]** **Offer edits not showing in History** — Editing and saving an offer isn't recording an entry in the offer's History section. This fix ensures your changes are properly logged so there's a reliable record of what changed. (#380)
- **[Feature]** **Automatic performance projections for new offers** — Explores replacing today's manual "gut-check" review with a data-driven estimate of how a new offer is likely to perform, based on your own historical offer data — giving Kurt a quick read at intake time. (#322)

## Dashboard

- **[Task]** **Investigate dashboard report numbers vs. the legacy app** — Some dashboard report figures don't match the old system, making it hard to trust the numbers. This work pins down where the difference comes from and either fixes it or confirms the figures are correct. (#271)
- **[Feature]** **Add and view notes on Placement, Advertiser, and Offer dashboards** — Brings back the ability to attach short, categorized notes (with topic and priority) to a placement, advertiser, or offer, plus a recent-notes roll-up on the main Dashboard — matching what the legacy app offered. (#382)

## Surveys

- **[Feature]** **Design-tab customizations that actually show up** — Ensures every option on the Design tab is reflected in the live survey view, and audits all entity forms so no setting is left doing nothing. You'll get customizations that behave the way the form implies. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey widget** — Several Placement Design-tab settings (like survey height and display format) are saved but don't yet affect the widget. This wires them through so your choices take effect, or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — Certain after-success delivery steps from the legacy app weren't carried over. This work re-adds them so those clients' post-conversion handling works as before. (#327)
- **[Feature]** **Restore custom pre-delivery validation checks** — Hundreds of data clients rely on legacy serve-time validation that currently doesn't run in New Adsmith Frontend. This high-priority work reconnects those checks so leads are validated correctly before delivery. (#338)

## Admin Area

- **[Task]** **Users screen catch-up with the legacy app** — A review comparing the old Users area with the new one, identifying missing pieces like bulk actions, extra columns, and password options so the new Users screen reaches full parity. (#80)
- **[Feature]** **Remove admin settings that don't do anything** — Several controls (Advertiser Web Presence fields, certain user-permission toggles, and a few data-client and pre-ping options) are shown but currently have no effect. This hides or removes them so the admin screens don't imply features that aren't there. (#296)

## Modals

- **[Feature]** **Make the Modal Design tab work — or retire it** — The Modal Design tab's settings (header title, colors, progress bar, etc.) are saved but don't currently change what visitors see. This wires them up so they take effect, or removes the tab if the modal is meant to be header-less. (#294)

## Publishers

- **[Bug]** **Pausing a publisher or property doesn't always take effect** — Because of an internal mismatch, pausing a publisher or property isn't being fully enforced on one of the serving paths. This fix makes a pause reliably stop serving everywhere. (#299)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned compared to other forms — plain textareas, unstyled color pickers and checkboxes, and fields stacking instead of sitting side by side. This work brings the Flow form's look in line with the rest of the product. (#152)

## Advertisers

- **[Feature]** **Show Web Presence links on the Advertiser detail page** — The website, social profiles, and a "Search on Google" shortcut are captured on the edit form but never displayed. This adds the familiar cluster of icon links to the Advertiser detail header. (#383)

## Behind the Scenes

- **[Feature]** **Slack-to-issue helper** — An internal tool to turn Slack conversations into tracked work items automatically, reducing manual copy-and-paste when logging follow-ups. No visible change in the product. (#272)
- **[Task]** **Automated-testing improvements** — Behind-the-scenes cleanup of the automated test suite to close coverage gaps and reduce false results, helping catch issues before they reach you. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
