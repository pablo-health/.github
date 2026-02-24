<div align="center">

<img src="https://pablo-health.github.io/images/pablo-tie.webp" alt="Pablo Bear" width="120" />

# pablo-health

**AI-powered therapy documentation — built in the open.**

[![License: MIT](https://img.shields.io/badge/License-MIT-E8A849?style=flat-square&labelColor=3D2B1F)](https://github.com/pablo-health/AudioCaptureKit/blob/main/LICENSE)
[![HIPAA Compliant](https://img.shields.io/badge/HIPAA-Compliant-7A9E7E?style=flat-square&labelColor=3D2B1F)](https://pablo-health.github.io)
[![Platform: iOS](https://img.shields.io/badge/Platform-iOS-89B4C8?style=flat-square&labelColor=3D2B1F&logo=apple&logoColor=white)](https://github.com/pablo-health/AudioCaptureKit)
[![Made by Kurt Niemi](https://img.shields.io/badge/Made%20by-Kurt%20Niemi-3D2B1F?style=flat-square)](https://linkedin.com/in/kurtniemi)

*We build in the open because therapists deserve to verify what touches their sessions — not just trust a marketing page.*

</div>

---

## What is pablo.health?

[Pablo](https://pablo-health.github.io) is an AI-powered documentation assistant for therapists and prescribers in solo and small-group practice. It turns session recordings into clinical notes — SOAP, DAP, BIRP — then a second NLP verification layer confirms every generated claim is grounded in what was actually said.

> **You review and approve every note. Nothing is filed automatically. Ever.**

The clinical AI space has a transparency problem. We're fixing that — one open source component at a time.

---

## Open Source

### 🎙️ [AudioCaptureKit](https://github.com/pablo-health/AudioCaptureKit)

> *HIPAA-compliant audio capture for iOS — the open layer beneath Pablo's session recording.*

AudioCaptureKit is the foundation that every Pablo session runs on. It handles secure microphone capture, end-to-end encryption, and prepares audio for HIPAA-compliant cloud processing. Before you trust any AI with a therapy session, you should be able to read how your audio is captured.

So we open sourced it.

```
Patient session  →  AudioCaptureKit  →  encrypted upload  →  Pablo AI  →  clinical note
                     (you can read                              (cloud,
                      this part)                                HIPAA-eligible GCP)
```

**What it does:**
- Secure on-device audio capture with hardware-level encryption
- Designed from the ground up for HIPAA-eligible environments
- Zero PHI in logs, encrypted in transit from the first byte
- No audio leaves the device unencrypted

[→ View AudioCaptureKit](https://github.com/pablo-health/AudioCaptureKit)

---

### 🌐 [pablo-health.github.io](https://github.com/pablo-health/pablo-health.github.io)

> *The pablo.health landing page — static HTML/CSS, no build step, deployed via GitHub Pages.*

The public-facing landing page. Single-file, readable HTML. No framework overhead.

**Stack:** Vanilla HTML · CSS custom properties · Formspree · GitHub Pages

[→ View repo](https://github.com/pablo-health/pablo-health.github.io) · [→ Live site](https://pablo-health.github.io)

---

## Why we build in the open

Healthcare AI has a verification problem. Every vendor claims HIPAA compliance. Every marketing page says your data is safe. You're expected to take their word for it.

We think that's wrong — especially when the data is therapy sessions.

AudioCaptureKit is open source because:
- **Transparency earns trust.** Therapists and their patients deserve to know exactly how audio is captured, encrypted, and handled.
- **Security improves in the open.** Community review catches what private audits miss.
- **Clinicians shouldn't have to trust black boxes.** Read the code. Understand it. Then decide.

More of Pablo's infrastructure will open over time. This is the start.

---

## Contributing

AudioCaptureKit welcomes contributions — especially from developers with experience in:
- iOS audio session management (AVFoundation, AudioToolbox)
- On-device encryption patterns
- HIPAA-eligible architecture on Google Cloud Platform

See [`CONTRIBUTING.md`](https://github.com/pablo-health/AudioCaptureKit/blob/main/CONTRIBUTING.md) in the AudioCaptureKit repo.

---

<div align="center">

**pablo.health** &nbsp;·&nbsp; *Paperwork Automation for Behavioral Logging & Outcomes*

Built by [Kurt Niemi](https://linkedin.com/in/kurtniemi) — bootstrapped, no VC, no data monetization.

[pablo-health.github.io](https://pablo-health.github.io) &nbsp;·&nbsp; [Get early access](https://pablo-health.github.io#signup)

*Pablo's got it.*

</div>
