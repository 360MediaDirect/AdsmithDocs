# Open Issues — Plain-Language Overview

_Last updated 2026-07-17 23:17:29 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — When an advertiser sets up conversion tracking pixels to fire on a successful lead, they currently don't fire at all, silently, so credit for those conversions is being lost. This high-priority fix makes configured success pixels fire reliably again. (#297)
- **[Bug]** **Auto-register offers ignore audience targeting** — Offers that register visitors automatically are currently being shown to everyone, even people they should exclude by age, gender, state, ZIP, or device. This fix makes those offers respect the same targeting rules as regular offers so they only reach the intended audience. (#333)
- **[Bug]** **Some saved offer settings never take effect** — A number of options you can set on an offer (including Modal tab settings, Force More Info, Display URL, and several data-client flags) are saved but never actually used when the offer runs. Each will either be made to work or removed so the form only shows options that do something. (#295)
- **[Bug]** **"Conflicting Referrals" field does nothing today** — This offer field can be filled in but has no effect on which offers get shown. It's being reviewed to confirm the intended rule and then either wired up to work or removed to avoid confusion. (#351)
- **[Feature]** **Preview your unsaved changes** — On placement and offer edit pages, the Preview button currently shows the last saved version, not your in-progress edits. Once updated, you'll be able to preview changes before saving. (#292)
- **[Feature]** **Predict how a new offer will perform** — Explores an automated way to estimate a new offer's likely performance based on your own historical offer data, replacing today's informal manual gut-check. This would give you a data-driven projection at intake. (#322)

## Surveys

- **[Feature]** **Make sure every design option actually shows up** — A thorough check across all entity forms to confirm that each design and customization option you set is truly reflected in the live survey view, with any dead options fixed or removed. Fewer settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting Placement design settings** — Several placement design options (such as survey height and display format) are saved but not yet applied to the live widget. This finishes wiring them so your choices take effect, or removes any that aren't needed. (#293)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — Right now every field on the Modal Design tab (header text, colors, progress bar, and more) is saved but has no effect on what visitors see. These will either be made to work in the visitor modal or removed so the tab isn't misleading. (#294)

## Data Clients & Pre-Pings

- **[Feature]** **Restore custom pre-ping checks for data clients** — Hundreds of data clients relied on custom validation checks at serve time that don't currently run on the new platform. This high-priority work brings that behavior back so each client's checks are applied again. (#338)
- **[Feature]** **Bring back after-success delivery steps** — Post-conversion delivery and redirect behaviors from the legacy system hadn't been carried over. This adds a flexible, configurable version so those after-success steps work again. (#327)

## Admin & Users

- **[Task]** **Users area gap review vs. the old system** — An ongoing comparison of the old Users screens against the new ones to identify missing capabilities (like bulk actions and extra columns) and prioritize what to add, so the Users area reaches full parity. (#80)
- **[Feature]** **Remove admin controls that don't do anything** — Several admin settings (an advertiser Web Presence tab, some user permission toggles, and a few data-client and pre-ping options) are saved but read by nothing, which can be misleading. These will be hidden or removed, or scheduled to be properly implemented. (#296)

## Behind the Scenes

- **[Task]** **Set up a safe testing environment** — Standing up a review environment that mirrors real data in a read-only way, so the team can verify the product against realistic information without any risk of changing live data. (#270)
- **[Feature]** **Automatically turn conversations into tracked tasks** — A helper that reads designated chat channels and files action items as tracked work automatically, reducing manual copy-paste and helping nothing slip through the cracks. (#272)

## Properties

- **[Bug]** **Enforce the domain allowlist** — A property's list of allowed domains is currently saved but not enforced, so ads can serve on any site, not just approved ones. This fix makes the allowlist actually block unapproved domains as publishers expect. (#350)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly and inputs using plain browser defaults. This tidies up the styling so the Flow form looks consistent with the rest of the app. (#152)

## Dashboard & Reports

- **[Task]** **Confirm report numbers match the old system** — Dashboard report figures didn't line up with the legacy system during testing. This investigation compares the two over a fixed period, finds where any differences come from, and confirms the numbers you see are accurate. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
