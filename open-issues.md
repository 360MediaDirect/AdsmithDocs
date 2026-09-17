# Open Issues — Plain-Language Overview

_Last updated 2026-09-17 06:07:35 UTC · 35 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Manually selected offers now carry over correctly** — For Manual-delivery placements, the exact offers you picked (and their order) will show up and display just like the legacy app, instead of the selection coming through empty. (#370)
- **[Feature]** **Preview shows your unsaved changes** — When you click Preview while editing a placement or offer, you'll see your current in-progress edits reflected right away, instead of having to save first. (#292)
- **[Bug]** **Saved offer settings reach the live experience** — Fixes cases where certain options you filled in on an offer weren't actually being carried through to what visitors see. Each option will either work end-to-end or be cleaned up. (#295)
- **[Bug]** **Auto-register offers respect the same rules** — Auto-registered offers will honor the same duplicate, conflict, and address-matching checks as regular offers, so an offer won't fire when it shouldn't. (#355)
- **[Bug]** **"Conflicting Offers" setting works again** — Fixes a problem where the conflicting-offers list set in the current admin wasn't being enforced, which could let mutually exclusive offers appear together. (#358)
- **[Bug]** **Offer-group counts read accurately** — Fixes a behind-the-scenes data quirk that could make an offer-group list come back empty, so offer counts display correctly. (#372)
- **[Feature]** **A decision on the HubSpot List ID field** — This field on offers currently does nothing; the team will either build a real HubSpot connection or remove the field so it's no longer misleading. (#362)
- **[Feature]** **Automatic performance projection for new offers** — Explores giving an at-a-glance estimate of how a new offer is likely to perform, based on your own historical offer data, replacing today's manual review. (#322)

## Data Clients

- **[Feature]** **Custom pre-ping checks brought over** — Restores the per-client pre-ping validation from the legacy system (used by hundreds of data clients) so those checks run on the new platform. (#338)
- **[Feature]** **After-success delivery steps restored** — Re-adds the post-conversion delivery and redirect behavior certain clients rely on after a lead succeeds, so those flows work the same as before. (#327)
- **[Bug]** **Accurate lead validation for manually processed leads** — Leads processed through the manual/broker path will be validated for real instead of always reporting "valid," matching the survey flow. (#366)

## Dashboard & Reports

- **[Feature]** **Today's numbers on the Dashboard** — Adds live, up-to-the-hour stats (impressions, clicks, leads, revenue) for the "today" view so the Dashboard reflects current activity. (#34)
- **[Task]** **Checking report numbers against the legacy system** — A high-priority investigation into why some Dashboard report totals didn't match the old system, to pin down the cause and confirm the numbers can be trusted. (#271)

## Surveys

- **[Feature]** **Design settings fully reflected in the live survey** — Every customization on the Design tab will actually appear in the survey visitors see, and all form options across the product are being audited so none are left disconnected. (#288)
- **[Bug]** **More reliable lead submission** — Prevents survey lead submissions from timing out when several outside checks run back-to-back, so visitors get a clean result instead of an error. (#367)

## Admin & Users

- **[Task]** **Users area feature-gap review** — A detailed comparison of the Users screens against the legacy system to catch missing pieces (like bulk actions and role changes) and prioritize what to add. (#80)
- **[Feature]** **Removing controls that don't do anything** — Admin controls that look like they change something but currently have no effect (some user permissions, data-client, and pre-ping options) will be hidden or removed to avoid confusion. (#296)

## Advertisers

- **[Feature]** **Per-advertiser pre-ping checks** — Confirms each active advertiser's pre-ping is set up correctly before switching over, so leads are validated properly for every advertiser. (#41)

## Modals

- **[Feature]** **Redesigned visitor modal (voucher style)** — The visitor modal will get the richer legacy look: a personalized header with a voucher number, a color-coded progress bar for each offer, branded offer rows with "Claim Offer" and "No Thanks," and a secure footer. (#386)

## Behind the Scenes

- **[Feature]** **Faster historical reporting** — Maintenance that summarizes stats ahead of time so historical reports load more quickly. (#35)
- **[Task]** **Speeding up the Survey engine** — Adding a caching layer so surveys and offers load faster. (#42)
- **[Task]** **Safety-testing the new pre-ping system** — Running the new and old pre-ping side by side to confirm they agree before switching over. (#40)
- **[Task]** **Running new scheduled jobs alongside the old ones** — Deploying the new automated background jobs in parallel to verify they match before the switch. (#43)
- **[Task]** **Retiring legacy scheduled jobs — group 3** — Turning off the lowest-risk legacy background jobs once their replacements prove stable. (#44)
- **[Task]** **Retiring legacy scheduled jobs — group 2** — Turning off the next set of legacy background jobs after group 3 is stable. (#45)
- **[Task]** **Retiring legacy scheduled jobs — group 1** — Carefully turning off the most critical legacy background jobs, with the ability to switch back instantly if needed. (#46)
- **[Task]** **Documenting how to roll back** — Writing clear steps to safely revert each system if something goes wrong. (#48)
- **[Task]** **Troubleshooting guides for common issues** — Creating quick-reference guides for handling problems like lead-processing or stats hiccups. (#49)
- **[Task]** **Reviewing an old stats job** — Checking whether a legacy stats process is still needed or can be retired. (#33)
- **[Task]** **Master tracking of the legacy-to-new transition** — A single place to see overall progress toward matching everything the old system did. (#319)
- **[Task]** **Weekly progress scorecard** — An automated weekly snapshot of how close the new platform is to full parity with the legacy system. (#323)
- **[Task]** **Automated end-to-end testing in the release process** — Making sure the full suite of automated checks runs on every update so issues are caught before they reach users. (#376)
- **[Task]** **More reliable automated testing** — Cleaning up test data handling so automated checks are steadier and don't interfere with each other. (#377)
- **[Task]** **Automated testing review and fixes** — A review of the automated test suite, with several improvements already underway. (#379)
- **[Feature]** **Slack tool to capture action items** — Explores a helper that turns conversations into tracked tasks automatically, reducing manual note-taking. (#272)

---

_This page is generated automatically from open issues and refreshes daily. Please don't edit it by hand — changes will be overwritten._
