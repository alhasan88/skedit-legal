---
title: Privacy Policy
permalink: /privacy.html
---

# Privacy Policy

**sKedIt AI**

**Effective date:** 15 May 2026

**Last updated:** 15 May 2026

This Privacy Policy explains what data sKedIt AI ("we", "us", "the app") collects, how we use it, and the choices you have. If anything here is unclear, email **alhasanmuhammadai@gmail.com** and we'll explain in plain language.

## Who runs sKedIt AI

sKedIt AI is operated by **Alhasan Muhammad Hasan**, an independent developer based in Egypt. There is no parent company. You are talking to one person and a small set of trusted service providers.

## What stays on your device

The majority of what you do in sKedIt AI never leaves your phone. The following are stored only in a local SQLite database on your device:

- Schedule blocks, tasks, and goals (titles, times, dates, durations, notes)
- App settings (work hours, wake/sleep time, working days, scheduling mode, etc.)
- Streak counts and completion history
- Usage counters for free-tier limits

When you uninstall the app, this data is deleted with it.

## What we send to our backend

To make voice scheduling and AI features work, the following data leaves your device:

- **Voice recordings:** when you tap the microphone, the audio file is sent to our backend for transcription, then to Anthropic's Claude API for parsing into structured items. **The audio file is discarded immediately after transcription. We do not store recordings on our servers.**
- **Transcripts:** the text version of what you said is processed by Claude, then returned to your device as structured tasks/blocks/goals. We do not retain transcripts after the response is sent back.
- **Task and block summaries:** when you use AI scheduling, reschedule, or goal-scheduling features, a short list of your current pending tasks and existing blocks for the target day is sent to our backend so the AI can plan around them. These are not stored after the response is returned.

We use the following third-party processors for these features:

- **Anthropic (Claude API)** — natural language understanding. Audio is never sent here; only text.
- **OpenAI (Whisper API)** — audio-to-text transcription. Audio is processed and discarded.
- **Supabase Edge Functions / Modal.com** — backend hosting that orchestrates the above. Does not store your content.

These providers process data on our behalf and are contractually bound not to use it for any other purpose. They do not sell, share, or train models on your data when accessed via their paid APIs.

## What we store remotely

A small amount of data is stored on our servers (via Supabase, hosted in the EU/US depending on your region):

- **Your email address** — used to sign you in.
- **Your display name** — if you provided one during sign-up or via Apple Sign In.
- **Authentication tokens** — stored encrypted on your device in iOS Secure Enclave (via expo-secure-store), and managed by Supabase's auth service on the server side.
- **Subscription status** — whether you're on the Free or Pro plan, and which Apple-issued subscription identifier corresponds to your account. Apple handles the payment; we never see your card, name, or address.

That is the complete list of remotely stored personal data.

## What we DO NOT do

- We **do not** use analytics tools (no Google Analytics, no Amplitude, no Mixpanel, no Sentry).
- We **do not** track your behaviour across the app or anywhere else.
- We **do not** show advertisements.
- We **do not** sell, rent, or share your data with any third party for marketing, profiling, or any commercial purpose.
- We **do not** allow Anthropic, OpenAI, or any other API provider to use your data for model training (all calls use paid APIs with no-training terms).
- We **do not** collect device identifiers, location, contacts, photos, calendar, or any other resource not explicitly listed above.

## How long we keep data

- **Local data on your device:** until you delete it manually, clear the app data via "Delete account & data" in Profile, or uninstall the app.
- **Account email and subscription status:** retained as long as your account exists. When you delete your account (Profile → Delete account & data), your auth record, AI usage history, and subscription record are removed from our servers **immediately** via a server-side function. If our server is temporarily unreachable at the moment of deletion, we fall back to a manual deletion process completed within 14 days.
- **Voice recordings:** discarded immediately after transcription (typically within seconds of the API call returning).
- **Transcripts and task summaries sent to AI APIs:** not stored by us. Anthropic and OpenAI may retain API logs for a short period for abuse prevention as described in their respective policies; we do not have access to these logs.

## Your rights

You can, at any time:

- **Access** your data — everything we hold about you is visible inside the app.
- **Correct** your data — edit your name in Profile, edit any task/block directly.
- **Delete** your data — Profile → "Delete all data" wipes both your device and your server-side record.
- **Export** your data — email us and we'll send a JSON export within 30 days.
- **Object to processing or withdraw consent** — uninstall the app, and email us to delete your remote account.
- **Complain to a supervisory authority** — if you are in the EU/UK, you may lodge a complaint with your local data protection authority.

To exercise any of these rights, email **alhasanmuhammadai@gmail.com**. We respond within 14 days.

## Children

sKedIt AI is not directed at children under 13. We do not knowingly collect personal data from children under 13. If you believe a child has provided us with personal data, email us and we will delete the account.

## Security

- Authentication tokens are stored in iOS Secure Enclave via expo-secure-store.
- Backend traffic is over HTTPS/TLS only.
- Supabase enforces row-level security so that each user can only read and write their own records.
- API keys for third-party services (Anthropic, OpenAI) are kept on the server only, never embedded in the app.

No system is perfectly secure. If we discover a breach involving your data, we will notify you by email within 72 hours of becoming aware of it.

## International transfers

Our backend (Supabase, Anthropic, OpenAI) may process data in the United States or the European Union. By using sKedIt AI you agree to these transfers. We rely on each provider's Standard Contractual Clauses (SCCs) for cross-border data flow.

## Changes to this policy

We may update this policy as the app evolves. When we make material changes, we'll update the "Last updated" date at the top and, for significant changes, notify you in-app on next launch.

## Governing law

This policy is governed by the laws of the Arab Republic of Egypt.

## Contact

For any privacy question, data request, or concern:

**Email:** alhasanmuhammadai@gmail.com

**Operator:** Alhasan Muhammad Hasan, Egypt
