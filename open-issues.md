# Open Issues — Plain-Language Overview

_Last updated 2026-07-20 11:59:26 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Some saved offer options never reach live ads** — Several settings you configure on an offer (including the Modal tab fields, "Force More Info Visible," Display URL, and various data-client flags) are currently dropped before they take effect. This work makes sure each option either works as expected or is removed so nothing on the form is misleading. (#295)
- **[Bug]** **Success pixels will actually fire** — High priority. Right now, the "Pixels to Fire on Success" you set up on an offer silently never fire, meaning conversions aren't being tracked. This fix restores that tracking so your attribution and revenue signals come through correctly. (#297)
- **[Feature]** **Automatic performance projection for new offers** — When a new offer comes in, you'll get a data-driven estimate of how it's likely to perform, based on your own historical offers — replacing the informal manual gut-check review. Think of it as a helpful decision aid at intake. (#322)
- **[Bug]** **Auto-register offers will respect visitor targeting** — High priority. Today, auto-register offers ignore your age, gender, state, zip, and device targeting and can fire for visitors they should exclude. This work makes them honor the same targeting rules as regular offers. (#333)
- **[Bug]** **"Conflicting Referrals" field will finally do something** — This field on the offer Delivery tab is currently saved but has no effect at serve time. This work confirms how it should behave and wires it up (or clarifies its purpose) so it isn't a dead setting. (#351)

## Placements

- **[Feature]** **Preview your unsaved edits** — On the placement and offer edit screens, the Preview button will show the changes you're currently making, instead of only the last saved version. No more saving just to see how an edit looks. (#292)
- **[Feature]** **Placement Design tab settings will take effect** — Several Design-tab options (like iFrame height, display format, and skip/more-info behavior) are saved today but don't yet change what visitors see. This work connects each one so your design choices actually show up — or removes any that aren't needed. (#293)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — Certain after-success actions (delivery and redirect steps that ran after a conversion in the old system) weren't carried over. This work brings that behavior back for the clients that still rely on it. (#327)
- **[Feature]** **Bring back file-based pre-ping validation** — High priority. Many data clients rely on custom serve-time checks from the legacy system that currently don't run on the new platform. This work restores those checks so those clients are validated the way they expect before serving. (#338)

## Admin / Users

- **[Task]** **Users area feature comparison** — A documentation review comparing the old Users management screens with the new ones, so any missing capabilities (like bulk actions, last-login, and two-factor status) are identified and prioritized. (#80)
- **[Feature]** **Clean up admin controls that don't do anything** — Some settings across the app (Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) are saved but have no effect. Removing or hiding them means the controls you see actually work, avoiding confusion. (#296)

## Behind the Scenes

- **[Task]** **Set up a safe testing environment** — A staging copy of the app is being prepared using recent production-like data, in read-only mode, so the team can verify behavior without any risk to live data. (#270)
- **[Feature]** **Automatic issue capture from team chat** — A helper that turns action items discussed in team conversations into tracked work items automatically, so nothing gets lost in the shuffle. (#272)

## Reports

- **[Task]** **Confirm dashboard numbers match the old system** — An investigation into why some dashboard report figures didn't line up with the legacy app, to pin down the cause and confirm the new reports are accurate. (#271)

## Surveys

- **[Feature]** **Design customizations that show up everywhere** — A full review to make sure every option on the design tabs is actually reflected in the live survey view across all entity types, with no settings that quietly do nothing. (#288)

## Modals

- **[Feature]** **Make the Modal Design tab work — or retire it** — The entire Modal Design tab (header text, colors, and progress bar options) is saved but never shown to visitors. This work either connects those settings to the visitor modal or removes the tab if it isn't needed. (#294)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or out of place compared to other forms (plain text boxes, misaligned paired fields, unstyled color pickers). This work brings its look in line with the rest of the app. (#152)

## Properties

- **[Bug]** **Domain allowlist will actually block other sites** — The allowed-domains list on a property is currently saved but never enforced, so ads can serve from any website. This fix makes the allowlist work, so offers are only served on the domains you've approved. (#350)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
