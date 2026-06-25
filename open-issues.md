# Open Issues — Plain-Language Overview

_Last updated 2026-06-25 16:47:58 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Selecting "Custom" in the date filter will open a start- and end-date picker so you can view dashboard data for any specific period instead of only preset ranges like Today or This Month. (#58)
- **[Feature]** **Make the Edit, Preview, and Pull Leads buttons work on detail pages** — On Placement, Modal, Offer, and Advertiser detail pages, these buttons currently do nothing when clicked. They'll be wired up so they actually take you to the right place or pull the lead data. (#154)
- **[Feature]** **Move Sub-ID Stats into the Dashboard** — Sub-ID Stats will move out of the placement form and into the Dashboard's reporting area, where this kind of performance data belongs. (#236)
- **[Task]** **Restore missing Dashboard sections** — Right now only the system overview loads. Campaign stats, top offers, and watch lists will be brought back, and the date-range selector will properly update them. This is high priority. (#240)
- **[Feature]** **15-minute detail on offer timespan stats** — The offer detail timespan chart will show data in 15-minute increments again, giving you the fine-grained view needed to spot offer or partner-server issues quickly. (#243)
- **[Feature]** **New "Other Dashboard" monitoring views and an activity log** — Adds views for long-running ("offers with legs") and CLP offer performance, with low-converting CLP offers flagged, plus a searchable log that records changes like pausing an offer or adjusting daily caps. (#256)
- **[Feature]** **Consistent Dashboard color scheme** — A defined color palette will be applied across the Dashboard for better, more consistent readability. (#263)

## General / Across the App

- **[Feature]** **Dark and Light mode toggle** — You'll be able to switch the entire Admin between dark and light themes from your user menu, with your choice remembered next time you sign in. (#59)
- **[Feature]** **Bring back the Campaigns module** — The Campaigns area from the legacy admin isn't in New Adsmith Frontend yet. It will be rebuilt so you can view, create, edit, and configure campaigns and their offer groups. This is a critical, high-priority addition. (#200)
- **[Feature]** **Link Testing remembers where you came from** — When you open Link Testing from a specific placement, that placement will already be selected for you instead of making you pick it each time. (#238)
- **[Bug]** **Clear error for invalid links in Link Testing** — Testing a bad link currently dumps you back on the dashboard. Instead, you'll see a clear failure message right in Link Testing. (#239)
- **[Feature]** **Stronger brand guidelines for AI-generated output** — A comprehensive brand-guidelines document will be established and used as the main reference for AI output, improving consistency and quality. (#264)
- **[Feature]** **Prevent two people from overwriting each other's edits** — When you open a record that someone else is already editing, you'll see a clear "locked by" notice, and you'll be warned if a record changed while you had it open — so no one's work gets silently lost. (#267)

## Offers

- **[Feature]** **Set all offer fields at creation time** — Piggyback offers, HD pixel placement IDs, and ZIP code targeting can currently only be added after an offer exists. You'll be able to set them right when you first create the offer. This is high priority. (#142)
- **[Feature]** **Enforce required pre-ping fields before sending** — When a pre-ping runs before a data push, missing required fields will stop the lead immediately rather than relying on the advertiser's system to catch it, preventing incomplete leads from slipping through. (Pending a decision to confirm the change.) (#218)
- **[Feature]** **Easier advertiser and state selection on the offer form** — The Advertiser field will get a type-to-search box, and state targeting will accept a typed or pasted comma-separated list (e.g. CA, TX, FL) in addition to picking states. (#249)
- **[Feature]** **Add a whole offer group to Conflicting Offers at once** — On the Delivery & Settings tab, you'll be able to select an offer group and add all of its offers to the Conflicting Offers list in one step, saving a lot of repetitive work. (#250)

## Flows

- **[Task]** **Fix the Flow form's appearance** — The Flow form currently has unstyled text boxes, color pickers, and checkboxes, and some paired fields stack awkwardly instead of sitting side by side. This brings the form in line with the polished look of the Placement and Modal forms. (#152)
- **[Feature]** **"Add all fields" button on the Form tab** — Instead of adding form fields one at a time, you'll be able to add every available field at once with a single click. (#224)
- **[Feature]** **Make "Step order" understandable** — The step-order control on the Flow form is confusing. Clearer labels and help text will explain exactly what it controls and what the values mean. (#226)
- **[Feature]** **Improved TCPA consent checkbox** — On the published lander, the TCPA consent checkbox will be made larger, rounded, and properly aligned with its consent text. (#229)

## Placements

- **[Feature]** **Better control over selected offers** — The offer list will default to Manual Order, let you drag and drop to reorder your selected offers, add an X to remove an offer (so clicking is reserved for dragging), and let you filter the offer list by taxonomy. (#235)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 48398f3905362f8d5574f34143365776d51e1568ad4d21955aa674c3c27e4b37 -->
