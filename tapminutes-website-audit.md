# TapMinutes Website Audit and Compliance Record

Date: September 28, 2026

## 1. Audit of the Previous Public Website

The previous homepage and Help Center contained these inaccurate, ambiguous, or incomplete claims:

- Audio/video imports were described as being sent for online transcription. This omitted Basic on-device transcription and embedded-caption reuse.
- Folders, tags, and bookmarks were presented without clearly stating that creating or editing them requires Pro.
- The homepage said “Record on iPhone, iPad, or Apple Watch,” which could imply standalone Watch recording. Apple Watch is a remote companion for an iPhone recording.
- Export, external sharing, PDF creation, and read aloud were not consistently identified as Pro features.
- Basic’s limits of 3 processed meetings per day, 6 per week, and 20 minutes per meeting were missing.
- The shared allowance between recordings and audio/video imports was missing.
- Basic’s two regenerations were mentioned, but Pro’s unlimited regeneration and the plan distinction were incomplete.
- Pro document import did not accurately list PDF, TXT, SRT, and VTT or explain the lack of DOCX and built-in OCR.
- Embedded caption/transcript detection and the reuse-or-transcribe choice were missing.
- Backup, restore, Recover Saved Recordings, read aloud, custom presets, and one-time purchase behavior were missing or incomplete.
- iCloud wording did not fully distinguish device storage from synchronization through the user’s personal iCloud account.
- The Privacy Policy described audio as leaving the device too broadly and did not clearly distinguish on-device transcription, premium cloud transcription, and AI generation from transcript text.
- The site did not explain that subscription products and one-time purchases may vary by storefront or release state.

## 2. Proposed and Implemented Sitemap

- `/` — Product overview, how it works, labeled feature grid, screenshots, Basic vs. Pro comparison, import compatibility, privacy summary, FAQ, and support CTA.
- `/help.html` — Recording, imports, embedded captions, outputs, organization, iCloud, plans and purchases, backup/recovery, and troubleshooting.
- `/privacy.html` — Device storage, iCloud, on-device transcription, cloud transcription, AI generation, service providers, retention, and user choices.
- `/terms.html` — Redirect to Apple’s Standard End User License Agreement.

No App Store download CTA was added because no verified App Store URL was supplied.

## 3. Production Copy Location

Final production-ready copy is embedded directly in:

- `index.html`
- `help.html`
- `privacy.html`
- `terms.html`

The site uses `styles.css` for responsive presentation and `script.js` only for accessible mobile navigation.

## 4. Claim Change Log

| Previous claim or omission | Corrected replacement |
| --- | --- |
| “Import supported audio and video for online transcription.” | Basic uses on-device transcription on supported iOS versions; Pro uses premium cloud transcription. |
| No embedded-caption behavior | Imported media can be inspected for meaningful caption tracks; users can preview and reuse text or transcribe audio. |
| “Record on iPhone, iPad, or Apple Watch.” | Record on iPhone or iPad; Apple Watch remotely controls the paired iPhone recording. |
| Folders/tags/bookmarks shown as generally available | Creating folders, moving meetings, editing tags, and creating bookmarks require Pro; existing items remain visible when relevant. |
| Export and sharing presented without gating | Copy, external sharing, export, PDF creation/sharing, and read aloud require Pro. |
| No Basic count or duration limits | Basic: 3 processed meetings/day, 6/week, 20 minutes each; allowances are shared between recordings and audio/video imports. |
| “Free users get two regenerations.” | Basic includes two regenerations per meeting; Pro includes unlimited regeneration. |
| General PDF/document import wording | Pro supports text-based PDF, TXT, SRT, and VTT; no DOCX or built-in OCR; PDF extraction may be capped. |
| “iCloud Sync for everyone” without storage context | Basic and Pro can sync meeting data through the user’s personal iCloud account when enabled; TapMinutes has no direct access to that content. |
| Audio described as broadly sent to servers | On-device transcription keeps audio processing on device; premium cloud transcription sends necessary audio; AI generation may send transcript text and style instructions after disclosure/consent. |
| Branding described only as Pro | Branding is included with Pro and may be separately offered when shown in the app; PDF export itself normally requires Pro. |
| No purchase availability caveat | Weekly/monthly/yearly Pro, trial, and one-time options are described as available only when shown in the app; no fixed prices are published. |
| Recovery described without gating | Backup, restore, and Recover Saved Recordings are labeled Pro. |

## 5. Compliance Checklist

- [x] Every feature is mapped to Basic, Pro, companion, or conditional one-time availability.
- [x] Basic daily, weekly, per-meeting, and shared import/recording limits are explicit.
- [x] Pro meeting length is described as longer or beyond Basic limits, not literally unlimited.
- [x] No fixed subscription prices are published.
- [x] Subscription and purchase availability is qualified by in-app/storefront availability.
- [x] Branding purchase does not imply that PDF export is independently unlocked.
- [x] On-device and cloud transcription are clearly distinguished.
- [x] Cloudflare proxy and OpenAI API processing are disclosed.
- [x] OpenAI API content training wording is preserved and scoped to the API policy.
- [x] No absolute “nothing leaves the device,” end-to-end encryption, certification, or compliance claim is made.
- [x] No unsupported codec list, DOCX, OCR, testimonial, customer logo, metric, award, or social integration is claimed.
- [x] Apple Watch is described only as a remote recording companion.
- [x] Semantic landmarks, heading order, skip links, visible focus styles, keyboard navigation, reduced-motion support, and descriptive screenshot alt text are included.
- [x] The comparison remains a semantic table and becomes readable stacked plan rows on small screens.
- [x] Material plan limitations appear in the main content, not hidden in footnotes.
- [x] Apple Standard EULA remains the Terms destination.

## 6. Owner Verification Before Publication

The product specification establishes that the app can offer weekly, monthly, and yearly subscriptions, a seven-day trial, Custom PDF Branding, and Custom Preset Pack. Their current App Store approval and storefront availability were not independently verified. The site therefore uses “when shown in the app,” “may offer,” and similar conditional wording. Confirm current in-app product availability before replacing those qualifications with definitive purchase language.
