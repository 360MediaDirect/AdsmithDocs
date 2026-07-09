# Open Issues — Plain-Language Overview

_Last updated 2026-07-09 22:30:10 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When you open a record to edit, the app will hold it for you and warn if someone else already has it open, so two people can no longer unknowingly save over each other's changes. (#267)
- **[Feature]** **A searchable history of who changed what** — Administrators will get an Audit Log that records every change to offers, placements, advertisers, and other records — including automated changes — with a timestamp and who made it, making it easy to answer "who changed this and when?" (#276)
- **[Feature]** **Cleaning up controls that don't actually do anything** — Several settings that appear to work but have no effect (like the Advertiser Web Presence fields, certain user permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden, so what you see in the admin reflects what really happens. (#296)
- **[Task]** **Users screen brought in line with the old system** — A review is underway comparing the new Users area to the legacy one, so missing capabilities (like bulk actions and extra columns) can be added back. This is documentation/planning work that's mostly done. (#80)
- **[Bug]** **Invalid link tests now show a clear error** — When you test a link that isn't valid, you'll see a proper error message instead of being dropped back onto the dashboard. This fix is nearly finished. (#239)
- **[Task]** **Decision on the old file-share page** — We're confirming whether the legacy file-share page is still used by anyone before deciding to rebuild or retire it. (#328)

## Offers

- **[Bug]** **Success tracking pixels weren't firing** — Conversion pixels set up on offers were silently never firing, meaning lost tracking. This fix makes configured success pixels reliably fire when a conversion happens. (#297)
- **[Bug]** **Some saved offer settings weren't reaching the live page** — A number of saved offer options (including modal settings, Display URL, and several backend flags) never made it through to the live offer, so they had no effect. Each will be either properly connected or removed. High priority. (#295)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Certain automatic offers fire for every visitor regardless of age, gender, state, zip, or device targeting. This fix makes them respect the same targeting rules as regular offers, so they only show to the intended audience. High priority. (#333)
- **[Bug]** **bPerx voucher code missing from offer preview** — The voucher code line isn't showing in the offer preview on the test site. We're tracing why the code lookup fails so the voucher appears correctly in both the preview and the live survey. (#344)
- **[Feature]** **Automatic performance estimates for new offers** — We're exploring a way to estimate how a new offer is likely to perform based on your historical offer data, replacing the current informal manual review. Exploratory, no deadline. (#322)

## Surveys

- **[Feature]** **Making sure every design option actually takes effect** — We're checking that all design-tab customizations flow through to the live survey, and reviewing form options across every screen so there are no settings that look active but do nothing. (#288)
- **[Bug]** **Voucher code and info links missing on live survey** — A configured voucher code and the privacy/terms/details links aren't appearing on the new survey page even though they're saved in the admin. This fix restores both, which matter for passing leads and for compliance. High priority. (#291)
- **[Feature]** **Finishing the Placement design settings on the survey** — Several Placement design-tab settings (like survey height and display format) are saved but not yet shown on the survey. This work connects them so your choices actually appear. (#293)

## Reports

- **[Task]** **Confirming report numbers match the old system** — Dashboard report figures didn't line up with the legacy app during testing. We're comparing the two over a fixed date range to find and explain any differences and confirm the numbers can be trusted. (#271)
- **[Feature]** **Historical placement reports showing zero offer impressions** — Older placement reports display "0" for offer impressions because that figure wasn't being recorded. This adds it so historical reports show the real numbers. (#339)

## Pre-Pings

- **[Feature]** **Real-time offer checks before showing an offer** — For offers set to check at display time, the app will now perform the live advertiser check and hide the offer if it's rejected, matching the old system's behavior. High priority. (#337)
- **[Feature]** **Restoring custom pre-check rules for data clients** — Hundreds of data clients relied on custom validation checks that don't yet run on the new platform. This work brings those checks back so offers are properly validated at serve time. High priority. (#338)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of the app using production-like data for verification and testing, locked to read-only so nothing can be accidentally changed. Mostly complete. (#270)
- **[Feature]** **Turning conversations into tracked tasks automatically** — A helper that reads designated chat conversations and files them as tracked work items, reducing manual copy-and-paste. (#272)

## Placements

- **[Feature]** **Preview reflects your unsaved changes** — On placement and offer edit screens, the Preview button will show your current edits instead of only the last-saved version, so you can check changes before saving. (#292)

## Data Clients

- **[Feature]** **Restoring post-conversion delivery behavior** — Custom actions that ran after a successful conversion for certain clients weren't carried over. This work brings that behavior back in a flexible, configurable way. Nearly complete. (#327)

## Modals

- **[Feature]** **Making the Modal design settings work (or removing them)** — The Modal Design tab's six fields currently have no effect on the visitor-facing modal. Each will be either wired up to actually display or removed from the form. (#294)

## Flows

- **[Task]** **Fixing the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned compared to other forms. This tidies up the layout and styling, with a careful approach so other tabs aren't affected. Partially done. (#152)

## Campaigns

- **[Feature]** **Bringing the Campaigns area to the new platform** — Campaign management from the old admin isn't available yet in the new platform. This adds the ability to view, create, edit, and configure campaigns and their offer groups. Critical and high priority. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 20c05265760e30b087db164aa9ffb7701fea9cb19d23bb2497ef9c503a36041b -->
