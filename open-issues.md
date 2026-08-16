# Open Issues — Plain-Language Overview

_Last updated 2026-08-16 06:06:06 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your changes before saving** — On the Placement and Offer edit screens, the Preview will show exactly what you've just typed in, including edits you haven't saved yet, so you no longer have to save first just to check how something looks. (#292)
- **[Bug]** **Some saved offer options weren't reaching live pages** — Several offer settings you can fill in (including Modal-tab fields, "Force More Info Visible," Display URL, and certain data-delivery flags) were being saved but never actually used on the live experience. We're fixing each one so it either takes effect or is removed to avoid confusion. (#295)
- **[Feature]** **Automatic performance projections for new offers** — Exploring a way to estimate how a new offer is likely to perform based on your own historical offer data, giving Kurt a data-driven gut-check at intake instead of relying on a manual review. (#322)
- **[Bug]** **Set surveys to Display or AR again** — On the Offer Details Delivery tab, the controls for assigning a survey to Display or AR are currently missing. This fix restores those selectable options so you can configure delivery mode without going back to the old app. (#371)
- **[Bug]** **Offer edits will show up in History** — Right now, changing a field on an offer doesn't always create a History entry, so the record looks like nothing changed. This fix makes sure every real edit is recorded with who made it and when. (#380)
- **[Bug]** **Manually selected offers now carry over correctly** — On Manual-delivery placements, the list of hand-picked offers wasn't transferring from the old app, leaving the "Selected Offers" panel empty and showing the wrong offers to visitors. This fix preserves your selected offers and their order. (#370)

## Surveys

- **[Feature]** **Design-tab customizations actually show in the survey** — Making sure every option on the Design tab is fully connected to what visitors see, and checking every entity's form so no setting is a dead end that quietly does nothing. (#288)
- **[Feature]** **Finish connecting Placement Design settings** — A handful of Placement Design-tab options (like iFrame height, display format, and skip/more-info toggles) are saved but not yet reflected in the live widget. This finishes wiring them up so they take effect, or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — Certain after-conversion delivery and redirect steps from the old system hadn't been carried over. This brings them back so those clients keep working as before. (#327)
- **[Feature]** **Bring back custom pre-delivery checks** — A large group of data clients relied on custom validation that runs before a lead is delivered, and that logic wasn't active on the new platform. This high-priority work restores those checks so leads are validated consistently. (#338)

## Admin / Users

- **[Task]** **Closing the gap on the Users area** — A detailed comparison of the old and new Users screens to identify what's missing (like bulk actions, last-login and two-factor details, and password/notification options) and prioritize bringing those capabilities into New Adsmith Frontend. (#80)
- **[Feature]** **Remove buttons and fields that don't do anything** — Some admin controls (Advertiser Web Presence fields, certain user-permission toggles, and a few data-client and pre-ping options) are saved but have no effect. We're hiding or removing them so nothing implies a capability that isn't really there. (#296)

## Dashboard & Reports

- **[Task]** **Making sure report numbers match the old system** — Dashboard report figures didn't line up with the legacy app during testing. We're comparing the two over a fixed date range to find where the difference comes from and confirm the numbers are trustworthy. (#271)
- **[Feature]** **Add notes to Placements, Advertisers, and Offers** — Bringing back the ability to attach short, categorized notes to a Placement, Advertiser, or Offer from its detail page, with a recent-notes roll-up on the main Dashboard, so your team can leave context right where it's needed. (#382)

## Modals

- **[Feature]** **Make the Modal Design tab actually work** — Every field on the Modal Design tab (header title, subtitle, colors, progress bar, and more) currently saves but never appears in the visitor modal. This will either connect those fields so they display or remove the tab if the modal is meant to be header-less. (#294)

## Publishers

- **[Bug]** **Pausing a publisher or property will reliably stop serving** — A check meant to honor a paused publisher or property wasn't working on one of the serving paths, so pausing didn't always take effect. This fix makes pausing enforced consistently. (#299)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or stacked awkwardly compared to other forms. This is a careful cleanup so text boxes, color pickers, checkboxes, and paired fields look right without breaking the other tabs. (#152)

## Advertisers

- **[Feature]** **Show advertiser website and social links on their detail page** — The website, social profiles, and a "Search on Google" shortcut you enter on the Web Presence tab aren't currently displayed. This adds that cluster of icon links to the Advertiser Details header, opening safely in a new tab. (#383)

## Behind the Scenes

- **[Feature]** **A helper to turn conversations into tracked work items** — A tool that reads designated chat conversations and automatically files the action items as tracked issues, reducing manual copy-paste when capturing follow-ups from meetings. (#272)
- **[Task]** **Strengthening our automated testing** — An internal review of our automated test coverage found a few gaps (tests that were silently skipping, not running automatically, or timing-sensitive). Addressing these makes our quality checks more reliable, with no direct change to the screens you use. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
