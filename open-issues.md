# Open Issues — Plain-Language Overview

_Last updated 2026-06-25 22:30:15 UTC · 15 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Feature]** **Restore the full Dashboard with all reporting sections** — Right now only the system overview loads. This brings back campaign stats, top offers, and watch lists, and makes sure they update when you change the date range. (#240)
- **[Feature]** **New monitoring views and an activity log** — Adds an "Other Dashboard" area with views for long-running ("legs") offers and CLP offer performance that flags anything converting under 30%, plus a searchable record of key actions like pausing an offer or changing a daily cap, so you can see who changed what and when. (#256)
- **[Feature]** **Dark and Light mode for the Admin** — You'll be able to switch the whole interface between dark and light themes from your user menu, and your choice will stick the next time you sign in. Helpful for bright rooms or reducing eye strain. (#59)
- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" will open a start- and end-date picker so you can look at exactly the period you want instead of only the preset ranges. (#58)
- **[Feature]** **Sub-ID Stats move to the Dashboard** — Sub-ID statistics will live in the Dashboard reporting area instead of being tucked inside the placement form, making them easier to find. (#236)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan view will show data in 15-minute increments, giving you a near-real-time way to spot errors or partner-server issues quickly. (#243)
- **[Task]** **Consistent Dashboard colors** — A defined color palette will be applied across the Dashboard for cleaner, easier-to-read visuals. (#263)

## General / Across the App

- **[Feature]** **Campaigns management is coming to the new platform** — The Campaigns area from the old admin will be rebuilt here, letting you view, create, and edit campaigns and manage offer groups, CTA text, offer order and quantity, and assigned offers — a core workflow that's currently missing. High priority. (#200)
- **[Feature]** **Protection against two people overwriting the same record** — When you open a record to edit, others will see it's locked and by whom, and if someone changed it while you had it open you'll be prompted to reload instead of accidentally erasing their work. Applies across offers, flows, placements, advertisers, and other entity screens. (#267)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link will now show a proper failure message in the Link Testing screen instead of quietly sending you back to the dashboard. (#239)

## Flows

- **[Task]** **Fix the Flow form's appearance** — Cleans up the Flow form so text boxes, color pickers, checkboxes, and paired fields display correctly and sit side-by-side, matching the polished look of the Placement and Modal forms. (#152)
- **[Feature]** **Make the "Step order" setting understandable** — Adds clear labels and help text (or a reworked control) so it's obvious what the step-order setting does and what its values mean. (#226)

## Placements

- **[Feature]** **Easier offer ordering on placements** — Selected offers will default to manual order, support drag-and-drop reordering, include an "X" to remove an offer (so clicking is reserved for dragging), and let you filter the offer list by taxonomy. (#235)

## Offers

- **[Bug]** **Enforce required fields before a pre-ping is sent** — When a pre-ping runs before a data push, leads missing required fields will be stopped right away instead of being passed along to the advertiser, preventing incomplete leads from slipping through. Pending confirmation that this is the desired behavior. (#218)

## Behind the Scenes

- **[Task]** **Stronger brand guidelines for AI-generated content** — The team will create one comprehensive brand-guidelines document to use as the main reference for AI output, improving the quality and consistency of generated content. (#264)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 2a56fd67f9291cb8ae4aad8782237f68a408d23759c09f54732863f026266184 -->
