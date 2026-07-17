# Open Issues — Plain-Language Overview

_Last updated 2026-07-17 05:02:10 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers to fire on success have silently not been working, meaning some completed leads weren't being counted. This high-priority fix ensures the pixels you configure actually fire when a visitor succeeds. (#297)
- **[Task]** **Auto-register offers ignore visitor targeting** — Certain "auto-register" offers have been firing for every visitor regardless of the age, gender, state, zip, or device targeting you set. This high-priority fix makes those offers respect your targeting rules so they only fire for the right audience. (#333)
- **[Bug]** **Some saved offer settings never reached live offers** — A number of offer options you can fill in (including several modal-tab fields and other settings) weren't actually being carried through to the live experience. This work makes sure every field either does something or is removed so nothing is misleading. (#295)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — Today the Preview button shows the last saved version, so you have to save before you can see your edits. Soon Preview will reflect your current in-progress changes without forcing a save. (#292)
- **[Feature]** **Predict how a new offer will perform** — Instead of relying on a manual gut-check, this explores an automated projection that estimates how a new offer is likely to perform based on your historical offer data. It would give a quick, data-grounded read at intake time. (#322)

## Surveys

- **[Feature]** **Make sure every Design tab option actually works** — A review across all entities to confirm each customization option on the Design tab is truly reflected in the live survey, with any settings that do nothing either fixed or removed. You'll be able to trust that what you set is what visitors see. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey** — Several Placement Design tab settings (like iFrame height and display format) were saved but not applied to the live survey widget. This finishes wiring them up so your choices take effect. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Restore "after success" delivery behavior** — Some post-conversion delivery and redirect steps from the previous system hadn't been carried over. This brings them back as a reusable, configurable option so affected clients keep working as before. (#327)
- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients relied on custom validation checks that ran before serving, and those weren't yet active on the new platform. This high-priority work restores that behavior so those clients' checks run again. (#338)

## Admin & Users

- **[Task]** **Compare old and new Users screens for missing features** — An ongoing review of the Users area against the previous system to spot anything missing (like bulk role changes, last-login info, and 2FA status) so the new Users experience reaches full parity. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several settings across Advertisers (Web Presence), user permissions, Data Clients, and Pre-Ping are saved but never actually used, which is confusing and misleading. These will be hidden or removed unless they're built out for real. (#296)

## Modals

- **[Feature]** **Make the Modal Design tab work or remove it** — Every field on the Modal Design tab is currently saved but has no effect on what visitors see. This will either wire those header and progress-bar options into the live modal or remove the tab so it isn't misleading. (#294)

## Flows

- **[Task]** **Fix styling issues on the Flow form** — Parts of the Flow form look unstyled or awkward, with fields stacking vertically instead of sitting side by side. This tidies up the form so it matches the polished look of the Placement and Modal forms. (#152)

## Dashboard & Reports

- **[Task]** **Confirm dashboard report numbers match the old system** — During testing, some dashboard report figures didn't line up with the previous system, making it hard to verify. This investigation pinpoints why and confirms the numbers can be trusted. (#271)

## Behind the Scenes

- **[Task]** **Set up a safe, read-only test environment** — Standing up a copy of New Adsmith Frontend using production-like data for verification, locked to read-only so testing can happen without any risk of changing real data. (#270)
- **[Feature]** **Turn Slack conversations into tracked to-dos automatically** — An internal helper that reads designated Slack channels and files action items as tracked issues, reducing manual copy-paste work for the team. No direct effect on the product screens you use. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->
