# Open Issues — Plain-Language Overview

_Last updated 2026-07-01 01:45:10 UTC · 11 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range picker for the dashboard filter** — Choosing "Custom" on the date filter will open a proper calendar picker where you can set a start and end date, then apply it to see exactly the range you want. The selected range shows on the filter button, and end dates can't come before start dates. (#58)
- **[Feature]** **Pick report dates without editing the web address** — Today, viewing a specific day or range means hand-editing the address bar, which is easy to get wrong. New date controls in the dashboard toolbar let you pull daily or custom-range reports directly, while still keeping links shareable. (#268)

## Campaigns

- **[Feature]** **Bring the Campaigns module to the new platform** — Campaign management from the old admin isn't available yet in New Adsmith Frontend. This high-priority work adds the ability to view, create, edit, and configure campaigns — including offer groups, offer handling, CTA text, and marketing partners — so this core workflow can be done in the new system. (#200)

## Placements

- **[Feature]** **Smarter offer ordering and filtering on Placements** — Following earlier drag-to-reorder improvements, this sets new placements to use your manual offer order by default (so the order you set actually takes effect), and adds a way to filter the available offers list by category/vertical instead of only searching by text. (#275)

## Users

- **[Task]** **Close the gaps between the old and new Users area** — A detailed review of the old Users screens versus the new ones highlights missing pieces to bring back, such as bulk-selecting users to change their roles at once, a password field and welcome-email option when adding a user, and login/two-factor details in the list. This work tracks getting the new Users area up to full parity. (#80)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned — plain text boxes, unstyled color pickers, and paired fields stacking vertically instead of side by side. This work restores consistent styling to match the Placement and Modal forms. It's partly done, with the rest handled carefully to avoid disrupting other tabs. (#152)

## Link Testing

- **[Bug]** **Clear error when testing an invalid link** — Right now, entering an invalid link quietly sends you to the dashboard with no explanation. This fix makes Link Testing show a clear failure message so you know the link didn't work. (#239)

## Reports

- **[Task]** **Confirm report numbers match the old system** — During testing, some dashboard report figures didn't line up with the legacy system. This investigation compares the two over the same date range, pinpoints where any differences come from, and either fixes them or confirms the numbers are correct — so you can trust your reports. (#271)

## Audit

- **[Feature]** **A searchable history of changes across the app** — A new admin "Audit Log" will record who changed what and when — covering manual edits (like pausing offers or updating placements) and automated system changes. You'll be able to search and filter by entity, person, action, or date, and view a change history right from each item's detail page. (#276)

## Behind the Scenes

- **[Task]** **A safe testing environment with recent data** — A separate staging environment loaded with May and June data lets the team validate reports and test changes without ever touching live information. (#270)
- **[Feature]** **Turn conversations into tracked work automatically** — A helper that reads designated team chat channels and turns action items into properly labeled tickets, reducing manual copy-and-paste and helping make sure requests don't slip through the cracks. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 18c895dd2d51d67625ab25b86c398b76285d058485c5365f84641d856758854b -->
