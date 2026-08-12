# Open Issues — Plain-Language Overview

_Last updated 2026-08-12 06:27:41 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Saved offer settings now reach the live ad** — Some options you set on an offer (including modal settings and display details) weren't being carried through to what visitors actually see. This fix ensures each setting either takes effect or is cleared out if it isn't used. (#295)
- **[Bug]** **Restore Display/AR survey controls on Offer Details** — On an offer's Delivery tab, the controls for assigning a survey to Display or AR went missing. This brings back the ability to set a survey's delivery mode without falling back to the old app. (#371)
- **[Bug]** **Offer edits now appear in History** — Editing an offer wasn't creating a History entry even though the save worked. Once fixed, your changes will show up in the offer's History section. (#380)
- **[Bug]** **Manually selected offers carry over correctly** — Placements set to manual delivery were showing the wrong or no offers because the selected-offer list wasn't brought over from the old system. This makes the same offers appear in the same order as before. (#370)
- **[Feature]** **Preview unsaved changes on placements and offers** — The Preview button will show your current edits before you save, so you can check how a change looks without having to save first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, you'll get a data-driven estimate of how a new offer is likely to perform, based on your own historical offers. This is an early, exploratory effort. (#322)

## Data Clients

- **[Feature]** **Restore custom pre-delivery checks** — High priority. Custom validation that ran before delivery in the old system wasn't running in the new one. This restores those checks so leads are accepted or rejected as intended. (#338)
- **[Feature]** **Restore post-conversion delivery steps** — Certain after-success behaviors from the old system are being brought over so data clients keep working the way they always have. (#327)

## Dashboard

- **[Feature]** **Add notes to Placements, Advertisers, and Offers** — You'll be able to attach short, categorized notes (with topic and priority) to these records and see a recent-notes roll-up on the main Dashboard, just like the old app. (#382)
- **[Task]** **Confirm dashboard numbers match the old system** — Investigating why some dashboard report figures differed from the legacy app, so you can trust that the numbers line up. (#271)

## Surveys

- **[Feature]** **Make sure design options actually change the survey** — Every customization on the Design tab will be reflected in the live survey, with a full check across all screens to catch any options that currently have no effect. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Settings such as survey height and display format will take effect in the live survey, and any unused options will be cleaned up. (#293)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — The Modal Design tab's settings (header text, colors, progress bar) don't currently affect the visitor modal. They'll either be wired up so they take effect, or removed to avoid confusion. (#294)

## General / Across the App

- **[Feature]** **Remove admin controls that don't do anything** — Several saved settings (Advertiser Web Presence fields, certain user-permission toggles, and some Data-Client and Pre-Ping options) currently have no effect. They'll be hidden, removed, or properly implemented so the screens don't imply behavior that isn't there. (#296)
- **[Task]** **Bring the new Users area up to par with the old one** — A review comparing the old and new Users screens to spot missing features (like bulk actions, last-login, and two-factor status) so the new area can reach full parity. (#80)

## Advertisers

- **[Feature]** **Show Web Presence links on Advertiser Details** — The advertiser's website, social profiles, and a "Search on Google" shortcut will appear as icons in the page header, using the information already entered on the Web Presence tab. (#383)

## Publishers

- **[Bug]** **Pausing a publisher or property now fully takes effect** — A pause wasn't being enforced consistently across the system. This makes sure a paused publisher or property is properly blocked everywhere. (#299)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form looked unstyled and some paired fields stacked awkwardly instead of sitting side by side. This tidies up the appearance so it matches the other forms. (#152)

## Behind the Scenes

- **[Feature]** **Slackbot that turns conversations into tracked tasks** — A behind-the-scenes tool that reads Slack conversations, pulls out action items, and files them automatically, reducing manual copy-and-paste work. (#272)
- **[Task]** **More reliable automated testing** — Behind-the-scenes maintenance to strengthen the automated test suite so it runs regularly and catches problems more dependably. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
