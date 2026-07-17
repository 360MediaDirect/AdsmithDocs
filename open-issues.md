# Open Issues — Plain-Language Overview

_Last updated 2026-07-17 19:26:11 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers & Placements

- **[Feature]** **Preview shows your unsaved edits** — When you use the Preview button while editing a placement or offer, you'll see your current changes reflected right away, without having to save first. (#292)
- **[Feature]** **Placement design settings that actually take effect** — Several look-and-feel settings on a placement's Design tab (like survey height and display format) will now carry through to what visitors actually see, so nothing you set there is quietly ignored. (#293)
- **[Bug]** **Offer settings no longer get lost before going live** — A number of saved offer options currently drop out before reaching the live experience. This fix makes sure the settings you configure on an offer are the ones that get used. (#295)
- **[Bug]** **Success tracking pixels will fire correctly** — Conversion pixels set up on offers currently never fire, meaning completed conversions weren't being counted. This high-priority fix restores that tracking so you don't lose attribution. (#297)
- **[Feature]** **Automatic performance projection for new offers** — Instead of relying on a manual gut-check, new offers will get a data-driven estimate of how they're likely to perform, based on your own historical offer results. (#322)
- **[Bug]** **Auto-register offers will respect visitor targeting** — Certain automatic offers currently ignore age, gender, state, ZIP, and device targeting and can show to people they shouldn't. This high-priority fix makes them honor the same targeting rules as regular offers. (#333)
- **[Bug]** **"Conflicting Referrals" field will do what it says** — This offer field is saved today but has no effect. The work confirms the intended rule and makes it actually influence which offers are served. (#351)

## Admin & Users

- **[Task]** **Bringing the Users area up to par with the old system** — A detailed review of the new Users screens against the previous version, so missing conveniences (like bulk actions, extra columns, and filters) can be added back. (#80)
- **[Feature]** **Removing controls that don't do anything** — Several admin settings currently appear on screen but have no effect (for example the Advertiser Web Presence fields and some user-permission toggles). These will be hidden or removed so the interface only shows options that truly work. (#296)

## Data Clients & Pre-Pings

- **[Feature]** **After-success delivery steps carried over from the old system** — Post-conversion delivery and redirect behaviors that ran in the legacy platform will be brought into New Adsmith Frontend, so client hand-offs keep working as before. (#327)
- **[Feature]** **Restoring custom pre-ping checks for data clients** — Hundreds of data clients relied on custom validation checks that don't yet run in the new platform. This high-priority effort brings those checks back so leads are validated as intended. (#338)

## Surveys

- **[Feature]** **Design choices that reliably show up in the survey** — A thorough review to make sure every customization option on the design side actually appears in the live survey, with no settings that quietly go nowhere. (#288)

## Modals

- **[Feature]** **Fixing the Modal Design tab** — Every field on the Modal Design tab currently has no effect. These will either be wired up to change the visitor pop-up or removed, so what you set is what you get. (#294)

## Flows

- **[Task]** **Tidying up the look of the Flow form** — Some parts of the Flow form appear unstyled or misaligned. This clean-up makes text boxes, color pickers, and paired fields look consistent with the rest of the app. (#152)

## Properties

- **[Bug]** **Domain allowlist will actually block other sites** — A property's list of allowed domains is currently ignored, so ads can serve on any site. This fix ensures ads only appear on the domains you've approved. (#350)

## Dashboard & Reports

- **[Task]** **Making dashboard numbers match the old system** — An investigation into why some dashboard report figures differ from the legacy platform, so you can trust that the reports line up. (#271)

## Behind the Scenes

- **[Task]** **A safe test environment mirroring live data** — Setting up a read-only copy of the system loaded with realistic data, used for verification and testing without any risk to live information. (#270)
- **[Feature]** **Turning conversations into tracked work automatically** — A helper that captures action items from team chats and files them as tracked tasks, reducing manual note-shuffling behind the scenes. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
