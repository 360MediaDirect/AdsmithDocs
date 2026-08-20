# Open Issues — Plain-Language Overview

_Last updated 2026-08-20 06:07:29 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your changes before saving** — On the Placement and Offer edit screens, the Preview button will show the offer or placement exactly as you've edited it, including changes you haven't saved yet, so you no longer have to save first just to see how something looks. (#292)
- **[Bug]** **Saved offer settings that never reached live pages** — Several offer options you can set (including the Modal-tab fields, "Force More Info Visible," Display URL, and some data-delivery flags) were being saved but never actually applied where visitors see them. This fix makes each option either work as expected or be removed so nothing is misleading. (#295)
- **[Feature]** **Automatic performance projection for new offers** — Instead of relying on a manual gut-check, New Adsmith Frontend will estimate how a new offer is likely to perform based on your own historical offer data, giving you a data-driven read at intake time. This is exploratory work with no set deadline. (#322)
- **[Bug]** **Manually chosen offers now carry over correctly** — For placements set to Manual delivery, the list of hand-picked offers (and their order) wasn't coming across to the new platform, so visitors could see the wrong or empty offers. This fix makes the selected offers match what you configured. (#370)

## Surveys

- **[Feature]** **Design settings that actually take effect** — A full sweep across every entity to make sure each Design-tab customization you set is reflected in the live survey, with any options that do nothing being fixed or removed. Less guesswork about which settings matter. (#288)
- **[Feature]** **Placement Design-tab settings wired through to the survey** — Options like survey height and display format, plus a few others, will properly show up in the live survey widget instead of quietly having no effect. (#293)

## Advertisers

- **[Feature]** **Website and social links on the Advertiser page** — The Advertiser details page will show a cluster of quick links (website, social profiles, and a "Search on Google" shortcut) drawn from the Web Presence tab, so the info you enter there is actually visible and usable. (#383)
- **[Feature]** **Notes on your key records** — You'll be able to add short, categorized notes to a Placement, Advertiser, or Offer right from its detail page, and see a recent-notes roll-up on the Dashboard — with your new notes appearing instantly, no page reload needed. (#382)

## Dashboard & Reports

- **[Task]** **Making sure the numbers match** — An investigation into why some Dashboard report figures didn't line up with the older system, so you can trust that the reported numbers are accurate and consistent. (#271)

## Admin & Users

- **[Task]** **Bringing the Users area up to par** — A detailed review of the older Users management screens versus the new ones, identifying missing features (like bulk actions, last-login info, and 2FA status) so the new Users area can catch up. Mostly complete. (#80)
- **[Feature]** **Removing controls that do nothing** — Several admin settings (such as the Advertiser Web Presence fields, certain user-permission toggles, and a few data-client and pre-ping options) currently look active but have no effect. They'll be hidden or removed so the settings you see are the settings that work. (#296)

## Data Clients

- **[Feature]** **Post-conversion delivery steps restored** — Behaviors that used to run after a successful conversion for certain clients weren't carried over to the new platform. This brings them back in a flexible, configurable way. Nearly finished. (#327)
- **[Feature]** **Bringing over custom pre-delivery checks** — Hundreds of data clients relied on custom validation checks that don't yet run on the new platform. This high-priority work maps and restores those checks so client rules are enforced as before. (#338)

## Behind the Scenes

- **[Feature]** **Turning conversations into tracked work automatically** — A helper that reads designated chat channels and files the action items as tracked work items, cutting out manual copy-and-paste after meetings. (#272)
- **[Task]** **Strengthening automated testing** — Fixing gaps in the behind-the-scenes automated checks so problems are caught reliably before they reach you, improving overall stability. (#379)

## Modals

- **[Feature]** **Modal Design tab made real (or retired)** — The Modal Design tab currently saves settings that visitors never see. Each field will either be made to work in the visitor-facing modal or removed, so nothing is misleading. (#294)

## Publishers

- **[Bug]** **Pausing a publisher or property will reliably stop it** — A pause check wasn't working on one delivery path, so pausing didn't always take effect. This fix makes pausing consistent everywhere. (#299)

## Flows

- **[Task]** **Cleaning up the Flow form's appearance** — Parts of the Flow form show unstyled boxes, off-looking color pickers, and fields stacked awkwardly instead of side by side. This tidies up the layout to match the other forms. Partly done. (#152)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
