# Open Issues — Plain-Language Overview

_Last updated 2026-07-21 09:49:48 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview shows your unsaved changes** — When editing a placement or offer, the Preview button will show the edits you've made right now, so you no longer have to save first just to see how a change looks. (#292)
- **[Bug]** **Some offer settings weren't reaching live ads** — A number of saved offer options were being dropped before they reached visitors. This fix makes sure the choices you configure actually take effect on the live experience. (#295)
- **[Bug]** **Success tracking pixels weren't firing** *(high priority)* — Conversion pixels set up on offers were silently never firing, which meant lost tracking and revenue signal. Once fixed, configured success pixels will fire reliably. (#297)
- **[Feature]** **Automatic performance estimate for new offers** — Instead of a manual gut-check, new offers will get a data-driven projection of likely performance based on your historical offers. This is an early, exploratory decision aid at intake time. (#322)
- **[Task]** **Auto-register offers now respect visitor targeting** *(high priority)* — Auto-register offers were firing for everyone, ignoring age, gender, state, zip, and device targeting. This work makes them honor the same targeting rules as regular offers so they only fire for the right visitors. (#333)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — This offer field can be filled in but has no effect on what visitors see. This work confirms the intended behavior and makes the field actually work (or removes it if it isn't needed). (#351)

## Admin / Users

- **[Task]** **Review of the Users area vs. the old system** — A side-by-side comparison of the old and new Users management screens, highlighting missing pieces (like bulk actions, last-login, and two-factor status) so they can be prioritized. This is planning documentation. (#80)
- **[Feature]** **Tidying up admin controls that do nothing** — Certain settings (such as the Advertiser Web Presence tab, some user permission toggles, and a few data-client options) are saved but have no real effect. They'll be hidden or removed so the admin screens only show controls that actually do something. (#296)

## Surveys

- **[Feature]** **Design choices reflected in the live survey** — Every customization option on the Design tab will be checked to confirm it actually shows up in the survey visitors see, with any disconnected options fixed. (#288)
- **[Feature]** **Finishing the Placement design settings** — Several placement Design-tab settings (such as height and display format) don't currently change the live widget. This work connects them so your settings take effect, or removes ones that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bringing back post-conversion delivery steps** — Certain "after success" delivery and redirect behaviors from the old system haven't been carried over yet. This restores them so those clients keep working as before. (#327)
- **[Feature]** **Restoring custom pre-check rules for data clients** *(high priority)* — A large group of data clients relied on custom serve-time validation checks that aren't running on the new platform. This work brings those checks back so the right visitors are validated before delivery. (#338)

## Modals

- **[Feature]** **Making the Modal Design tab do something** — The Modal Design tab (header title, subtitle, colors, progress bar) currently has no effect on the modal visitors see. This work either makes those settings work or removes the tab if a header isn't wanted. (#294)

## Flows

- **[Task]** **Cleaning up the look of the Flow form** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly. This fixes the appearance so it matches the polished look of other forms. (#152)

## Properties

- **[Bug]** **Domain allowlist will actually be enforced** — A property's allowed-domains list is saved but currently isn't checked, meaning ads could serve from any website. This fix blocks requests from sites that aren't on the list, while leaving properties with no list set unaffected. (#350)

## Reports

- **[Task]** **Confirming dashboard numbers match the old system** — Some dashboard report figures didn't line up with the legacy app during testing. This investigation compares the two over a fixed date range to find any differences and confirm the numbers are trustworthy. (#271)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of New Adsmith Frontend that uses real-like data for review and testing, with all changes blocked so nothing can be altered. (#270)
- **[Feature]** **Turning conversations into tracked to-dos automatically** — An internal helper that reads team conversations and files them as tracked work items, reducing manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
