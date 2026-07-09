# Open Issues — Plain-Language Overview

_Last updated 2026-07-09 00:29:33 UTC · 24 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record to edit it, others will see a clear "locked by…" note and won't be able to accidentally save over their changes. If a record was changed while you had it open, you'll be prompted to reload instead of losing work. (#267)
- **[Feature]** **A searchable history of every change** — Administrators will get an "Audit Log" that records who changed what and when across offers, placements, advertisers, and more — including automated changes — so you can finally answer "who edited this and when?" (#276)
- **[Feature]** **Clean up controls that don't actually do anything** — Several settings that currently appear editable but have no effect (some Advertiser web-presence fields, certain user-permission toggles, and a few Data Client and Pre-Ping options) will be removed or hidden so the screens only show controls that really work. (#296)
- **[Bug]** **Invalid links in Link Testing now show an error** — Testing a bad link will return a clear failure message instead of quietly sending you back to the Dashboard. This fix is nearly complete. (#239)
- **[Task]** **Decide the future of the old file-share page** — We're confirming whether the legacy file-sharing page is still needed and, if so, where it belongs in the new admin, or documenting that it's being retired. (#328)

## Offers

- **[Bug]** **Saved offer settings that never reach the live page** — A number of offer options are saved but dropped before they appear on the live experience (including some modal fields, "Force More Info Visible," Display URL, and several back-end data flags). We'll make sure each saved option is either shown where expected or removed if it's not needed. (#295)
- **[Feature]** **Preview shows your unsaved changes** — On Offer and Placement edit screens, Preview will reflect the edits you've just made instead of only the last saved version, so you can check changes without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — We're exploring an assistant that estimates how a new offer is likely to perform based on your historical offer data, replacing today's manual gut-check review. (#322)
- **[Task]** **Auto-register offers should respect visitor targeting** — Certain automatic offers currently fire for everyone, even when age, gender, state, zip, or device targeting says they shouldn't. We'll confirm the intended behavior and make targeting apply consistently. (#333)

## Surveys

- **[Feature]** **Make every design option actually take effect** — We're reviewing all the customization options across screens to confirm each one truly changes what visitors see on the survey, fixing or removing any that don't. (#288)
- **[Bug]** **Voucher code and info links missing on live surveys** — For affected data clients, the voucher code line and the privacy/terms/details links are configured but not showing on the live page like they did before. This fix restores them (important for passing leads and compliance). (#291)
- **[Feature]** **Finish connecting Placement design settings** — A handful of Placement "Design" tab settings (like survey height and display format) are saved but don't yet change the survey. We'll wire them through or remove the ones that aren't used. (#293)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — We're setting up a staging version of New Adsmith Frontend using production-like data for testing and verification, locked to read-only so nothing can be changed by accident. (#270)
- **[Feature]** **Turn conversations into tracked to-dos automatically** — An internal helper will read designated chat channels and open or update work items automatically, cutting out manual copy-and-paste of action items. (#272)
- **[Task]** **Consistent colors for alerts and banners** — Warning, info, success, and error banners will use one shared set of color definitions so the same type of message looks identical on every screen. (#341)

## Reports

- **[Task]** **Confirm the new reports match the old system** — We're comparing report numbers between the legacy system and New Adsmith Frontend over a fixed date range to find and explain any differences, so you can trust the figures. (#271)
- **[Feature]** **Fix zero offer-impression counts in placement reports** — Historical placement reports currently show offer impressions as zero. We'll start recording that figure so the reports show real numbers. (#339)

## Pre-Pings

- **[Feature]** **Check offers with the advertiser before showing them** — For offers set to check at display time, the system will make the real-time verification call and hide the offer if it's rejected, matching how the legacy system worked. (#337)
- **[Feature]** **Bring back per-client pre-ping checks** — Hundreds of data clients relied on custom pre-serve validation in the old system that isn't running yet. We'll map and restore these checks so those clients validate as expected. (#338)

## Data Clients

- **[Feature]** **Restore after-conversion delivery steps** — The old system's post-conversion delivery and redirect behavior for certain clients (bperx, rwdb) will be brought over as a configurable option, so nothing is lost after a lead converts. This work is nearly done. (#327)

## Campaigns

- **[Feature]** **Add the missing Campaigns area** — The Campaigns management area from the old system isn't in the new platform yet. This adds the ability to view, create, edit, and configure campaigns and offer groups, restoring a core workflow. (#200)

## Modals

- **[Feature]** **Make the Modal design settings work (or remove them)** — The entire Modal "Design" tab currently has no effect on what visitors see. We'll either connect those header and progress-bar settings to the live modal or remove the tab. (#294)

## Flows

- **[Task]** **Fix the styling of the Flow form** — Parts of the Flow form look unstyled or misaligned (plain text boxes, unstyled color pickers, fields stacking instead of sitting side by side). We'll tidy these up carefully so the form matches the rest of the app. Partly done. (#152)

## Users

- **[Task]** **Compare the new Users area to the old one** — We're documenting what the old Users management had versus the new one to spot missing features (like bulk actions and login/2FA details) and prioritize what to add. This review is mostly complete. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: e97c0c87fd1c264309b547c86ecde9d1b7abd3cebd9c6dc642ac728d6283da48 -->
