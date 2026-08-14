# Open Issues — Plain-Language Overview

_Last updated 2026-08-14 06:27:24 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer options never reach the live display** — Certain offer settings you configure (including the Modal-tab fields, Display URL, and several delivery flags) currently don't carry through to what visitors actually see. Once fixed, the options you set will reliably take effect or be removed if they serve no purpose. (#295)
- **[Bug]** **Restore the Display/AR selection controls on the Delivery tab** — Right now the DISP and AR columns show as headings but have no selectable buttons, so you can't set a survey to Display or AR without going back to the legacy app. This fix brings those controls back so delivery mode can be set and saved. (#371)
- **[Bug]** **Manually selected offers now carry over correctly** — On Manual-delivery placements, the list of hand-picked offers wasn't being brought into New Adsmith Frontend, so the wrong or no offers appeared. This fix makes the selected offers (and their order) match the legacy app. (#370)
- **[Bug]** **Offer edits will show up in History** — Editing an offer currently saves fine but doesn't record an entry in its History section. This fix ensures your changes are logged so you can see who changed what and when. (#380)
- **[Feature]** **Preview your unsaved changes on placements and offers** — The Preview button will show the edits you've made in the form right now, instead of only the last saved version, so you can check your work before committing it. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, New Adsmith Frontend will estimate how a new offer is likely to perform based on your historical offer data, giving you a helpful decision aid at intake. (#322)

## Surveys

- **[Feature]** **Design choices reliably reflected in the live survey** — Every customization option on the Design tab will be checked to confirm it actually changes what visitors see, with any options that do nothing either fixed or removed across all entity screens. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the live survey** — A handful of Placement Design-tab settings (like survey height and display format) either aren't applied or aren't used. This work makes each one take effect in the survey or removes it from the form. (#293)

## Reports & Dashboard

- **[Task]** **Investigate Dashboard report numbers that don't match the legacy system** — Some report figures didn't line up with the old app during testing. This work traces where the difference comes from and confirms the numbers can be trusted. (#271)
- **[Feature]** **Add notes to Placements, Advertisers and Offers** — You'll be able to attach short, categorized notes (with topic and priority) right from a Placement, Advertiser, or Offer detail page, with new notes appearing without a page reload and a recent-notes roll-up on the main Dashboard. (#382)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behaviors** — The legacy "after-success" delivery and redirect steps that ran after a conversion are being brought into New Adsmith Frontend so those clients keep working as before. (#327)
- **[Feature]** **Bring over custom serve-time pre-ping checks (high priority)** — Hundreds of data clients relied on custom validation checks that don't currently run on the new platform. This work restores those checks so lead validation behaves consistently with the legacy app. (#338)

## General / Across the App

- **[Feature]** **Remove admin controls that do nothing** — Several settings (an Advertiser "Web Presence" tab's role in delivery, some user-permission toggles, and a few data-client and pre-ping options) are shown but have no effect. Hiding or removing them prevents confusion and false expectations about what they control. (#296)
- **[Task]** **Comparison of the old and new Users management** — A documentation review lining up the legacy Users screen against the new one to identify what's missing (like bulk actions and 2FA status) and guide upcoming improvements. (#80)

## Modals

- **[Feature]** **Make the Modal Design tab actually work — or remove it** — The Modal Design tab's settings (header title, colors, progress bar, etc.) currently don't change the visitor-facing modal. This work either wires them up so they take effect or removes them if the modal is meant to be header-less. (#294)

## Advertisers

- **[Feature]** **Show Web Presence links on the Advertiser detail page** — The website, social profiles, and a "Search on Google" shortcut you enter in the Web Presence tab will finally appear as icon links in the page header, matching the legacy app (and this time all ten networks are supported). (#383)

## Flows

- **[Task]** **Fix unstyled areas of the Flow form** — Parts of the Flow form (text boxes, color pickers, checkboxes, and paired fields) currently look plain or misaligned compared to other forms. This tidies up the styling so the Flow form matches the rest of the app. (#152)

## Publishers

- **[Bug]** **Pausing a Publisher or Property is enforced everywhere** — A pause could be ignored on one of the serving paths, leading to inconsistent behavior. This fix makes a paused Publisher or Property reliably stop serving. (#299)

## Behind the Scenes

- **[Feature]** **A Slack helper that turns conversations into tracked tasks** — An internal tool to automatically capture action items from Slack discussions and file them as work items, reducing manual note-taking. No direct effect on the product screens. (#272)
- **[Task]** **Strengthen automated testing** — Behind-the-scenes improvements to the automated test suite so it runs reliably and catches issues before they reach you. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
