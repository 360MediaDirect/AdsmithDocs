# Open Issues — Plain-Language Overview

_Last updated 2026-07-20 01:51:53 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — Conversion tracking pixels set up on offers currently never fire, so successful conversions go unrecorded. This fix makes configured success pixels fire reliably so you don't lose credit for conversions. High priority. (#297)
- **[Bug]** **Some offer settings never reach the live ad** — Several saved offer options — including the Modal tab fields, "Force More Info Visible," Display URL, and a few data-client flags — are being dropped before they reach visitors. This work makes sure the options you set actually take effect, or clearly retires the ones that aren't needed. (#295)
- **[Bug]** **Auto-register offers ignore targeting rules** — Auto-register offers currently fire for every visitor, even ones who fall outside your age, gender, state, ZIP, or device targeting. This fix makes auto-register offers respect the same targeting rules as regular offers so they only reach the right people. High priority. (#333)
- **[Bug]** **"Conflicting Referrals" field does nothing today** — The Conflicting Referrals box on an offer's Delivery tab is saved but has no effect on which offers show. We're confirming the intended rule with the business and then making the field actually work (or removing it). (#351)
- **[Feature]** **Preview shows your unsaved edits** — On placement and offer edit pages, the Preview button will reflect the changes you've made on screen instead of only the last saved version — so you can check your work before saving. (#292)
- **[Feature]** **Performance projections for new offers** — Explore an automated way to estimate how a new offer is likely to perform, based on your own historical offer data, replacing the current manual gut-check review. Medium priority, exploratory. (#322)

## Surveys

- **[Feature]** **Design choices show up in the live survey** — A full check that every option on the Design tab is actually reflected in what visitors see, across all entity screens, with any unused options fixed or removed. You'll be able to trust that the customizations you set really appear. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A handful of Placement Design-tab settings (like survey height and display format) are saved but not yet applied to the live survey. This work wires them through — or removes ones that aren't needed — so what you configure is what visitors get. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring over legacy post-conversion delivery steps** — The after-success delivery/redirect behaviors from the old system haven't been carried over yet. This work restores them in the new platform so post-conversion handoffs work as they did before. Nearly complete. (#327)
- **[Feature]** **Restore custom pre-ping validation for data clients** — Hundreds of data clients relied on custom serve-time checks in the old system that don't run in the new platform yet. This work brings those checks back so lead validation behaves as expected before cutover. High priority. (#338)

## Admin & Users

- **[Task]** **Users screen review against the old system** — A side-by-side comparison of the old and new Users management screens to spot missing capabilities (like bulk actions and login/2FA details) and plan what to add. This guides bringing the new Users area up to par. (#80)
- **[Feature]** **Remove settings that don't do anything** — Several admin controls (Advertiser Web Presence fields, some user permission toggles, and a few data-client and pre-ping options) are shown but have no effect. We'll hide or remove them so screens only show controls that actually work. (#296)

## Behind the Scenes

- **[Task]** **Safe testing environment against real-world data** — Setting up a read-only staging environment that mirrors live data, so the team can verify the product against realistic information without any risk of changing real records. (#270)
- **[Feature]** **Auto-create tasks from team conversations** — A helper that turns action items mentioned in team chat into tracked work items automatically, reducing manual copy-and-paste. (#272)

## Modals

- **[Feature]** **Make the Modal Design tab work (or remove it)** — Every field on the Modal Design tab is currently saved but never shown to visitors. We'll either make these header and progress-bar settings appear in the visitor modal or remove the tab so it isn't misleading. (#294)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly instead of sitting side by side. This work tidies the layout so the Flow form matches the polished look of other forms. (#152)

## Properties

- **[Bug]** **Make the domain allowlist actually block other sites** — The allowed-domains list on a Property is saved but not enforced, so ads can serve on sites you didn't approve. This fix ensures only the hostnames you list can serve your ads, while properties with no list set stay unaffected. (#350)

## Reports & Dashboard

- **[Task]** **Confirm dashboard numbers match the old system** — Investigate why some dashboard report figures differed from the legacy system during testing, pin down the cause, and either fix it or confirm the numbers are correct. This gives you confidence the reports are accurate. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
