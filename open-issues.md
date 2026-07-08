# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 23:25:19 UTC · 24 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When you open a record that someone else is already editing, you'll see a clear notice and be kept from accidentally saving over their changes, avoiding lost work. (#267)
- **[Feature]** **Clean up controls that don't do anything** — Several settings that look active but currently have no effect (like the Advertiser Web Presence fields, certain user permission toggles, and some Data Client and Pre-Ping options) will be hidden or removed so the screens only show controls that actually work. (#296)
- **[Task]** **Decide the future of the legacy file-share page** — The old file-share page has no equivalent yet; this is a decision on whether to rebuild it or retire it, so nothing is left in limbo. (#328)
- **[Task]** **Consistent colors for alerts and banners** — Warning, info, success, and error messages will look identical from page to page instead of drifting in shade. This is a behind-the-scenes tidy-up you'll notice as a more polished, consistent look. (#341)

## Offers

- **[Bug]** **Saved offer settings not reaching the live page** — Some offer options you fill in and save (including the Modal-tab fields, Force More Info Visible, and Display URL) currently never show up where they should. This fix makes sure saved settings actually take effect, or removes any option that isn't meant to be used. (#295)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, new offers could be scored against your historical offer data to estimate how they're likely to perform, giving you a quick data-driven read at intake. This is exploratory. (#322)
- **[Task]** **Auto-register offers should respect audience targeting** — Auto-register offers currently fire for everyone, ignoring age, gender, state, ZIP, and device targeting. This work confirms the correct behavior and ensures these offers only fire for the intended visitors. (#333)

## Surveys

- **[Feature]** **Make sure Design tab settings show up in the live survey** — Every customization you set on the Design tab will be checked end-to-end so it actually appears on the survey visitors see, with no settings that quietly do nothing. (#288)
- **[Bug]** **Voucher code and info links missing on live survey** — A configured voucher code line and the privacy/terms/details links aren't appearing on the live survey page even though they're saved. This fix restores them, which matters for passing leads and for compliance. (#291)
- **[Feature]** **Finish connecting Placement Design settings to the survey** — Several Placement Design settings (like iFrame height and display format) are saved but don't yet affect the survey. This wires them through so your choices take effect, or removes any that aren't needed. (#293)

## Pre-Pings

- **[Feature]** **Run display pre-ping checks at the right moment** — Offers using the "display" pre-ping trigger will properly perform their real-time verification and be hidden when rejected, matching how the legacy system behaved. (#337)
- **[Feature]** **Restore custom per-client pre-ping checks** — Hundreds of data clients rely on custom pre-ping validation from the old system that isn't running yet on the new platform. This brings that verification back so those clients' offers are checked correctly before serving. (#338)

## Placements

- **[Feature]** **Preview your unsaved changes** — On placement and offer edit screens, the Preview button will show your current in-progress edits instead of only the last saved version, so you can check changes before committing them. (#292)
- **[Feature]** **Correct offer impression counts in placement reports** — Historical placement reports currently show zero offer impressions; this fills in that number so your reports reflect real performance. (#339)

## Dashboard

- **[Bug]** **Show a clear error for invalid links instead of the dashboard** — When you test an invalid link, you'll get a proper failure message instead of being unexpectedly sent to the dashboard. (#239)
- **[Task]** **Confirm dashboard report numbers match the legacy system** — An investigation into why some dashboard figures didn't line up with the old system, so you can trust the numbers you see. (#271)

## Behind the Scenes

- **[Task]** **Prepare a safe, read-only test environment** — Setting up a staging version of New Adsmith Frontend that mirrors real data but can't change anything, used for verification. No user-facing change. (#270)
- **[Feature]** **Automatically turn team conversations into tracked tasks** — A helper that reads designated chat channels and files action items as tracked issues, reducing manual note-taking. This is an internal workflow tool. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — The Modal Design tab's header and progress-bar settings don't currently affect the modal visitors see. This either connects them so your choices display, or removes the tab if it's not needed. (#294)

## Data Clients

- **[Feature]** **Bring back post-conversion delivery behavior** — Certain "after success" delivery and redirect behaviors from the old system weren't carried over. This restores them so conversions complete the same way they did before. (#327)

## Flows

- **[Task]** **Fix unstyled areas of the Flow form** — Parts of the Flow form currently look broken or unstyled (plain text boxes, unstyled color pickers, misaligned fields). This tidies up the layout so the form looks consistent with the rest of the app. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns area to the new platform** — The Campaigns module from the old admin isn't available yet. This adds it back so you can create, edit, and manage campaigns and their offer groups. High priority. (#200)

## Users

- **[Task]** **Compare the new Users area to the old one** — A review of what the legacy Users screen offered versus the new one, so any missing capabilities (like bulk role changes and last-login info) can be prioritized and added. (#80)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 8e666a901068071cf7f0d70228648729a3442a16df96262801f3773c853e1044 -->
