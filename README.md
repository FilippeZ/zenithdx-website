# ZenithDx Digital Health Platform

[![Status](https://img.shields.io/badge/Regulatory%20Status-MDR%20Class%20IIa%20Compilation-blue.svg)](#statutory-compliance--regulatory-framework)
[![Security](https://img.shields.io/badge/Data%20Sovereignty-100%25%20Air--Gapped%20LAN-emerald.svg)](#air-gapped-security--data-sovereignty)
[![Clinical Validation](https://img.shields.io/badge/Trial%20Cohort-121%20Physicians%20•%2014%2C200%2B%20Cases-cyan.svg)](#4-validation--121-clinicians-page-page-research)
[![License](https://img.shields.io/badge/Intellectual%20Property-Proprietary%20Clinical%20SaMD-slate.svg)](#intellectual-property--governance)

> **The First 100% On-Device AI Diagnostic Copilot for Emergency Departments**  
> Delivering real-time, zero-cloud-egress multimodal fusion of DICOM radiological imaging, HL7 FHIR clinical notes, and longitudinal patient histories directly within hospital Local Area Networks (LAN).

---

## 📋 Table of Contents
1. [Executive Summary](#executive-summary)
2. [Architecture & Technology Stack](#architecture--technology-stack)
3. [Analytical Breakdown of Pages & Modules](#analytical-breakdown-of-pages--modules)
   - [0. Fullscreen Cinematic Brand Assembly Landing](#0-fullscreen-cinematic-brand-assembly-landing)
   - [1. Home Page (`#page-home`)](#1-home-page-page-home)
   - [2. Solutions & Value Analysis Page (`#page-solutions`)](#2-solutions--value-analysis-page-page-solutions)
   - [3. The Platform & Hardware Moat Page (`#page-tech`)](#3-the-platform--hardware-moat-page-page-tech)
   - [4. Validation & 121 Clinicians Page (`#page-research`)](#4-validation--121-clinicians-page-page-research)
   - [5. About Us, Team & Governance Page (`#page-investors`)](#5-about-us-team--governance-page-page-investors)
   - [6. Book a Clinical Demo & Intake Page (`#page-demo`)](#6-book-a-clinical-demo--intake-page-page-demo)
4. [Enterprise Lead Dispatch Engine](#enterprise-lead-dispatch-engine)
5. [Internationalization Engine (Bilingual EN / EL)](#internationalization-engine-bilingual-en--el)
6. [Repository Structure & Asset Mapping](#repository-structure--asset-mapping)
7. [Vercel Deployment & Production Optimization](#vercel-deployment--production-optimization)
8. [Statutory Compliance & Regulatory Framework](#statutory-compliance--regulatory-framework)

---

## 🏥 Executive Summary

ZenithDx addresses the acute care crisis facing modern emergency medicine: **cognitive overload, severe physician burnout, and delayed differential diagnosis in crowded Emergency Departments (ED)**. 

Unlike conventional healthcare AI offerings that require off-premise streaming of Protected Health Information (PHI) to third-party public cloud endpoints, ZenithDx operates as an **autonomous, 100% air-gapped on-premise hardware appliance**.

### Core Technical Pillars:
- **Zero Cloud Egress**: Strict compliance with GDPR Article 25 (Data Protection by Design and by Default) and statutory hospital data sovereignty.
- **Ultra-Low Latency (< 2.8s)**: Real-time inference executed on local Tensor Core accelerators without external API roundtrips.
- **Multimodal Clinical Fusion**: Simultaneous evaluation of radiological DICOM series, unstructured physician notes, vital telemetry, and EHR timeline records.
- **Demonstrated Clinical Impact**: 96.28% diagnostic accuracy across 14,200+ multi-center international cases, yielding a -41.8% reduction in critical diagnostic triage omissions.

---

## 💻 Architecture & Technology Stack

The web platform is built for fast initial render times, responsive layouts across devices, and compliance with modern medical web aesthetics.

```
┌─────────────────────────────────────────────────────────────┐
│                       ZenithDx Web App                      │
├──────────────────────────────┬──────────────────────────────┤
│ Core Engine                  │ Single Page Architecture     │
│ Styling & Design Tokens      │ Tailwind CSS & Custom Themes │
│ Typography                   │ Inter, Playfair Display      │
│ Multimedia                   │ HTML5 Video + Media Fragment │
│ Data Transmission            │ Dual AJAX & FormSubmit Engine│
│ Hosting & Edge CDN           │ Vercel Serverless Edge       │
└──────────────────────────────┴──────────────────────────────┘
```

- **Clean SPA Architecture**: Zero bloated framework overhead; built on semantic HTML5 and vanilla JavaScript for sub-second first contentful paint (FCP).
- **Design Tokens & Palette**:
  - Medical Cyan: `#0891b2` / `#06b6d4`
  - Surgical Teal: `#0d9488` / `#14b8a6`
  - High-Contrast Navy/Slate: `#0f172a` / `#1e293b`
  - Muted Health Diagnostics Pastels & Organic Contour SVGs
- **Hardware-Accelerated Fluid Animations**: Pure CSS keyframes with `cubic-bezier(0.16, 1, 0.3, 1)` spring easing curves.

---

## 🔍 Analytical Breakdown of Pages & Modules

### 0. Fullscreen Cinematic Brand Assembly Landing
- **Purpose**: Establishes high-fidelity brand authority upon initial visitor arrival through a dynamic 3D geometric logo data assembly.
- **Implementation**:
  - **Full Viewport Canvas**: Seamless pure-white background integration (`bg-white`, `object-contain md:object-cover`) spanning 100vw/100vh.
  - **Blur Artifact Skip**: Utilizes `#t=1.0` media fragment indexing and JS sync (`video.currentTime = 1.05s`) to completely bypass the initial 0.0s compression blur.
  - **Unmuted Sovereign Sound Engine**: Direct audio playback integration (`video.muted = false; video.volume = 1.0;`) with global interaction listeners ensuring seamless unmute across strict browser autoplay policies.
  - **Enter the Platform Gateway**: Bottom-right floating action button that terminates the overlay in a 450ms fade and coordinates the staggered entrance animations of the hero elements.

---

### 1. Home Page (`#page-home`)
The core institutional presentation of ZenithDx's value proposition:

1. **Hero Display & Cascading Metric Deck**:
   - **Dynamic Headline**: *"The First 100% On-Device AI Diagnostic Copilot for Emergency Departments"*.
   - **Sub-Hero Thesis**: Explaining the fusion of DICOM imaging, NLP clinical notes, and patient history within hospital LANs.
   - **Action CTAs**: Instant routing to Book Clinical Demo (`#demo`) and 121 Clinician Validation Study (`#research`).
   - **4 Telemetry Metric Cards** (Triggered with staggered pop-in animation on platform entry):
     1. **`96.28%`**: Diagnostic accuracy across 14,200+ international acute care validation cases.
     2. **`N=121`**: Frontline emergency physicians validating the copilot across hospital networks.
     3. **`-41.8%`**: Triage error and diagnostic omission reduction rate.
     4. **`< 2.8s`**: Local LAN inference roundtrip time with zero cloud latency.
2. **Interactive Clinical Milestone Roadmap**:
   - Visual stages from initial validation to CE Mark Class IIa and pan-European multi-center rollout.
3. **Multimodal Technical Architecture Pipeline**:
   - Step-by-step clinical ingestion: Patient Bedside Intake → DICOM/EHR Edge Parsing → Local Neural Co-Pilot Processing → Physician Decision Validation.
4. **Interactive Hospital ROI & Economic Payback Calculator**:
   - Real-time client-side financial model simulating annual ER patient volume (10k to 120k) and baseline misdiagnosis rates.
   - Calculates annual malpractice avoidance savings, diagnostic DRG optimization, and capital payback periods (~4.6 months).
5. **Clinical Testimonials Spotlight**:
   - Multi-tab verified clinical feedback from Chief Medical Officers, Emergency Department Heads, and Academic Radiologists.

---

### 2. Solutions & Value Analysis Page (`#page-solutions`)
Tailored directly for Value Analysis Committees (VAC), Chief Financial Officers (CFO), and Chief Information Officers (CIO):

1. **3-Tier Commercial Deployment Matrix**:
   - **RUO Shadow Tier**: Zero-risk, read-only passive evaluation running in background shadow mode.
   - **Clinical Production Appliance**: Active emergency department bedside deployment with native PACS/EHR bidirectional hooks.
   - **Enterprise Sovereign Network**: Multi-hospital federated deployment across regional health authorities.
2. **Executive Objection Dossiers (Pastel Contour Cards)**:
   - **CFO • Budget Concerns**: Demonstrating 4.6-month capital payback, 412% 3-year net ROI, and €0 marginal recurring cloud API token fees.
   - **CIO • IT Staff Bandwidth**: Demonstrating 1-week plug-and-play autonomous appliance deployment with zero firewall rule modifications.
   - **CMO • Clinical Safety & MDR**: Statutory compliance overview covering MDR Class IIa Rule 11 and Article 14 human-in-the-loop clinical oversight.
   - **DPO • GDPR Data Protection**: Complete LAN air-gapped isolation with SHA-256 tamper-proof write-once audit logs.
3. **Master Hospital Procurement Decision Package**:
   - Central procurement hub enabling hospital committees to request the consolidated 14.8 MB dossier kit (.ZIP) under mutual NDA.

---

### 3. The Platform & Hardware Moat Page (`#page-tech`)
Detailed technical breakdown for hospital IT architects, biomedical engineers, and CISO evaluation teams:

1. **Air-Gapped Hardware Appliance Specifications**:
   - High-throughput NVIDIA Tensor Core inference engine engineered for 24/7 continuous emergency department operation.
   - Dual redundant power supplies, tamper-evident physical chassis, and hardware-level cryptographic key stores.
2. **On-Device Multimodal Fusion Engine**:
   - Ingestion protocols: HL7 v2.x, HL7 FHIR R4, DICOMweb, and native PACS modalities (CT, X-ray, Ultrasound).
   - Local Vector RAG & Knowledge Graph mapping longitudinal patient history without external egress.
3. **Explainable AI (XAI) & Clinical Transparency**:
   - Automated anatomical heatmaps, attention weight overlays, and verbatim cross-references to medical literature and hospital guidelines.

---

### 4. Validation & 121 Clinicians Page (`#page-research`)
The scientific foundation backing ZenithDx's software:

1. **Multi-Center Clinical Trial Methodology**:
   - Comprehensive study protocol involving 121 practicing physicians across Greek public hospital networks and international validation cohorts.
2. **Diagnostic Accuracy Head-to-Head Comparison**:
   - Benchmarking ZenithDx's specialized clinical diagnostic engine against generalist frontier models (OpenAI ChatGPT-4o, Anthropic Claude 3.5 Sonnet, Google Gemini 1.5 Pro, xAI Grok, DeepSeek).
   - Highlighting critical error rates and hallucination frequencies of generalist models in emergency acute care vs ZenithDx's validated clinical engine.
3. **Pathology Distribution & Cohort Segmentation**:
   - Detailed coverage breakdown including pulmonary embolism, acute pneumothorax, aortic dissection, ischemic stroke, and acute abdomen pathologies.

---

### 5. About Us, Team & Governance Page (`#page-investors`)
Institutional background and corporate governance:

1. **University Spin-Off Heritage**:
   - Born out of the Computer Engineering and Informatics Department (CEID) at the University of Patras.
   - Certified members of Elevate Greece and NVIDIA Inception Healthcare Accelerator.
2. **Leadership & Medical Advisory Board**:
   - Founded by Filippos Zygouris, supported by clinical specialists in emergency medicine, radiology, and medical software regulation.
3. **Regulatory Milestones**:
   - Structured timeline towards MDR Class IIa CE Mark statutory certification and pan-European commercial availability.

---

### 6. Book a Clinical Demo & Intake Page (`#page-demo`)
The primary institutional engagement and consultation scheduling gateway:

1. **30-Minute Consultation High-Impact Walkthrough**:
   - **`[ 01 ] WORKFLOW MAPPING`**: Evaluation of hospital ER bottlenecks and seamless PACS/EHR integration pathways.
   - **`[ 02 ] CLINICAL EVIDENCE REVIEW`**: Real-world trial walkthrough (96.28% diagnostic accuracy, -41.8% omissions).
   - **`[ 03 ] PILOT STRUCTURING`**: Step-by-step design of a zero-friction 30-day Shadow Mode deployment operating with zero firewall changes.
2. **Specialized Consultation Focus (Executive Briefing)**:
   - **Operational Alignment**: Tailoring algorithmic thresholds to departmental clinical protocols.
   - **Real-World Best Practices**: Practical insights from acute emergency implementations.
   - **Acute Pathology Triage**: Demonstrating automated lung segmentation and acute triage algorithms.
   - Direct Action Link: `👉 [Schedule Your Consultation Today] →` with smooth auto-scroll to the intake form.
3. **Lead Qualification Form**:
   - Captures first name, last name, hospital network, professional email, role focus, country, target pilot date, and message.
   - Direct connection to hospital deployment teams via asynchronous dispatch.

---

## ✉️ Enterprise Lead Dispatch Engine

All interactive forms on the portal are integrated to dispatch inquiries to:
**`zenithdxcopilot@gmail.com`**

### Submission Mechanism:
- **Dual-Layer Delivery**:
  1. **Asynchronous AJAX Dispatch**: Utilizes FormSubmit's REST API endpoint with `FormData` payloads, ensuring no disruptive page refreshes and providing instantaneous on-page confirmation.
  2. **Native HTML POST Fallback**: Standard `action="https://formsubmit.co/zenithdxcopilot@gmail.com"` ensures submissions succeed even if client-side JavaScript is restricted by strict hospital browser group policies.
- **Form Endpoints**:
  - **Clinical Demo Intake Form** (`#demo-intake-form`)
  - **Shadow-Mode Pilot Protocol Modal** (`#pilot-modal-form`)
  - **CFO Executive ROI Dossier Form** (`#cfo-report-form`)
  - **Portal Contact Inquiry Form** (`#cta-contact-form`)
  - **VAC Master Procurement Dossier Request** (`window.requestVACKit`)

---

## 🌐 Internationalization Engine (Bilingual EN / EL)

The platform features seamless client-side switching between **English (EN)** and **Greek (EL)**:
- Controlled via `#lang-btn-en` and `#lang-btn-el` in the global header.
- Persistent language state stored in `localStorage.getItem('zenith_lang')`.
- Zero page reload required: elements with `.lang-en` and `.lang-el` toggle dynamically with appropriate typography scaling.

---

## 📂 Repository Structure & Asset Mapping

```
ZENITHWEB/
├── index.html                   # Primary Single-Page Application (All views & modules)
├── landing.html                 # Standalone video landing showcase
├── vercel.json                  # Vercel SPA rewrites & security header configuration
├── .gitignore                   # Excludes scratch files, python scripts, and temp assets
├── README.md                    # Analytical documentation
│
├── assets/credentials/          # Institutional logos (Univ of Patras, Elevate Greece, NVIDIA, EU)
├── images/                      # High-resolution architectural schematics (RAG, EHR, Vision)
├── llms/                        # Benchmark comparative model badges
├── pipeline/                    # Clinical diagnostic workflow icons & schematics
├── profiles/                    # Clinician and patient UI illustration elements
├── standards/                   # Regulatory standards badges (GDPR, MDR, IEC 62304, HIPAA, ISO)
├── steps/                       # Step-by-step methodology graphics
├── testimonials/                # Verified physician portraits
│
├── ZenithDX_logo_data_assembly_anim.mp4  # 3D Brand assembly animation video (1080p)
├── frame_1.0s.jpg               # Video poster image (skips initial compression blur)
├── video_preview_9.5s.jpg       # Secondary preview snapshot
├── logo.png                     # Official ZenithDx brand emblem & logotype
└── image.png                    # Clinical diagnostic workstation rendering
```

---

## 🚀 Vercel Deployment & Production Optimization

The repository includes a production-ready `vercel.json` configuration file:

```json
{
  "version": 2,
  "cleanUrls": true,
  "rewrites": [
    { "source": "/(.*)", "destination": "/index.html" }
  ]
}
```

### Deploying to Vercel:
1. Navigate to [Vercel Dashboard](https://vercel.com/new).
2. Connect your GitHub account and import **`FilippeZ/zenithdx-website`**.
3. Click **Deploy**. Vercel will automatically configure the static output directory and deploy across its global edge network.

---

## ⚖️ Statutory Compliance & Regulatory Framework

- **EU Medical Device Regulation (EU MDR 2017/745)**: Software as a Medical Device (SaMD) currently compiled under Rule 11 classification (Class IIa).
- **EU Artificial Intelligence Act**: Designed for high-risk Article 14 statutory oversight with mandatory human-in-the-loop clinical governance.
- **GDPR (Regulation EU 2016/679)**: Article 25 compliant. All patient health identifiers (PHI) and DICOM pixels remain strictly within the hospital's local network perimeter.
- **Quality Management Standards**: ISO 13485 (Medical Devices QMS), IEC 62304 (Medical Device Software Life-Cycle), and ISO 14971 (Risk Management for Medical Devices).

---

© 2026 ZenithDx. All rights reserved. Investigational medical device software prototype.
