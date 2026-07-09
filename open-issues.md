# Open Issues — Plain-Language Overview

_Last updated 2026-07-09 16:50:14 UTC · 24 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Feature]** **Protection against overwriting each other's work** — When two people open the same record, New Adsmith Frontend will show that someone else is already editing it and warn you if the record changed since you opened it, so edits can't silently wipe out each other. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will be able to see who changed what and when across the app — including automated changes — making it easy to answer "who edited this record?" (#276)
- **[Feature]** **Hiding settings that don't actually do anything** — Several controls that look active but have no effect (like the Advertiser Web Presence fields, certain user permission toggles, and some Data Client and Pre-Ping options) will be removed or hidden, so screens only show controls that truly work. (#296)
- **[Task]** **Consistent look for alert and status banners** — Warning, info, success, and error banners will look the same on every screen instead of varying slightly from page to page. (#341)
- **[Bug]** **Clear error when testing an invalid link** — Testing a link that isn't valid will show a proper error message instead of unexpectedly sending you to the Dashboard. (#239)
- **[Task]** **Review of user-management features from the old system** — A documentation effort comparing the old and new user screens to make sure important capabilities carry over to New Adsmith Frontend. (#80)
- **[Task]** **Decide whether to keep the old file-share page** — Checking whether the legacy file-sharing page is still needed, then either giving it a home in the new admin or formally retiring it. (#328)

## Offers
- **[Bug]** **Saved offer settings that weren't reaching the live experience** — A number of offer options (including modal fields, Display URL, and several data-client flags) were being dropped and never applied to what visitors saw. These will either be properly applied or clearly removed from the form. (#295)
- **[Feature]** **Preview offers and placements with your unsaved changes** — The Preview button will show the edits you've just made rather than only the last saved version, so you can check changes before committing them. (#292)
- **[Feature]** **Automatic performance estimate for new offers** — New Adsmith Frontend will be able to project how a new offer is likely to perform based on your historical offer data, replacing today's manual gut-check review. (#322)
- **[Task]** **Auto-register offers should respect visitor targeting** — Auto-register offers currently fire for everyone, ignoring age, gender, state, zip, and device targeting. This will be corrected (or confirmed as intended) so they only fire for the right visitors. (#333)

## Surveys & Modals
- **[Feature]** **Design-tab settings that fully take effect** — An end-to-end check to ensure every survey design customization you set is actually reflected in what visitors see, with no options that quietly do nothing. (#288)
- **[Feature]** **Finishing placement survey design options** — Placement Design-tab settings (like survey height and display format) will be fully connected so they show up in the live survey, or removed if they aren't used. (#293)
- **[Feature]** **Making the Modal Design tab work — or removing it** — The Modal Design tab's header and progress-bar settings currently have no effect; they'll either be applied to the visitor modal or taken out of the form. (#294)

## Pre-Pings & Data Clients
- **[Feature]** **Restoring after-conversion delivery steps for clients** — Post-conversion delivery and redirect behavior from the old system will be brought over so those clients continue to work in New Adsmith Frontend. (#327)
- **[Feature]** **Live pre-ping checks at display time** — Display-triggered pre-pings will actually contact the advertiser and hide the offer if it's rejected, matching the old system's behavior. (#337)
- **[Feature]** **Bringing over custom per-client pre-ping checks** — Hundreds of data clients rely on custom pre-ping validation from the old system that isn't running yet; this work restores those checks so offers pass or fail correctly at serve time. (#338)

## Behind the Scenes
- **[Task]** **Read-only test environment for validation** — Setting up a staging copy of New Adsmith Frontend against production-like data for safe checking, with no risk of changing real data. (#270)
- **[Feature]** **Turning conversations into tracked work items automatically** — A helper that reads team conversations and files or updates issues automatically, reducing manual note-taking. (#272)
- **[Task]** **Hardening the change-tracking safeguard** — Behind-the-scenes improvements to make the "someone else changed this" protection more reliable under rare simultaneous saves. (#342)

## Dashboard & Reports
- **[Task]** **Confirming report numbers match the old system** — An investigation into why some Dashboard report totals didn't line up with the legacy system, so you can trust the figures during validation. (#271)
- **[Feature]** **Fixing zeroed-out offer impressions in placement reports** — Historical placement reports will show real offer-impression numbers instead of always displaying zero. (#339)

## Flows
- **[Task]** **Fixing the styling on the Flow form** — Parts of the Flow form (text boxes, color pickers, checkboxes, and side-by-side fields) look unstyled or misaligned; this cleans up the appearance to match other forms. (#152)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 22c25e65cd09866ecd1852615a4445296f9dfa6bf905dc468d9a85af11345067 -->
