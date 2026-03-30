<div align="center">

<img src="https://pablo.health/images/pablo-bear.jpg" alt="Mental Health Documentation work sucks. My human is going to fix it." width="480" />

# pablo-health

**AI-powered therapy documentation — built in the open.**

[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL%20v3-E8A849?style=flat-square&labelColor=3D2B1F)](https://github.com/pablo-health/pablo/blob/main/LICENSE)
[![HIPAA Compliant](https://img.shields.io/badge/HIPAA-Compliant-7A9E7E?style=flat-square&labelColor=3D2B1F)](https://pablo.health)
[![Platforms](https://img.shields.io/badge/Platforms-macOS%20%7C%20Windows-89B4C8?style=flat-square&labelColor=3D2B1F)](https://github.com/pablo-health/pablo-companion)
[![Self‑Host](https://img.shields.io/badge/Self--Host-GCP-B8A9C9?style=flat-square&labelColor=3D2B1F)](https://github.com/pablo-health/pablo)

*We build in the open because therapists deserve to verify what touches their sessions — not just trust a marketing page.*

</div>

---

## What is pablo.health?

[Pablo](https://pablo.health) is an AI-powered documentation assistant for therapists and prescribers in solo and small-group practice. It turns session recordings into SOAP notes — with additional note formats (DAP, BIRP) on the roadmap.

> **You review and approve every note. Nothing is filed automatically. Ever.**

Self-host on your own GCP account with one script, or let us handle infrastructure with [Pablo Solo](https://pablo.health).

---

## Open Source Repos

```
┌─────────────────────────────────────────────────────────┐
│  Pablo Companion (desktop)                              │
│  Click Start Session → records + launches video call    │
│  ┌───────────────────────────────┐                      │
│  │  AudioCaptureKit              │                      │
│  │  encrypted audio capture      │                      │
│  └──────────────┬────────────────┘                      │
│                 │ encrypted upload                       │
│                 ▼                                        │
│  ┌───────────────────────────────┐                      │
│  │  Pablo (backend + web app)    │                      │
│  │  AI SOAP note generation      │                      │
│  │  calendar · patient mgmt      │                      │
│  └───────────────────────────────┘                      │
│        your GCP  ·  or  ·  pablo.health                 │
└─────────────────────────────────────────────────────────┘
```

### [Pablo](https://github.com/pablo-health/pablo) &nbsp; — &nbsp; platform &amp; backend

The full web app and API. Next.js + FastAPI + Firestore, deployable to Cloud Run with a single setup script. Includes AI SOAP note generation, built-in calendar, patient management, and audit logging.

```bash
git clone https://github.com/pablo-health/pablo.git && cd pablo && ./setup-solo.sh
```

### [Pablo Companion](https://github.com/pablo-health/pablo-companion) &nbsp; — &nbsp; desktop app

Native macOS and Windows app that sits in the menu bar during the workday. Therapists see today's sessions, click **Start Session**, and Pablo automatically records and launches their video call (Zoom, Teams, or Google Meet). Monorepo: shared Rust core with SwiftUI (macOS) and WinUI 3 (Windows).

### [AudioCaptureKit](https://github.com/pablo-health/AudioCaptureKit) &nbsp; — &nbsp; audio capture library

Cross-platform HIPAA-compliant audio capture — the open layer beneath every Pablo session recording. macOS (Swift / CoreAudio) and Windows (Rust / WASAPI). Encrypted on-device from the first byte, zero PHI in logs.

---

## Why we build in the open

Healthcare AI has a verification problem. Every vendor claims HIPAA compliance. Every marketing page says your data is safe. You're expected to take their word for it.

We think that's wrong — especially when the data is therapy sessions.

- **Transparency earns trust.** Therapists and their patients deserve to know exactly how audio is captured, encrypted, and handled.
- **Security improves in the open.** Community review catches what private audits miss.
- **Clinicians shouldn't have to trust black boxes.** Read the code. Understand it. Then decide.

---

## Get Started

| | Self-Host | Managed (Pablo Solo) |
|---|---|---|
| **Hosting** | Your GCP account | pablo.health |
| **HIPAA** | You manage compliance | BAA included |
| **Price** | Free (AGPL-3.0) | From $14/mo |
| **Setup** | `./setup-solo.sh` | [Sign up](https://pablo.health) |

---

<div align="center">

Built by [Kurt Niemi](https://linkedin.com/in/kurtniemi) for therapists like his sister Kendra — PMHNP-BC, solo private practice.

[pablo.health](https://pablo.health) &nbsp;·&nbsp; [Sign up](https://pablo.health#signup) &nbsp;·&nbsp; [Self-host](https://github.com/pablo-health/pablo)

*Pablo's got it.*

</div>
