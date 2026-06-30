# Open Issues — Plain-Language Overview

_Last updated 2026-06-30 19:34:04 UTC · 13 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker on the Dashboard** — Choosing "Custom" in the date filter will open start and end date pickers so you can view dashboard data for any date range you like, with the chosen range shown on the filter button. (#58)
- **[Task]** **Bring back the full Dashboard with richer stats** — The Dashboard will show much more than just system counts: campaign performance (impressions, clicks, leads, revenue), top offers, a placements watch list, and alerts for offers converting poorly. An activity log of system and offer changes is also planned so admins can see what changed and when. This is high priority. (#240)
- **[Feature]** **Change report dates without editing the web address** — You'll get proper date controls right in the Dashboard toolbar, so you can pull daily or custom-range reports by clicking instead of hand-editing the address bar (links will still stay shareable). (#268)

## Reports & Data Accuracy

- **[Task]** **A safe testing environment with real May & June data** — A separate staging area will be set up with recent data so reports can be checked and validated without ever touching live information. (#270)
- **[Task]** **Confirm new report numbers match the old system** — We're comparing report figures between the legacy system and New Adsmith Frontend to find and explain any differences, so you can trust the numbers you see. (#271)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record to edit, others will see it's locked, and if something changed while you had it open you'll be warned to reload instead of accidentally saving over someone else's work. This protects your changes across every editable screen. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper error message instead of unexpectedly sending you back to the Dashboard. This fix is nearly done. (#239)

## Users

- **[Task]** **Closing the gaps between the old and new Users area** — A review of the Users screens identified missing pieces from the legacy version (like bulk role changes, select-all, last-login and two-factor details, and password setup on new users) so the new Users area can match what you had before. (#80)

## Campaigns

- **[Feature]** **Add the Campaigns area to New Adsmith Frontend** — A Campaigns module is being built so you can create, edit, and manage campaigns and offer groups—including titles, questions, CTAs, offer handling and ordering—just like in the legacy admin. This is a critical, high-priority gap. (#200)

## Flows

- **[Task]** **Fix the look of the Flow form** — Remaining styling issues on the Flow form will be cleaned up so text boxes, color pickers, checkboxes, and paired fields display correctly and consistently with other forms. Part of this is already done. (#152)

## Offers

- **[Task]** **Quick action links under each offer** — Each offer will gain handy links (Edit, Quick Edit, Trash, View, Preview, Trends, Details), with Trends opening an Offer Activity page showing lead and revenue trends, date filtering, and a daily performance breakdown. Nearly complete. (#252)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on Placements** — Follow-up improvements to the offer list: defaulting new placements to "Manual Order" so your chosen order actually takes effect, plus a way to filter the available offers by category/vertical (not just text search). (#275)

## Behind the Scenes

- **[Feature]** **Automatic issue logging from Slack** — An internal helper that reads team conversations and turns action items into tracked tasks automatically, reducing manual copy-and-paste. This is a workflow tool with no direct effect on the product screens. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f4e8ac0b707d60441fe831fa987ec9ec71fe79497c302a996ba8e6e00eecfa1a -->
