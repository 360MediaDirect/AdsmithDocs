# Open Issues — Plain-Language Overview

_Last updated 2026-07-10 03:04:23 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Feature]** **Campaigns management coming to New Adsmith Frontend** — Campaign management isn't available yet in the new platform. This adds it back, so you'll be able to view, create, and edit campaigns and their offer groups — including question text, CTA text, offer order and quantity, marketing partners, and which offers are attached — just like the old admin. High priority. (#200)
- **[Feature]** **Preview offers with your unsaved changes** — Today the offer preview only shows the last saved version. This lets the Preview reflect edits you've made but haven't saved yet, so you can check your changes before committing them. (#292)
- **[Bug]** **Saved offer settings that never reached the live page** — Several offer options (such as modal settings, "Force More Info Visible," and the display URL) were being dropped before the offer displayed to visitors. This ensures the options you save actually take effect. (#295)
- **[Bug]** **Success tracking pixels weren't firing** — Conversion pixels set up under "Pixels to Fire on Success" were silently never firing, meaning lost tracking. This fixes them so configured pixels fire as expected. High priority. (#297)
- **[Feature]** **Automatic performance projections for new offers** — Instead of a manual gut-check, a new offer can be scored against your historical offer data to estimate how it's likely to perform, giving a data-driven read at intake. (#322)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently fire for everyone, ignoring age, gender, state, ZIP, and device targeting. This makes them honor the same targeting rules as other offers so they only fire for the right visitors. High priority. (#333)
- **[Bug]** **bPerx voucher code missing from the offer preview** — The voucher code line isn't showing on the offer preview (and likely the live survey) on the test environment. This gets the voucher code rendering again. (#344)

## General / Across the App
- **[Feature]** **Protection against two people overwriting each other's edits** — When you open a record someone else is already editing, you'll see it's locked and who has it, and you'll be warned before you can accidentally undo their changes. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will let admins see who changed what and when across offers, placements, advertisers, and more — making it easy to answer "who changed this?" (#276)
- **[Feature]** **Removing settings that don't do anything** — Some admin controls (Advertiser Web Presence fields, certain user permission toggles, and a few data-client and pre-ping options) are saved but have no real effect. They'll be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Bringing the Users area up to full parity** — A review comparing the old Users management with the new one to close gaps like bulk role changes, last-login and two-factor status, and password fields. (#80)
- **[Bug]** **Clearer result when testing an invalid link** — Testing an invalid link currently dumps you on the dashboard. It will instead show a clear error so you know the test failed. (#239)
- **[Task]** **Decide the future of the old file-share page** — Confirming whether the legacy file-share page is still needed or can be retired. (#328)

## Surveys
- **[Bug]** **Voucher code and info links missing on the live survey page** — Voucher codes and the privacy/terms/details links are configured but not showing on the new survey page, even though they appear in the old app. This restores them, which matters for both compliance and passing leads. High priority. (#291)
- **[Feature]** **Make every survey design option actually take effect** — A full check to ensure each customization on the design tab is reflected in what visitors see, with no settings that quietly do nothing. (#288)
- **[Feature]** **Finish connecting placement design settings to the survey** — A few placement design settings (like survey height and display format) are saved but not yet applied on the live survey. This wires them through or cleans them up. (#293)

## Reports
- **[Task]** **Investigating why dashboard numbers don't match the legacy system** — Reviewers noticed report figures differing from the old app. This digs into where the difference comes from and confirms the numbers can be trusted. (#271)
- **[Feature]** **Fixing zero offer-impression counts in placement reports** — Historical placement reports show offer impressions as zero. This populates that figure so past reports read correctly. (#339)

## Pre-Pings
- **[Feature]** **Display-trigger pre-ping checks will run at serve time** — Offers set to check with an advertiser before showing will now actually make that check and be hidden if rejected, matching how the old system worked. High priority. (#337)
- **[Feature]** **Restoring custom pre-ping validations for data clients** — Hundreds of data clients rely on custom pre-check logic from the legacy app that isn't running yet. This ports that logic so those checks work again. High priority. (#338)

## Flows
- **[Task]** **Tidying up the Flow form's appearance** — Some fields on the Flow form look unstyled or stack awkwardly instead of sitting side by side. This brings the form in line with the look of the other forms. (#152)

## Modals
- **[Feature]** **Make the Modal Design tab work — or remove it** — The six design fields on the Modal form currently have no effect on what visitors see. They'll either be wired up to the visitor modal or removed to avoid confusion. (#294)

## Data Clients
- **[Feature]** **Restoring after-success delivery behavior** — Post-conversion delivery and redirect steps from the legacy system haven't been carried over. This ports them so those clients keep working as before. (#327)

## Behind the Scenes
- **[Task]** **A read-only staging environment for testing** — Setting up a safe, look-but-don't-touch environment that mirrors real data, so testing can happen against realistic information without risk. (#270)
- **[Feature]** **Turning conversations into tracked to-do items automatically** — An internal Slack helper that reads discussions and files the resulting tasks automatically, reducing manual note-taking. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 20c05265760e30b087db164aa9ffb7701fea9cb19d23bb2497ef9c503a36041b -->
