---
title: Privacy Policy
subtitle: What stays on your device, what syncs, what we never collect.
description: Privacy policy for the RLS Log iOS app.
---

**Effective:** April 26, 2026 at 9:50 AM ET

RLS Log is built around a simple promise: **your health data stays yours.** This
policy explains what the app stores, where it's stored, and what we never do
with it.

## The short version

- We don't run a server. There is no "RLS Log account."
- All your logs live on your device and (optionally) in your private iCloud.
- We don't collect analytics, telemetry, or crash reports about your health data.
- We don't sell, share, or monetize anything you log.
- Apple Health data and clinical records you grant access to never leave your
  device.

## What the app stores

When you use RLS Log, the app saves:

- **Symptom logs** — severity, side affected, time, and any notes you add.
- **Triggers** — meals, supplements, medications, caffeine, alcohol, exercise,
  hydration, and other lifestyle entries you log.
- **Sleep entries** you record manually.
- **Goals** — targets you set (for example, "ferritin above 75 ng/mL") and
  follow-up dates.
- **Lab results** you enter manually or import from Apple Health clinical
  records.
- **Settings and preferences** — units, reminder times, which Today-tab cards
  you've enabled.

## Where your data is stored

- **On your device.** All logs are stored locally using Apple's SwiftData
  framework. The data lives in the app's sandboxed container.
- **In your private iCloud (optional).** If iCloud is enabled on your device,
  your logs sync across your own Apple devices using **CloudKit private
  database** — a private, end-to-end-managed iCloud space that only you can
  access. We cannot read it, and Apple does not share it with us.
- **Nothing on our servers.** RLS Log has no backend. We don't operate a
  database that holds your records.

## Apple Health and clinical records

RLS Log can read from Apple Health, but only with your explicit per-category
permission, and only the categories relevant to RLS:

- **Sleep analysis** — to correlate sleep quality with symptoms.
- **Workouts and active energy** — to track exercise patterns.
- **Step count and resting heart rate** — for daily-context summaries.
- **Clinical health records (optional)** — specifically lab results
  (`HKClinicalTypeIdentifierLabResultRecord`) to import iron studies, ferritin,
  vitamin D, and similar markers. This is opt-in and off by default.

What we **don't** do with Apple Health data:

- We don't write your Apple Health data to any server.
- We don't share it with third parties or analytics services.
- We don't keep a copy outside your device.
- Imports and reads happen in-process on your iPhone. The data never travels
  off-device unless you choose to export it yourself.

You can revoke any Apple Health permission at any time in **Settings → Privacy
& Security → Health → RLS Log**.

## What we don't do

- **No analytics SDKs.** RLS Log does not include Firebase, Mixpanel, Amplitude,
  Google Analytics, Segment, or any other analytics SDK.
- **No third-party trackers.** No advertising SDKs. No marketing pixels.
- **No custom telemetry.** We don't see what you log, what screens you open,
  or even when you launch the app.
- **No crash-reporting that includes user data.** The app does not send crash
  reports to us. (Apple's standard, anonymized App Store crash reports may be
  delivered to us through App Store Connect — these contain only stack traces,
  never your logs.)
- **No selling or sharing.** We don't sell, rent, or share your data with
  anyone, ever.

## A note on Apple's platform logging

Because the app uses Apple's iCloud and CloudKit to sync your data across your
own devices, Apple's platform-level operational logging applies — the same
logging that runs for every iCloud-enabled app on your iPhone. Apple is the
only party with visibility into that, and the contents of your CloudKit private
database are end-to-end-managed and not visible to us. We never receive a copy
of your data, your sync activity, or any usage signals from Apple.

## No AI training, no data centers

The predictions and pattern detection in RLS Log run **entirely on your
iPhone**, against your own log history. There are no remote AI calls, no cloud
inference, and no training pipeline that ingests your data. The app does not
run servers in a data center on your behalf — so there's no GPU power and no
water cooling burning energy to crunch your numbers.

## Device identifiers

RLS Log does not collect or use any device identifiers for tracking. Specifically:

- **No IDFA** (Identifier for Advertisers). The app does not request the App
  Tracking Transparency permission and does not access the IDFA at all.
- **No IDFV** (Identifier for Vendor). The app does not read or persist the
  IDFV.
- **No fingerprinting.** No combinations of device or environment signals are
  collected to derive a stand-in identifier.

## App Store privacy nutrition label

The app's App Store privacy label is **"Data Not Collected"** — the developer
does not collect any data from this app. This page describes the same posture
in plain language. If anything in the App Store label and this policy ever
appear to disagree, treat the App Store label as the binding declaration and
let us know at **rlslogappsupport@iacwb.com** so we can correct the discrepancy.

## Notifications

If you enable reminders or follow-up notifications, the app schedules them
locally on your device using Apple's notification system. The notification
content stays on-device and is not routed through any server.

## Home Assistant and other integrations

RLS Log can optionally connect to your own Home Assistant instance — for
example, to read sleep-tracker, temperature, or motion-sensor states from your
home and correlate them with your symptoms.

This integration is **read-only**. RLS Log does **not**:

- Send any of your symptom logs, meals, supplements, medications, lab results,
  or any other RLS Log data to Home Assistant.
- Write, modify, or store anything on your Home Assistant server.
- Share any data you've logged in the app with Home Assistant or any other
  third-party service.

Requests go directly from your iPhone to your own Home Assistant URL over your
local network or VPN. We don't proxy them, observe them, or know that they
happen. The endpoint and credentials you configure stay on your device. The
same applies to any other local service you point the app at — it's a
user-directed local network read, not a data export.

## Children's privacy

RLS Log is not directed to children under 13 — or the applicable age of
digital consent in the user's jurisdiction (for example, up to 16 in some EU
member states under the GDPR) — and does not knowingly collect data from
children. The App Store rates the app appropriately for medical content.

## Exporting and deleting your data

- **Export.** Settings → Data → Export creates a JSON file containing all your
  logs, which you can save to Files, share, or back up.
- **Delete on this device.** Deleting the app from your iPhone removes all
  local data.
- **Delete from iCloud.** Settings → [Your name] → iCloud → Manage Account
  Storage → RLS Log → Delete Data. This removes the iCloud copy used for
  syncing.

## Changes to this policy

If we materially change this policy, we'll update the **Effective** timestamp at the
top of this page and surface a note in the app. The previous version remains
in this site's git history.

## Contact

Questions about privacy? Email **rlslogappsupport@iacwb.com**. We read every message.
