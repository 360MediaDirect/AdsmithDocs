# Open Issues — Plain-Language Overview

_Last updated 2026-07-21 11:34:48 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Preview reflects your unsaved changes** — When previewing a placement or offer you're editing, the preview will show your current, in-progress changes instead of the last saved version — so you can check your work before committing it. (#292)
- **[Bug]** **Some saved offer settings don't reach the live ad** — Several offer options you set (including modal-tab settings and a few delivery flags) are saved but never actually applied to what visitors see. This work makes sure each saved option either takes effect or is cleared out. (#295)
- **[Bug]** **Success pixels not firing** — A high-priority fix: conversion tracking pixels set up on offers were silently never firing, causing lost tracking. After this fix, configured success pixels will reliably fire. (#297)
- **[Feature]** **Automatic performance projections for new offers** — Instead of relying on a manual gut-check, you'll get a data-driven estimate of how a new offer is likely to perform, based on your own historical offer results. This is exploratory work. (#322)
- **[Task]** **Auto-register offers now respect targeting rules** — A high-priority fix: auto-register offers were being shown to visitors they should have excluded (by age, gender, state, zip, or device). This ensures those offers honor the same targeting rules as regular offers. (#333)
- **[Bug]** **"Conflicting Referrals" field now takes effect** — The Conflicting Referrals setting on the offer Delivery tab is saved but currently does nothing. This work confirms the intended rule and makes the field actually exclude the right offers (or removes it if not needed). (#351)

## Surveys

- **[Feature]** **Design-tab options fully reflected in the survey** — An audit across all entities to confirm every design and customization option you set actually shows up in the live survey, with no settings that quietly do nothing. (#288)
- **[Feature]** **Placement design settings applied to the widget** — Several placement Design-tab settings (like survey height and display format) are saved but not yet used by the live widget. This finishes connecting them so your choices take effect, or removes any that aren't needed. (#293)

## General / Across the App

- **[Task]** **Users screen: closing gaps with the previous version** — A review comparing the older Users management screen with the new one, guiding which features (like bulk actions and login details) still need to be brought over. This is a documentation and planning update. (#80)
- **[Feature]** **Removing controls that don't do anything** — Some admin settings (Advertiser Web Presence fields, certain user permission toggles, and a few Data-Client and Pre-Ping options) are saved but have no effect. These will be hidden or removed so the screens only show controls that actually work. (#296)

## Data Clients

- **[Feature]** **Post-conversion delivery steps carried over** — Custom actions that run after a successful conversion for certain clients weren't yet available in New Adsmith Frontend. This work brings them over so those clients keep working as before. (#327)
- **[Feature]** **Restoring per-client pre-ping validation** — A high-priority gap: custom serve-time checks that hundreds of data clients rely on aren't running on the new platform. This work maps and restores those checks so those clients validate correctly again. (#338)

## Behind the Scenes

- **[Task]** **Read-only staging environment for testing** — Setting up a safe, view-only test environment loaded with production-like data, so the team can verify behavior without any risk of changing real records. (#270)
- **[Feature]** **Automatic issue capture from team chat** — A helper that turns action items from team conversations into tracked work items automatically, reducing manual copy-and-paste. (#272)

## Modals

- **[Feature]** **Modal Design tab connected (or cleaned up)** — The Modal Design tab's settings (header title, subtitle, colors, and progress bar) are saved but not shown to visitors. This work either makes them appear in the modal or removes the tab if it isn't needed. (#294)

## Properties

- **[Bug]** **Domain allowlist now enforced** — A Property's allowed-domains list is currently ignored, so any website could serve its ads. This fix makes the allowlist actually block requests from domains you haven't approved, while properties without a list keep working unchanged. (#350)

## Flows

- **[Task]** **Cleaner, consistent Flow form styling** — Parts of the Flow form appear unstyled or misaligned, with fields stacking oddly instead of sitting side by side. This work brings the form's look in line with the Placement and Modal forms. (#152)

## Reports

- **[Task]** **Confirming report numbers match the previous system** — Dashboard report figures didn't line up with the older system during testing. This investigation pins down where the difference comes from and confirms the new reports are accurate. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
