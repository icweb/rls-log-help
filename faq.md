---
title: Frequently Asked Questions
subtitle: Quick answers about features, data, and how the app works.
description: Frequently asked questions about the RLS Log iOS app.
---

## Getting started

<details markdown="1">
<summary>What does RLS Log actually do?</summary>

It's a private tracker for restless legs syndrome. You log symptoms, meals,
supplements, medications, and sleep — and the app surfaces patterns, triggers,
and a personalized "tonight's forecast" built from patterns in your own
history. The forecast is an observation of your data, not a clinical
recommendation.
</details>

<details markdown="1">
<summary>How long until I get useful insights?</summary>

The first 7–10 days mostly fill the baseline. After about two weeks of regular
logging, the contribution heatmap and trend charts get meaningful. Forecasts
get sharper as your dataset grows.
</details>

<details markdown="1">
<summary>Do I need to log every day?</summary>

No. The more consistent you are, the better the patterns — but the app handles
gaps gracefully. Quick Log on the Today tab is designed for one-tap entries
when you're in a hurry.
</details>

## Data and privacy

<details markdown="1">
<summary>Where is my data stored?</summary>

On your iPhone, and (if you have iCloud enabled) in your private CloudKit
database for syncing across your devices. Nothing goes to our servers — we
don't run any. See the [Privacy Policy]({{ '/privacy.html' | relative_url }}).
</details>

<details markdown="1">
<summary>Do you collect analytics or tracking?</summary>

**We don't.** RLS Log contains no analytics SDKs, no marketing trackers, and no
custom telemetry from us. We don't see what you log, what screens you open, or
even when you launch the app.

To be precise: because the app uses Apple's iCloud and CloudKit to sync your
data across your own devices, Apple's platform-level operational logging
applies — the same logging that runs for every iCloud-enabled app on your
iPhone. Apple is the only party with any visibility there, and the contents of
your CloudKit private database are end-to-end-managed and not visible to us.
We never receive a copy.
</details>

<details markdown="1">
<summary>Can I export my data?</summary>

Yes. Settings → Data → Export gives you a JSON file with everything you've
logged. Save it to Files, share it, or keep it as a backup.
</details>

<details markdown="1">
<summary>How do I delete my data?</summary>

Deleting the app from your iPhone removes the local copy. To remove the iCloud
copy, go to Settings → [Your name] → iCloud → Manage Account Storage → RLS Log
→ Delete Data.
</details>

## Apple Health

<details markdown="1">
<summary>What does the app read from Apple Health?</summary>

Only what's relevant to RLS: sleep analysis, workouts, active energy, step
count, resting heart rate, and (optionally) clinical lab records like
ferritin and vitamin D. Each category is a separate permission you grant in
Settings.
</details>

<details markdown="1">
<summary>What are clinical records and why does the app ask?</summary>

Clinical records are lab results, medications, immunizations, and conditions
that Apple Health imports from your healthcare provider. RLS Log can read
**lab results only**, and only if you opt in — it's used to auto-populate
the lab targets you've set with your doctor so you don't have to type
values manually.
</details>

<details markdown="1">
<summary>Can I turn off Apple Health access later?</summary>

Yes. Settings → Privacy &amp; Security → Health → RLS Log lets you toggle each
category individually or revoke access entirely.
</details>

<details markdown="1">
<summary>Does the app write anything back to Apple Health?</summary>

Only when you log a caffeine or alcohol entry yourself with a specific time.
RLS Log writes that single sample (the milligrams of caffeine, or the number
of standard alcoholic drinks) back to Apple Health so other Health-aware apps
see the same entry. The app does **not** write sleep, activity, workouts,
water, calories, iron, audio exposure, or menstrual data, and it does not
write to Apple Health Records (clinical lab results) — those categories are
read-only.

If you'd rather not have RLS Log write at all, you can revoke the write
permission per-category in **Settings &rarr; Privacy &amp; Security &rarr; Health
&rarr; RLS Log**. Logging caffeine and alcohol in the app keeps working
either way.
</details>

## Goals and labs

<details markdown="1">
<summary>What are Goals?</summary>

Goals are targets you set for yourself — for example, a ferritin level you
and your doctor have agreed on, or "walk 30 minutes a day." The app tracks
progress and can remind you to retest a lab on a schedule.
</details>

<details markdown="1">
<summary>Why does iron / ferritin matter for RLS?</summary>

Iron deficiency is one of the most common physiological contributors to
restless legs symptoms. Many practitioners aim for ferritin above 75–100 ng/mL
in people with RLS. The app makes it easy to track that target alongside your
symptom log. (This is informational, not medical advice — talk to your doctor
about what's right for you.)
</details>

<details markdown="1">
<summary>Can I add lab results manually?</summary>

Yes. Open the Goals tab → tap a lab → Add Result. You can enter the value, the
date drawn, the lab name, and any notes.
</details>

## Predictions and patterns

<details markdown="1">
<summary>How does "tonight's forecast" work?</summary>

The app combines your recent triggers (caffeine, alcohol, late meals, missed
medications, poor sleep), your symptom history for the time of day and day of
week, and any goals or lab values you've flagged as relevant. It produces a
score with **headwinds** (what's working against you tonight) and **tailwinds**
(what's working in your favor) so you can see *why* — not just the number.

The forecast is a pattern-matching observation of your own logs, not a
clinical risk assessment or medical advice.
</details>

<details markdown="1">
<summary>Why is the prediction "still calibrating"?</summary>

The app needs roughly 14 days of data before predictions are stable. Until
then, the Insights banner notes that the model is still warming up.
</details>

<details markdown="1">
<summary>What is the contribution heatmap?</summary>

A grid that highlights which logged items most strongly correlate with your
worst symptom days. It's not a medical diagnosis — it's a visualization of
your own patterns.
</details>

<details markdown="1">
<summary>Does the app use AI? Is it training on my data?</summary>

The predictions and pattern detection run **entirely on your iPhone**, against
your own log history. There are no remote AI calls, no cloud inference, and
no training pipeline that ingests your data.
</details>

## Reminders

<details markdown="1">
<summary>Can the app remind me to log?</summary>

Yes. Settings → Reminders lets you schedule daily prompts at custom times.
</details>

<details markdown="1">
<summary>Can it remind me to retest a lab?</summary>

Yes. When you set a Goal, you can attach a follow-up date and the app will
schedule a local notification.
</details>

## Other

<details markdown="1">
<summary>Does it work with Siri and Shortcuts?</summary>

Yes. Say "Hey Siri, log RLS symptom in RLS Log" — the app name has to be in the phrase or Siri won't know which app you mean. Other built-in phrases include "log my mood in RLS Log," "log water in RLS Log," and "log caffeine in RLS Log." You can also build custom Shortcuts that log specific triggers, start Live Activities, or open the Today tab.
</details>

<details markdown="1">
<summary>Is there a Live Activity?</summary>

Yes. Start a session from the Today tab and the Live Activity surfaces on the
Lock Screen and in the Dynamic Island, with one-tap buttons to log severity
and end the session.
</details>

<details markdown="1">
<summary>How do I send feedback?</summary>

Email **rlslogappsupport@iacwb.com** or use the [Contact page]({{ '/contact.html' | relative_url }}).
</details>

<details markdown="1">
<summary>How much does the app cost?</summary>

**RLS Log is free.** No subscriptions, no in-app purchases, no paywalled
features, no ads.
</details>
