<div align="center">

<img src="https://pablo.health/images/pablo-bear.jpg" alt="Mental Health Documentation work sucks. My human is going to fix it." width="480" />

# pablo-health

**AI-powered therapy documentation — built in the open.**

[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL%20v3-E8A849?style=flat-square&labelColor=3D2B1F)](https://github.com/pablo-health/AudioCaptureKit/blob/main/LICENSE)
[![HIPAA Compliant](https://img.shields.io/badge/HIPAA-Compliant-7A9E7E?style=flat-square&labelColor=3D2B1F)](https://pablo.health)
[![Platforms](https://img.shields.io/badge/Platforms-macOS%20%7C%20Windows-89B4C8?style=flat-square&labelColor=3D2B1F)](https://github.com/pablo-health/AudioCaptureKit)

*We build in the open because therapists deserve to verify what touches their sessions — not just trust a marketing page.*

</div>

---

## What is pablo.health?

[Pablo](https://pablo.health) is an AI-powered documentation assistant for therapists and prescribers in solo and small-group practice. It turns session recordings into clinical notes — SOAP, DAP, BIRP — then a second NLP verification layer confirms every generated claim is grounded in what was actually said.

> **You review and approve every note. Nothing is filed automatically. Ever.**

The clinical AI space has a transparency problem. We're fixing that — one open source component at a time.

---

## Open Source

### 🎙️ [AudioCaptureKit](https://github.com/pablo-health/AudioCaptureKit)

> *HIPAA-compliant audio capture — the open layer beneath Pablo's session recording.*

AudioCaptureKit is the cross-platform library that every Pablo session runs on. It handles secure microphone capture, end-to-end encryption, and prepares audio for HIPAA-compliant cloud processing — on macOS and Windows.

Before you trust any AI with a therapy session, you should be able to read how your audio is captured. So we open sourced it.

```
Session  →  AudioCaptureKit  →  encrypted upload  →  Pablo AI  →  clinical note
              (you can read                            (HIPAA-eligible GCP)
               this part)
```

**What it does:**
- Cross-platform: macOS (Swift / CoreAudio) and Windows (Rust / WASAPI)
- Encrypted on-device from the first byte
- Designed for HIPAA-eligible environments
- Zero PHI in logs, encrypted in transit

[→ View AudioCaptureKit](https://github.com/pablo-health/AudioCaptureKit)

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

<div align="center">

Built by [Kurt Niemi](https://linkedin.com/in/kurtniemi) for therapists like his sister Kendra — PMHNP-BC, solo private practice.

[pablo.health](https://pablo.health) &nbsp;·&nbsp; [Get early access](https://pablo.health#signup)

*Pablo's got it.*

</div>
