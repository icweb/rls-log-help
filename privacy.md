---
title: Privacy Policy
subtitle: What stays on your device, what syncs, what we never collect.
description: Privacy policy for the RLS Log iOS app.
---

**Effective date:** April 26, 2026

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

- **No analytics.** RLS Log does not include Firebase, Mixpanel, Amplitude,
  Google Analytics, Segment, or any other analytics SDK.
- **No third-party trackers.** No advertising SDKs. No marketing pixels.
- **No crash-reporting that includes user data.** The app does not send crash
  reports to us. (Apple's standard, anonymized App Store crash reports may be
  delivered to us through App Store Connect — these contain only stack traces,
  never your logs.)
- **No selling or sharing.** We don't sell, rent, or share your data with
  anyone, ever.

## Notifications

If you enable reminders or follow-up notifications, the app schedules them
locally on your device using Apple's notification system. The notification
content stays on-device and is not routed through any server.

## Home Assistant and other integrations

If you choose to connect RLS Log to your own Home Assistant instance or another
local service, requests go directly from your iPhone to that service over your
network. We don't proxy or observe those requests.

## Children's privacy

RLS Log is not directed to children under 13 and does not knowingly collect
data from children. The App Store rates the app appropriately for medical
content.

## Exporting and deleting your data

- **Export.** Settings → Data → Export creates a JSON file containing all your
  logs, which you can save to Files, share, or back up.
- **Delete on this device.** Deleting the app from your iPhone removes all
  local data.
- **Delete from iCloud.** Settings → [Your name] → iCloud → Manage Account
  Storage → RLS Log → Delete Data. This removes the iCloud copy used for
  syncing.

## Changes to this policy

If we materially change this policy, we'll update the **Effective date** at the
top of this page and surface a note in the app. The previous version remains
in this site's git history.

## Contact

Questions about privacy? Email **support@rlslog.app**. We read every message.
