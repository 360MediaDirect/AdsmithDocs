# Open Issues — Plain-Language Overview

_Last updated 2026-08-07 06:22:54 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Hand-picked offers now carry over from the old system** — On placements set to show a manually chosen list of offers, the new app was showing the wrong or no offers because the selected list wasn't being brought across. This fix makes the new app display the same manually selected offers, in the same order, as the old system. (#370)
- **[Bug]** **Restore the Display / AR choice on offers** — On the Offer Details Delivery tab, the controls for setting a survey to Display or AR went missing, so you couldn't assign a delivery mode. This restores those selectable controls so you can configure survey delivery again without going back to the old app. (#371)
- **[Bug]** **Saved offer options now actually take effect** — Several options you can set on an offer weren't making it through to the live experience visitors see. This fix ensures each saved option either takes effect or is cleaned up, so what you configure is what shows. (#295)
- **[Bug]** **Offer edits will show up in History** — Right now, editing an offer doesn't always add an entry to the offer's History section. This fix makes sure your changes are recorded so there's a reliable record of who changed what and when. (#380)
- **[Feature]** **Preview offers with your unsaved changes** — The Preview button will show the offer (and placement) exactly as you've edited it, even before you save, so you no longer have to save first just to see how a change looks. (#292)
- **[Feature]** **Automatic performance estimate for new offers** — A new tool will estimate how a new offer is likely to perform based on your existing offers and their history, replacing the old manual gut-check review with a data-driven projection. (#322)

## Admin / Across the App

- **[Feature]** **Remove settings that don't do anything** — Some admin controls (such as Advertiser Web Presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping options) are currently saved but have no effect. They'll be removed or hidden so the settings you see are ones that actually work. (#296)
- **[Task]** **Review of the Users area against the old system** — A thorough comparison of user management in New Adsmith Frontend versus the legacy system to catch any missing capabilities, so the Users area can be brought up to full coverage over time. (#80)

## Data Clients & Pre-Pings

- **[Feature]** **Carry over legacy post-conversion delivery steps** — Certain delivery and redirect steps that ran after a successful conversion in the old system are being rebuilt in New Adsmith Frontend, so those clients keep working the same way after launch. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Many data clients relied on custom serve-time validation checks that don't yet run in the new platform. This high-priority work rebuilds those checks so leads are validated consistently, matching the old system's pass/reject behavior. (#338)

## Advertisers

- **[Feature]** **Notes on Placement, Advertiser, and Offer dashboards** — You'll be able to add short, categorized notes (with a topic and priority) directly on a placement, advertiser, or offer, and see a recent-notes roll-up on the main Dashboard — restoring a handy capability from the old system. (#382)
- **[Feature]** **Website and social links on the Advertiser detail page** — The Web Presence details you enter (website, social profiles, and a Search-on-Google shortcut) will appear as quick icon links in the Advertiser detail header, so you can jump straight to an advertiser's online presence. (#383)

## Surveys

- **[Feature]** **Design choices now show up in the survey** — Customizations made on the Design tab will be reflected in the survey visitors actually see, plus a full check across every entity to confirm no design option is left disconnected. (#288)
- **[Feature]** **Finish connecting placement design settings** — A few placement Design-tab settings (like iFrame height and display format) are saved but don't yet affect the survey. This wires them through so they take effect, and cleans up any that aren't needed. (#293)

## Behind the Scenes

- **[Feature]** **Automatic follow-up from team conversations** — An internal helper that turns action items from team chats into tracked to-do items automatically, reducing manual copy-and-paste. This is an internal workflow tool with no direct change to the product screens. (#272)
- **[Task]** **Improvements to automated testing** — Behind-the-scenes work to strengthen the automated checks that verify the admin screens, making future releases more reliable. (#379)

## Modals

- **[Feature]** **Make the Modal Design tab do something (or remove it)** — The Modal Design tab's settings (header title, colors, progress bar, etc.) are currently saved but never shown to visitors. This work will either make those settings appear in the visitor modal or remove the tab so it isn't misleading. (#294)

## Publishers & Properties

- **[Bug]** **Pausing a publisher or property will reliably take effect** — Because of a mismatch in how the pause status was checked, pausing didn't always stop serving. This fix makes the pause setting enforce consistently so a paused publisher or property is truly paused. (#299)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or awkwardly laid out (plain text boxes, misaligned paired fields). This cleanup brings the Flow form in line with the polished look of the Placement and Modal forms. (#152)

## Reports & Dashboard

- **[Task]** **Investigate mismatched dashboard report numbers** — Reviewers noticed dashboard report figures didn't match the old system. This investigation compares the two over a fixed period to find where the difference comes from and confirm the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
