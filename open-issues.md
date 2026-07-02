# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 21:25:57 UTC · 29 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Compliance & Lead Delivery
- **[Feature]** **Ongoing TrustedForm compliance and lead-handling improvements** — This is the umbrella effort to properly claim and store consent certificates for leads and to make lead delivery more reliable and dependable. (#309)
- **[Bug]** **Prevent a lead from being sent to an advertiser twice** — If something hiccups right after a lead is delivered, the system could re-send the same lead. This fix makes sure each lead reaches the advertiser only once, protecting against double-billing and advertiser-trust issues. (#303)
- **[Bug]** **Stop retrying leads that can never succeed** — Leads that are permanently rejected (duplicates, do-not-call, failed checks) will no longer be retried over and over, keeping error tracking clean and trustworthy. (#304)
- **[Feature]** **TrustedForm certificate switch on the Data Client form** — You'll be able to turn TrustedForm certificate claiming on or off for each data client directly in the admin, instead of it being something only a developer can set. (#305)
- **[Task]** **Review how long consent records are kept** — A behind-the-scenes check to confirm the retention period for TrustedForm consent evidence matches current data and privacy policy. (#306)

## Dashboard
- **[Task]** **Custom date range picker for the date filter** — Choosing "Custom" will open a start/end date picker so you can view dashboard data for any range you like, not just the preset options. (#58)
- **[Feature]** **Pick report dates right in the dashboard** — You'll be able to change the reporting day or range using controls in the dashboard itself, instead of hand-editing the web address. Links will still stay shareable. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example, as a spreadsheet). (#286)
- **[Task]** **Confirm dashboard numbers match the legacy system** — An investigation into why some report totals differ from the old app, so you can trust that the new dashboard reports are accurate. (#271)

## Surveys
- **[Bug]** **Make the survey Design settings actually take effect** — Many styling and behavior options (colors, continue button, question text, header, legal text) are saved but don't currently change what visitors see. This wires them up so your design choices actually appear on the live survey. (#290)
- **[Feature]** **Finish connecting the remaining Design-tab settings** — Wraps up the last few survey design options so each one either works on the live survey or is removed if it isn't needed. (#293)
- **[Feature]** **Make sure every design option is fully connected** — A sweep to confirm that customization options across all screens genuinely flow through from the form to what visitors see, with no "dead" settings that quietly do nothing. (#288)
- **[Bug]** **Voucher code and info links missing on the live survey** — For affected data clients, the voucher code line and the privacy/terms/details links are configured correctly but don't show up on the survey page like they did in the old app. This restores them. (#291)

## General / Across the App
- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone is editing a record, others will see it's locked and by whom, and the system will warn you if a record changed while you had it open, so no one's changes get silently lost. (#267)
- **[Feature]** **A searchable history of who changed what** — A new admin Audit Log will record every change to records (and automated changes too), with who made it and when, plus a per-record history, making it easy to answer "who changed this?" (#276)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings across the app are shown but have no effect. These will be hidden or removed so the admin only shows controls that actually work. (#296)
- **[Bug]** **Show a clear error when testing an invalid link** — Testing a bad link currently dumps you on the dashboard with no explanation. Instead you'll get a clear failure message. (#239)

## Offers
- **[Bug]** **Success pixels now fire as configured** — Conversion/postback pixels set up on an offer currently never fire, so conversions go untracked. This fixes them so configured pixels fire reliably. (#297)
- **[Feature]** **Preview shows your unsaved changes** — The Preview button on offer and placement edit pages will reflect the edits you're currently making, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Make sure saved offer options reach the live page** — Some offer settings are saved but never make it to what visitors see. Each will be connected and shown, or removed if it isn't needed. (#295)

## Modals
- **[Feature]** **Make the Modal Design tab work (or remove it)** — Every field on the Modal Design tab is saved but has no effect on the visitor's modal today. These will either be wired up to display properly or removed to avoid confusion. (#294)
- **[Bug]** **"In Order" offer sorting can't be saved** — The modal offers an "In Order" sorting choice that fails to save. It will either be made fully functional or removed from the form. (#301)

## Placements & Properties
- **[Feature]** **Smarter offer ordering and filtering on placements** — Deciding whether new placements should default to your manual offer order (so reordering actually sticks), plus a filter to narrow the available offers list by category. (#275)
- **[Bug]** **Domain restrictions on properties will take effect** — Domain settings entered for a property currently do nothing at run time. This fixes them so your allowed-domain rules are actually applied. (#300)

## Behind the Scenes
- **[Task]** **A safe test environment with May and June data** — Setting up a separate practice environment loaded with real-looking data so testing and report checks can happen without touching live information. (#270)
- **[Feature]** **A Slack helper that turns conversations into tracked tasks** — A bot that reads designated Slack channels and automatically files action items as tracked issues, reducing manual copy-paste. (#272)

## Flows
- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned compared to other forms. This cleans up the layout and styling so it matches the rest of the app. (#152)

## Campaigns
- **[Feature]** **Bring Campaigns into New Adsmith Frontend** — The Campaigns module from the old admin isn't in the new platform yet. This adds it so you can view, create, edit, and configure campaigns and offer groups as before. (#200)

## Users
- **[Task]** **Review of the Users area vs. the old system** — A documentation exercise comparing the old and new Users screens to catch any missing capabilities (like bulk actions or last-login info) and plan what to add. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 688fb8a78c0b972004980386a6635670609cd11ed85c7a46286f8edcaf995650 -->
