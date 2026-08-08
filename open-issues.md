# Open Issues — Plain-Language Overview

_Last updated 2026-08-08 06:13:44 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes before saving** — On placement and offer edit pages, the Preview button will show your current in-progress edits instead of the last-saved version, so you can check how a change looks without saving first. (#292)
- **[Bug]** **Saved offer settings that never reached live ads** — Several options you set on an offer (including some modal fields and the display URL) weren't making it through to what visitors actually see. This ensures your saved settings take effect, or removes any that aren't used. (#295)
- **[Feature]** **Automatic performance projections for new offers** — When a new offer comes in, you'll get a data-driven estimate of how it's likely to perform based on similar past offers, replacing the old manual gut-check. A medium-priority, exploratory improvement. (#322)
- **[Bug]** **Manually chosen offers now carry over correctly** — For placements set to manual offer delivery, the specific offers you'd selected were coming through empty, causing the wrong ads to appear. This restores your chosen offers and their order. (#370)
- **[Bug]** **Restore the Display/AR delivery controls** — On the Offer Details Delivery tab, the controls to set a survey to Display or AR were missing. This brings them back so you can set delivery mode without returning to the old app. (#371)
- **[Bug]** **Offer edits will show up in History** — Editing an offer currently doesn't record an entry in its History section. This fix makes your changes appear so you have a clear record of what was changed. (#380)

## Dashboard

- **[Feature]** **Add notes to Placements, Advertisers, and Offers** — You'll be able to attach short, categorized notes directly to these records and see a recent-notes roll-up on the Dashboard, matching what the old app offered. (#382)
- **[Task]** **Making sure Dashboard report numbers match the old system** — We're investigating why some Dashboard report figures differ from the legacy app, so you can trust that the numbers line up. (#271)

## Data Clients

- **[Feature]** **Restore post-conversion delivery steps** — Certain actions that used to run automatically after a successful conversion weren't carried over to the new platform. This brings them back so affected clients behave as before. Nearly complete. (#327)
- **[Feature]** **Restore custom pre-delivery lead checks** — Many data clients rely on custom validation that runs before a lead is delivered, and these weren't active on the new platform. This high-priority work restores them so leads are checked consistently. (#338)

## Surveys

- **[Feature]** **Design choices reliably appear in the survey** — We're making sure every customization option on the Design tab actually shows up in the live survey, and reviewing all entity forms so no setting is a dead end. (#288)
- **[Feature]** **Finish connecting placement design settings** — A few placement Design tab settings (such as survey height and display format) aren't yet affecting the live survey. This wires them up, or removes any that aren't actually used. (#293)

## General / Across the App

- **[Feature]** **Removing settings that don't do anything** — Several admin controls (such as the Advertiser Web Presence fields, some user permission toggles, and certain data-client options) are saved but currently have no effect. These will be made functional or hidden to avoid confusion. (#296)
- **[Task]** **Closing the gap between old and new user management** — A detailed review comparing the old Users area with the new one, to confirm important features like bulk actions and login details aren't missing. (#80)

## Behind the Scenes

- **[Feature]** **Automatic capture of action items from team chats** — A behind-the-scenes helper that turns items discussed in conversations into tracked tasks automatically, reducing manual follow-up. (#272)
- **[Task]** **Strengthening automated testing** — Behind-the-scenes improvements to our automated quality checks so issues are caught before they reach you. (#379)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned, with plain text boxes and fields stacking oddly. This cleans up the layout so it matches the other forms. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The Modal Design tab's settings (header title, colors, progress bar) currently have no effect on what visitors see. These will either be wired up to actually display, or removed. (#294)

## Publishers

- **[Bug]** **Pausing a publisher or property will reliably take effect** — Due to a mismatch, pausing wasn't always being enforced on one of the delivery paths. This ensures a paused publisher or property is properly stopped everywhere. (#299)

## Advertisers

- **[Feature]** **Show advertiser website and social links on the detail page** — The Advertiser Details page will display quick-access icons for the advertiser's website, social profiles, and a Google search, using the information already entered on the Web Presence tab. (#383)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
