# Open Issues — Plain-Language Overview

_Last updated 2026-07-19 22:17:28 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing on completed offers** — This is a high-priority fix. When an offer is set up to fire a tracking pixel after a successful conversion, that pixel currently never fires, so conversions can go unrecorded. This will make sure configured success pixels actually fire. (#297)
- **[Bug]** **Some saved offer settings never reach the live offer** — Several options you fill in on the offer form (including Modal-tab fields, Display URL, and certain data-client settings) aren't being carried through to what visitors actually see. This work makes each of those either take effect or be cleanly removed so nothing on the form is misleading. (#295)
- **[Task]** **Auto-register offers ignore visitor targeting** — This is a high-priority fix. Offers that register automatically currently skip the age, gender, state, ZIP, and device rules that normal offers follow, so they can fire for people they should exclude. This aligns them with the same targeting everyone expects. (#333)
- **[Bug]** **"Conflicting Referrals" field has no effect yet** — The Conflicting Referrals box on the offer Delivery tab is saved but doesn't actually exclude any offers. This item confirms the intended rule with the business and then either makes it work or removes the field so it isn't misleading. (#351)
- **[Feature]** **Preview offers and placements with your unsaved edits** — Today the Preview button shows the last saved version, so you have to save before you can see a change. This upgrade lets Preview reflect your current in-progress edits without saving first. (#292)
- **[Feature]** **Predict how a new offer will perform** — An exploratory feature to automatically estimate a new offer's likely performance based on your historical offer data, replacing an informal manual gut-check. It would give a data-grounded projection at offer intake. (#322)

## Surveys

- **[Feature]** **Make sure every Design-tab option actually changes the survey** — A full check across all entities to confirm that each customization option you set on a Design tab is truly reflected in what visitors see, with any dead options fixed or removed. Fewer settings that appear to do nothing. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live survey** — Several Placement Design options (like iFrame height and display format) are saved but not yet applied to the survey widget. This finishes wiring them up, or removes the ones that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore file-based pre-ping checks for data clients** — This is high priority. Hundreds of data clients rely on custom pre-delivery validation from the legacy system that doesn't run on New Adsmith Frontend yet. This work brings that validation back so those clients behave as expected. (#338)
- **[Feature]** **Bring over after-success delivery behavior** — The legacy post-conversion delivery and redirect steps for certain clients weren't carried over. This restores them as a configurable option so post-success handling works again. (#327)

## Admin & Users

- **[Task]** **Compare the new Users area to the legacy one** — A documentation review listing what the legacy Users management had versus the new Admin Users area (things like bulk role changes, last-login and two-factor columns, and password/notification options at creation), so gaps can be prioritized. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings across Advertisers (Web Presence), user permissions, Data-Client, and Pre-Ping are saved but currently have no effect. This hides or removes them so the admin screens only show controls that actually work. (#296)

## Reports & Dashboard

- **[Task]** **Confirm dashboard numbers match the legacy system** — Reviewers noticed report figures that didn't line up with the old system. This investigation pins down where the difference comes from and either fixes it or confirms the numbers are correct, so you can trust the Dashboard reports. (#271)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — Every field on the Modal Design tab (header title, colors, progress bar, etc.) is currently saved but never shown to visitors. This work either makes those settings appear in the visitor modal or removes the tab if it isn't meant to be used. (#294)

## Properties

- **[Bug]** **Enforce the domain allowlist on Properties** — A property's allowed-domains list is currently ignored, so ads can serve from any website even when you've restricted them. This makes the allowlist actually block requests from domains you haven't approved, with no change for properties that leave it empty. (#350)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form look unstyled or misaligned — plain textareas, unstyled color pickers, and paired fields stacking instead of sitting side by side. This tidies up the layout to match the Placement and Modal forms. (#152)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — Standing up a staging copy of New Adsmith Frontend using production-like data for testing, locked to read-only so nothing can be accidentally changed. No user-facing change. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels and automatically files action items as tracked issues, reducing manual copy-and-paste. A behind-the-scenes workflow improvement. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
