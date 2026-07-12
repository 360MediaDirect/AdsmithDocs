# Open Issues — Plain-Language Overview

_Last updated 2026-07-12 19:24:50 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — A high-priority fix: pixels set up to fire when an offer converts were silently not firing, meaning conversions weren't being recorded. Once fixed, configured success pixels will fire reliably and attribution will be accurate again. (#297)
- **[Task]** **Auto-register offers ignore visitor targeting** — A high-priority fix: offers that fire automatically on page load were reaching visitors who should have been excluded by age, gender, state, ZIP, or device rules. This will make sure those offers respect the same targeting as everything else. (#333)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several options you can set on an offer (including Modal-tab fields, Display URL, and certain data-client flags) were being saved but not actually used by the live widget. Each will be properly connected or removed so what you configure is what visitors see. (#295)
- **[Feature]** **Preview offers and placements with your unsaved edits** — Today the Preview button shows the last saved version. You'll be able to preview your in-progress changes before saving, so you can check your work without committing it first. (#292)
- **[Feature]** **Predict how a new offer will perform** — An exploratory tool that estimates a new offer's likely performance based on your historical offer data, replacing the current manual gut-check review. (#322)

## Admin / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is already editing a record, you'll see who has it open and be warned before your changes could overwrite theirs. This protects against accidental lost changes across all entity screens. (#267)
- **[Feature]** **Searchable history of every change** — A new Audit Log will record who changed what and when, across offers, placements, advertisers, and more (including automated changes). Administrators will be able to search and review this history to answer "who changed this?". (#276)
- **[Feature]** **Clean up controls that don't do anything** — Some settings (like the Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) are saved but have no effect. These will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Compare the new Users screen against the old one** — A documentation review identifying which features from the legacy Users area still need to be brought over to New Adsmith Frontend, so nothing important is missed. (#80)
- **[Task]** **Decide the future of the file-share page** — The old file-share page has no equivalent yet. This is a decision on whether to rebuild it or retire it. (#328)

## Surveys & Modals

- **[Feature]** **Make sure every survey design option actually changes the survey** — A review across all screens to confirm each design/customization setting is fully connected from the form through to what visitors see, with any dead options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings** — A handful of Placement Design-tab settings (like iFrame height and display format) aren't yet reflected in the live survey widget. Each will be wired up or removed so the tab behaves as expected. (#293)
- **[Feature]** **Fix or remove the Modal Design tab** — The entire Modal Design tab is currently saved but never shown to visitors. Its fields will either be made to display in the modal or removed from the form. (#294)

## Behind the Scenes

- **[Task]** **Check that report numbers match the legacy system** — An investigation into why some dashboard report figures didn't line up with the old system, to pinpoint the cause and confirm the numbers can be trusted. (#271)
- **[Task]** **Set up a safe, read-only test environment** — Standing up a staging environment loaded with production-like data for testing and verification, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads designated chat conversations and files the identified action items as tracked issues, reducing manual copy-and-paste. (#272)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back file-based pre-ping validation** — A high-priority effort to restore custom validation checks (used by hundreds of data clients) that ran in the old system but aren't yet running in New Adsmith Frontend, so those checks apply again. (#338)
- **[Feature]** **Restore after-success delivery for data clients** — The old post-conversion delivery/redirect behavior for certain clients wasn't carried over. This ports it as a reusable, configurable option so those clients work as before. (#327)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly instead of sitting side by side. This tidies up the form so it matches the polished look of the Placement and Modal forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — A high-priority, core feature that's missing today: you'll be able to view, create, edit, and configure campaigns and offer groups in New Adsmith Frontend, just like in the legacy admin. (#200)

## General / Across the App

- **[Bug]** **Testing an invalid link should show an error, not send you to the Dashboard** — When you test a bad link, you'll get a clear failure message right where you're testing instead of being unexpectedly bounced to the Dashboard. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
