# Open Issues — Plain-Language Overview

_Last updated 2026-07-18 16:18:27 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Conversion tracking pixels aren't firing** — A high-priority fix so that the success pixels you set up on an offer actually fire when a conversion happens. Right now they silently do nothing, which means lost tracking; once fixed, your configured pixels will fire reliably. (#297)
- **[Task]** **Auto-register offers now respect visitor targeting** — A high-priority fix so that auto-register offers honor the same age, gender, state, ZIP, and device rules as regular offers. Today they can fire for visitors they should exclude; this brings them back in line with your targeting settings. (#333)
- **[Bug]** **Saved offer options that never reached live ads** — Several options you set on an offer (including some Modal-tab settings and display details) weren't actually being carried through to what visitors see. This fix makes sure the choices you save take effect, or clearly removes options that were never meant to be there. (#295)
- **[Bug]** **"Conflicting Referrals" field will finally do something** — This offer field can be filled in today but has no effect at all. It'll either be wired up to properly exclude offers or removed after confirming the intended behavior, so you're never configuring something that quietly does nothing. (#351)
- **[Feature]** **Preview shows your unsaved edits** — On placement and offer edit pages, the Preview button will reflect the changes you're currently making instead of only the last-saved version. You'll be able to check your edits without having to save first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your existing offers and their history, giving Kurt a data-driven read at intake instead of relying on a manual review. (#322)

## Surveys

- **[Feature]** **Design choices reliably show up in the live survey** — A cross-product review to make sure every option on the Design tab (and other entity forms) actually appears in the survey visitors see. Any option that isn't connected end-to-end will be fixed or removed, so nothing you configure is ignored. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live widget** — Several placement design settings (like survey height and display format) are saved but not yet reflected in the widget. This wires them through so they take effect, and cleans up any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Bring back post-conversion delivery behavior** — The "after-success" steps that run once a lead converts (used by clients like bperx and rwdb) weren't carried over to New Adsmith Frontend. This restores that behavior in a flexible, configurable way. (#327)
- **[Feature]** **Restore custom pre-serve validation for data clients** — A high-priority effort to port the older per-client pre-ping checks (used by hundreds of published data clients) that currently don't run at all on the new platform. Once done, those clients' custom validation will properly pass or reject at serve time again. (#338)

## Admin & Users

- **[Task]** **Bringing the Users area up to par with the old system** — A detailed review comparing the older Users management screen with the new one, so missing pieces like bulk actions, extra columns, and filters can be prioritized and added. (#80)
- **[Feature]** **Removing admin controls that don't do anything** — Some settings across Advertisers (Web Presence), user permissions, Data-Client, and Pre-Ping look like they work but currently have no effect. These will be hidden or removed so the admin screens only show controls that genuinely do something. (#296)

## Behind the Scenes

- **[Task]** **A safe test environment using real-world-like data** — Setting up a read-only staging copy of New Adsmith Frontend against production-like data, so the team can verify behavior without any risk of changing live records. (#270)
- **[Feature]** **Automatically turning conversations into tracked work items** — A helper that reads designated chat channels and files the resulting to-dos as tracked issues, cutting out manual copy-and-paste when capturing action items from meetings. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — Every field on the Modal Design tab currently saves but has no visible effect for visitors. These will either be connected so they change the modal's header and progress bar, or removed if the modal is meant to stay header-less. (#294)

## Properties

- **[Bug]** **Honoring a property's allowed-domains list** — A property can be set up with a list of approved website addresses, but today ads still serve from any site regardless. This fix makes the allowlist actually block requests from sites that aren't on it, while leaving properties that haven't set one unaffected. (#350)

## Dashboard

- **[Task]** **Making sure report numbers match the old system** — Investigating why some Dashboard report figures differ from the legacy app, pinpointing where the difference comes from, and either fixing it or confirming the numbers are correct. This gives you confidence the reports you rely on are accurate. (#271)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Parts of the Flow form currently appear unstyled or awkwardly laid out (plain text boxes, misaligned paired fields, unstyled color pickers). This carefully cleans up the form's appearance to match the polished look of the Placement and Modal forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
