# ZenithDx Website

> **The First 100% On-Device AI Diagnostic Copilot for Emergency Departments**  
> Delivering real-time fusion of DICOM imaging, NLP clinical notes, and patient history. Processed entirely within hospital LANs with zero cloud data egress.

---

## 🏥 About ZenithDx

ZenithDx is a clinical precision medicine AI platform engineered specifically for Emergency Departments and acute care settings:
- **100% On-Device Execution**: Operates as an air-gapped on-premise hardware appliance with zero cloud egress.
- **Multimodal AI Fusion**: Synchronizes DICOM radiological imaging, HL7 FHIR clinical notes, and longitudinal patient records in real-time (< 2.8s inference).
- **Clinically Validated**: Tested across 14,200+ acute cases with 121 frontline emergency physicians (96.28% Diagnostic Accuracy, -41.8% triage errors).
- **Statutory Compliance**: Engineered for EU MDR Class IIa Rule 11, EU AI Act High-Risk Article 14 oversight, and GDPR Article 25 privacy by design.

---

## 🚀 Technology Stack

- **Frontend**: HTML5, Vanilla JavaScript, Tailwind CSS (Utility Framework)
- **Icons & Typography**: Google Material Symbols, Inter, Roboto, Outfit, Playfair Display
- **Deployment**: Vercel Serverless CDN / Static Hosting
- **Interoperability**: HL7 FHIR R4, DICOMweb, PACS/RIS native connectors

---

## 📦 Deployment on Vercel

This repository is optimized for one-click deployment on [Vercel](https://vercel.com/):

```bash
# Clone the repository
git clone https://github.com/FilippeZ/zenithdx-website.git

# Navigate to workspace
cd zenithdx-website

# Deploy via Vercel CLI
vercel
```

Or connect this GitHub repository directly to Vercel via the Vercel Dashboard for automated CI/CD deployments on `main`.

---

© 2026 ZenithDx. All rights reserved. Medical Device Software (SaMD) investigational prototype under regulatory compilation.
