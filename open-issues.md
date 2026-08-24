# Open Issues — Plain-Language Overview

_Last updated 2026-08-24 06:11:01 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview unsaved changes on placements and offers** — When editing a placement or offer, the Preview button will show your current edits right away, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Some saved offer settings weren't reaching live pages** — Several options you set on an offer (including the Modal-tab fields, Force More Info Visible, and Display URL) were being saved but never actually applied where visitors see them. Each will be either properly connected or removed so nothing on the form is misleading. (#295)
- **[Bug]** **Manually selected offers now carry over correctly** — On placements set to manual offer delivery, the new platform was showing the wrong or empty offer list because your hand-picked selections weren't being brought over. This fix ensures the same offers appear in the same order as before. (#370)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, giving Kurt a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Reports / Dashboard

- **[Feature]** **Notes on Placements, Advertisers, and Offers** — You'll be able to add short, categorized notes right from an object's detail dashboard and see a recent-notes roll-up on the main Dashboard — restoring a handy feature from the old app, with notes appearing instantly without a page reload. (#382)
- **[Task]** **Confirming report numbers match the old system** — A behind-the-scenes investigation into why some dashboard report totals didn't line up with the legacy app, so you can trust the numbers you see are accurate and consistent. (#271)

## Surveys

- **[Feature]** **Design settings will fully match the survey view** — Every customization you set on the Design tab will actually show up in the survey, and a full check across all screens will make sure no option is silently doing nothing. (#288)
- **[Feature]** **Placement Design-tab settings connected to the live survey** — Options like survey height and display format weren't being applied to what visitors see; these will now take effect, and any leftover unused settings will be cleaned up. (#293)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery steps** — Certain after-success behaviors from the old app (used by active clients) hadn't been carried over. These are being rebuilt as a flexible, configurable step so those clients keep working as expected. (#327)
- **[Feature]** **Bringing back custom pre-check validation for data clients** — A high-priority effort to restore the custom serve-time checks that hundreds of data clients relied on in the old app but which currently don't run, so lead validation behaves the same as before. (#338)

## General / Across the App

- **[Task]** **Users screen comparison with the old app** — A documentation review of what the old Users management offered versus the new Admin area, highlighting gaps like bulk role changes and last-login info to guide upcoming improvements. (#80)
- **[Feature]** **Removing controls that don't do anything** — Several admin settings (such as the Advertiser Web Presence tab, certain user-permission toggles, and a few data-client and pre-ping options) currently save but have no effect. They'll be hidden or removed so the interface only shows controls that actually work. (#296)

## Advertisers

- **[Feature]** **Web Presence links on the Advertiser detail page** — The advertiser's website, social profiles, and a "Search on Google" shortcut will appear as icon links in the page header, using the details already entered on the Web Presence tab. (#383)

## Modals

- **[Feature]** **Making the Modal Design tab actually work** — The Modal Design tab's settings (header title, colors, progress bar, etc.) currently have no effect on what visitors see. Each will either be applied to the visitor modal or removed from the form. (#294)

## Publishers

- **[Bug]** **Pausing a publisher or property will reliably take effect** — A bug meant pausing didn't always stop serving on one of the delivery paths. This fix makes pausing enforced consistently everywhere. (#299)

## Flows

- **[Task]** **Cleaning up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned compared to other forms — text boxes, color pickers, and paired fields don't display correctly. This work tidies up the layout so it matches the rest of the app. (#152)

## Behind the Scenes

- **[Feature]** **Turning Slack conversations into tracked tasks automatically** — An internal tool to capture action items from Slack and log them as tracked work items, reducing manual note-taking. Not user-facing. (#272)
- **[Task]** **Improving the automated testing setup** — Internal maintenance to make the app's automated quality checks more reliable and actually run consistently, helping catch issues before they reach you. (#379)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
