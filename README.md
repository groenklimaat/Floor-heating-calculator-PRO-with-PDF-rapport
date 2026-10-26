# 🌡️ Floor Heating Calculator PRO

A professional, multi-language web tool for calculating **underfloor heating (hydronic floor heating)** per circuit. It computes heat output, flow rate, pressure drop, and pump advice based on supply/return temperatures.

> **Key feature:** The exported PDF report is designed to serve as a **substantiated technical document** (stavingstuk / bewijsstuk) for installers, engineers, and project documentation.

---

## 📋 Table of Contents
- [Features](#-features)
- [Live Demo / Usage](#-live-demo--usage)
- [The PDF Report as a Substantiating Document](#-the-pdf-report-as-a-substantiating-document)
- [Supported Languages](#-supported-languages)
- [Technical Details](#-technical-details)
- [Installation](#-installation)
- [How to Use](#-how-to-use)
- [Calculation Model](#-calculation-model)
- [License](#-license)

---

## ✨ Features

- **Per-circuit calculation:** Add unlimited heating circuits, each with its own parameters.
- **Real-time results:** Heat output (W/m²), loop power (W), flow rate (l/min), pressure drop (kPa), pump head (mH₂O), and flow velocity (m/s).
- **Intelligent advice:** Automatic pump recommendations based on pressure drop and pipe diameter.
- **Multi-language UI:** 8 languages, switchable on the fly, remembered via `localStorage`.
- **Professional PDF export:** Landscape A4 report, print-ready, with all circuit data and totals.
- **Responsive design:** Works on desktop, tablet, and mobile.
- **SVG icons:** Crisp, scalable, no external dependencies.

---

## 🚀 Live Demo / Usage

Open `index.html` (or `Floor Heating Calculator PRO.html`) directly in any modern browser. No build step, no server required.

---

## 📄 The PDF Report as a Substantiating Document

The exported PDF is **not just a summary** — it is structured to function as a **technical substantiating document (bewijsstuk / stavingstuk)** in English and other languages. It can be used for:

- **Installation handover files** (opleverdossier)
- **Project documentation** for architects and HVAC engineers
- **Warranty records** and service documentation
- **Client reporting** and quotation support
- **Compliance evidence** for building regulations (e.g., EN 1264 context)

### What the PDF contains:
- Supply and return temperatures per circuit
- Center-to-center distance (spacing)
- Pipe loop length and outer diameter
- Average water temperature
- Heat output (W/m²) and total loop power (W)
- Flow rate (l/min) and pressure drop (kPa)
- Pump head (mH₂O) and flow velocity (m/s)
- Automatic advice per circuit
- **Total overview:** number of circuits, total power (W), total flow (l/min)

> ⚠️ **Note:** This tool provides engineering estimates based on standard hydronic formulas. For critical installations, always have results verified by a certified HVAC engineer.

---

## 🌍 Supported Languages

| Code | Language   | Flag |
|------|------------|------|
| `nl` | Dutch      | 🇳🇱   |
| `en` | English    | 🇬🇧   |
| `de` | German     | 🇩🇪   |
| `fr` | French     | 🇫🇷   |
| `es` | Spanish    | 🇪🇸   |
| `it` | Italian    | 🇮🇹   |
| `pl` | Polish     | 🇵🇱   |
| `zh` | Chinese    | 🇨🇳   |

The selected language is saved in `localStorage` and also determines the PDF filename (e.g., `underfloor_heating_35_30_report.pdf`).

---

## 🔧 Technical Details

- **Pure HTML/CSS/JavaScript** — no framework, no build tools.
- **PDF generation:** [html2pdf.js](https://github.com/eKoopmans/html2pdf.js) (bundled via CDN).
- **Icons:** Inline SVG sprite (scalable, no external files).
- **No backend:** All calculations run client-side. No data leaves the browser.
- **Browser support:** Modern evergreen browsers (Chrome, Edge, Firefox, Safari).

---

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/floor-heating-calculator-pro.git
