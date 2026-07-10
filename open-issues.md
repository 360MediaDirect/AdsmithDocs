# Open Issues — Plain-Language Overview

_Last updated 2026-07-10 00:30:41 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes before saving** — On the offer and placement edit screens, the Preview will show exactly what you've typed in right now, instead of the last version you saved, so you can check a change before committing to it. (#292)
- **[Bug]** **Saved offer settings not reaching the live page** — Several offer options you set up (including modal settings and "Force More Info Visible") aren't currently making it through to what visitors see. This fix ensures the options you configure actually take effect, or removes any that do nothing. (#295)
- **[Bug]** **Success tracking pixels not firing** — High priority. Conversion pixels set up on offers are silently not firing, which means lost tracking. This fix makes configured success pixels reliably fire when a conversion happens. (#297)
- **[Bug]** **Auto-register offers ignoring audience targeting** — High priority. Certain automatic offers are firing for visitors who should be excluded by age, gender, state, zip, or device rules. This fix makes them respect the same targeting as regular offers. (#333)
- **[Bug]** **Voucher code missing from offer preview** — For bPerx offers, the "Your Voucher Code" line isn't showing in the preview on the test environment. This fix restores the voucher code so previews (and live pages) match the older system. (#344)
- **[Feature]** **Predict how a new offer will perform** — A new tool that estimates an incoming offer's likely performance based on your historical offer data, replacing the old manual gut-check review. This is exploratory with no set deadline. (#322)

## General / Across the App

- **[Task]** **Bringing the Users area up to par with the old system** — A review of the older Users management screens against the new ones to close feature gaps, such as bulk role changes, last-login and two-factor status, and password setup during user creation. (#80)
- **[Bug]** **Testing a bad link now shows a clear error** — Currently, entering an invalid link quietly sends you to the Dashboard. This fix makes the Link Testing screen show a proper error result instead. (#239)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When two users open the same record, the app will warn that someone else is editing it and stop unsaved changes from being silently wiped out, protecting your work across all entity screens. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log showing who changed what and when, across offers, placements, advertisers, and more, including automatic system changes. Makes it easy to trace and troubleshoot changes. (#276)
- **[Feature]** **Tidy up controls that don't do anything** — Some admin fields (like Advertiser web-presence links and a few user-permission and data-client toggles) are saved but have no effect. This work removes or hides them so the screens only show controls that actually work. (#296)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent in New Adsmith Frontend. This determines whether it's still needed and should be rebuilt, or retired for good. (#328)

## Surveys

- **[Feature]** **Make sure every design option actually shows up** — A thorough check that every customization you set on the design tabs is carried all the way through to what visitors see on the survey, with any dead options fixed or removed. (#288)
- **[Bug]** **Voucher code and info links missing on the live survey** — High priority. A configured voucher code and the privacy/terms/details links aren't appearing on the new survey page even though they're saved. This fix restores both, which matter for compliance and passing leads. (#291)
- **[Feature]** **Finish connecting placement design settings to the survey** — A handful of placement design-tab settings (like survey height and display format) aren't yet reflected on the survey. This wires them through so they take effect, or removes them if unused. (#293)

## Pre-Pings

- **[Feature]** **Real-time offer checks at display time** — High priority. Restores the behavior where a display-triggered check actually contacts the advertiser and hides the offer if it's rejected, matching the older system. (#337)
- **[Feature]** **Bring back per-client validation checks** — High priority. Many data clients rely on custom validation that isn't running in the new platform yet. This ports those checks over so the right offers are shown or hidden as they were before. (#338)

## Reports

- **[Task]** **Confirm report numbers match the old system** — An investigation into why some Dashboard report figures differed from the legacy app, to pin down the cause and either fix it or confirm the numbers are correct. (#271)
- **[Feature]** **Show offer impressions in historical placement reports** — Historical placement reports currently show zero offer impressions. This fills in that figure so past reports display real numbers. (#339)

## Behind the Scenes

- **[Task]** **A read-only test environment with real-world data** — Setting up a safe, view-only copy of the system loaded with production-like data for testing and verification. (#270)
- **[Feature]** **Turn Slack discussions into tracked tasks automatically** — A helper that reads designated Slack conversations and files the action items as tracked work items, cutting out manual copy-and-paste. (#272)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — The legacy after-success handling (delivery and redirect steps that run once a visitor converts) is being brought over to New Adsmith Frontend so affected clients keep working as before. (#327)

## Flows

- **[Task]** **Fix the look of the Flow form** — Some parts of the Flow form appear unstyled or awkwardly laid out compared to other screens. This cleans up the styling so text boxes, color pickers, and paired fields look right. (#152)

## Modals

- **[Feature]** **Make the Modal design settings actually work** — The Modal design tab's header and progress-bar fields are saved but never shown to visitors. This either connects them so they display, or removes them if the modal is meant to have no header. (#294)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — Critical, high priority. The Campaigns area from the old admin—where you create and manage campaigns and offer groups—doesn't exist yet in New Adsmith Frontend. This adds it back with the same capabilities. (#200)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 20c05265760e30b087db164aa9ffb7701fea9cb19d23bb2497ef9c503a36041b -->
