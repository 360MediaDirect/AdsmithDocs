# Open Issues — Plain-Language Overview

_Last updated 2026-07-09 19:32:40 UTC · 26 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview your unsaved changes on Offers and Placements** — When editing an offer or placement, the Preview will show exactly what you're working on right now, including edits you haven't saved yet, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Some saved offer settings weren't reaching the live page** — A number of offer options (including several Modal-tab settings and "Force More Info Visible") were being saved but never actually applied where visitors see them. This fix ensures the choices you make in the Offer form take effect, or removes options that do nothing. (#295)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your own historical offer data, giving you a data-driven gut-check at intake instead of relying on a manual review. (#322)
- **[Bug]** **Auto-register offers now respect visitor targeting** — Auto-register offers were firing for everyone, ignoring age, gender, state, ZIP, and device targeting. This corrects them so they only fire for the visitors they're meant for. (#333)
- **[Bug]** **bPerx voucher code missing from the offer preview** — The "Your Voucher Code" line isn't showing up in the offer preview on the test environment. This investigates and fixes the lookup so the voucher code appears in both preview and the live survey. (#344)

## General / Across the App

- **[Feature]** **Editing protection so two people don't overwrite each other** — When someone is editing a record, others will see it's locked and by whom, and a safety check on save prevents accidentally wiping out a colleague's changes. High priority. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will get an "Audit Log" that records who changed what and when, across offers, placements, advertisers, and more, making it easy to answer "who changed this and why." (#276)
- **[Feature]** **Cleaning up controls that don't do anything** — Several admin settings (like the Advertiser Web Presence fields and some user-permission toggles) look active but aren't actually connected to anything. They'll be removed or hidden so the screens only show controls that work. (#296)
- **[Task]** **Decide the fate of the old file-share page** — The legacy file-share page has no equivalent in New Adsmith Frontend; this confirms whether anyone still needs it or whether it can be retired. Likely low priority. (#328)
- **[Bug]** **Invalid links should show an error, not send you to the Dashboard** — When testing a bad link, you'll now get a clear failure message instead of being unexpectedly dropped onto the Dashboard. (#239)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up an environment that mirrors real data for testing and verification, locked to read-only so nothing can be accidentally changed. (#270)
- **[Feature]** **A Slack helper that files issues automatically** — An internal tool that turns action items from Slack conversations into tracked tasks, reducing manual copy-and-paste work for the team. (#272)
- **[Task]** **Consistent colors for alerts and banners** — Standardizing the tint colors used for warning, info, error, and success banners so the same type of message looks identical on every screen. (#341)
- **[Task]** **Stronger safeguards behind the editing-protection feature** — Behind-the-scenes hardening so the change-tracking used to prevent overwrites stays reliable even in rare, edge-case timing situations. (#342)

## Surveys

- **[Feature]** **Every design option should actually change the survey** — A full review to make sure each customization option in the design tabs is truly reflected on the live survey, with any dead options fixed or removed. (#288)
- **[Bug]** **Voucher code and info links missing from the live survey** — On the new survey page, the configured voucher code line and the privacy/terms/details links aren't showing up even though they're set correctly in the admin. This restores them to match the previous system. High priority, and important for compliance. (#291)
- **[Feature]** **Finish connecting Placement design settings to the survey** — Several Placement design-tab settings (like survey height and display format) are saved but not yet applied to what visitors see. This wires them through or removes the ones that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore post-conversion delivery behaviors** — The legacy "after-success" scripts that run once a lead converts weren't carried over. This brings that behavior back as a configurable option for the affected clients. Nearly complete. (#327)
- **[Feature]** **Make display-trigger pre-ping checks actually run** — Certain pre-ping validations were only checking that a field existed rather than performing the real live check. This makes them work as before, hiding offers that get rejected. High priority. (#337)
- **[Feature]** **Bring back per-client pre-ping validation** — Custom pre-ping checks tied to hundreds of data clients weren't carried into the new platform, meaning some serve-time validations silently weren't running. This restores that coverage. High priority. (#338)

## Reports & Dashboard

- **[Task]** **Confirm report numbers match the previous system** — Investigating why some Dashboard report figures differed from the legacy app, so you can trust that the numbers line up. (#271)
- **[Feature]** **Fix zeroed-out offer impressions in placement reports** — Historical placement reports have been showing offer impressions as zero. This starts recording that figure so the reports show real numbers. (#339)

## Campaigns

- **[Feature]** **Bring the Campaigns area into New Adsmith Frontend** — The Campaigns module from the old system isn't in the new platform yet. This adds the ability to view, create, edit, and configure campaigns and their offer groups. Critical, high priority. (#200)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — All six settings on the Modal Design tab currently have no effect on the visitor-facing modal. This either wires them up so they apply or removes the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or misaligned compared to other forms. This cleans up the layout so text boxes, color pickers, and paired fields display properly. Partly done. (#152)

## Admin / Users

- **[Task]** **Compare the Users area against the old system** — A documentation review listing which Users features exist in New Adsmith Frontend versus the legacy app, so any missing pieces (like bulk actions or last-login info) can be prioritized. Mostly complete. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 72540624e535d3919fd77d9fe303c83f136dbb2b7ca301364f9323720c202039 -->
