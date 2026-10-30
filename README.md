# RationSetu (राशन सेतु) 🌾
### Smart PDS Access & Fast-Pass System — Design Thinking Prototype

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Prototype: HTML5/JS](https://img.shields.io/badge/Prototype-HTML5%20%2F%20TailwindCSS-blue.svg)](index.html)
[![PDS: NFSA & ONORC](https://img.shields.io/badge/Scheme-NFSA%20%7C%20ONORC-green.svg)](https://nfsa.gov.in)

> **RationSetu** is an inclusive, human-centered Public Distribution System (PDS) prototype designed using the **Design Thinking Methodology**. It transforms the ration collection experience for over 800 million citizens under the National Food Security Act (NFSA) and Antyodaya Anna Yojana (AAY) by eliminating long queues, preventing wage loss, and bridging the digital divide.

---

## 📌 The 3 Core Design Thinking Pillars

### 1. User Interaction Point (Touchpoint Architecture)
* **When & Where:** **7:30 AM at home / construction site (Pre-commute touchpoint)** before leaving for daily wage work.
* **Why it matters:** Traditionally, beneficiaries interact with the PDS only upon physically arriving at the Fair Price Shop (FPS), often finding empty stocks or 3-hour queues after losing a day's earnings (₹500). Moving the touchpoint upstream empowers workers with schedule control and protects their livelihoods.

### 2. The Single Element Addressing User Difficulty
* **The Hero Element:** The **Guaranteed Stock Quota & Fast-Pass Token Card** (`#heroSingleElementCard`).
* **Why it works:**
  - **Eliminates Stock Uncertainty:** Displays real-time grain inventory (Rice, Wheat, Coarse Grains, Sugar) verified against the State ERP.
  - **24-Hour Stock Reservation:** When a slot is locked, 30 kg of grain is earmarked in the dealer's e-PoS database, stopping black-market diversion.
  - **Offline Cryptographic QR Pass:** Generates a tamper-proof ECDSA token (`#TK-482`) that functions even when mobile networks are completely offline.

### 3. What We Do Not Yet Know Will Work (The Critical Unknown)
* **The Core Hypothesis:** *"Will Fair Price Shop (FPS) dealers reliably honor scheduled digital time-slots when pressured by an aggressive, non-digital crowd waiting physically outside in the heat?"*
* **De-Risking Mechanisms Built Into Prototype:**
  - **70/30 Dynamic Queue Balancing Protocol:** Alternates 1 digital token holder for every 2 physical walk-in beneficiaries.
  - **Multi-Tier Identity Fallback:** If biometric fingerprint sensors fail on worn laborer fingers, the system automatically falls back to Iris scan, SMS OTP, or family co-beneficiary approval.
  - **Zero-Internet Local Verification:** Offline QR verification directly on e-PoS machines without cellular data.

---

## ✨ Key Features & Capabilities

- **📍 5 Nearby Fair Price Shops (ONORC Portability):**
  1. *Shop #402: Sharma Fair Price Store* (1.2 km, 14 min walk, Assigned FPS)
  2. *Shop #108: Metro Depot PDS Center* (600 m, 7 min walk, Fastest Walk)
  3. *Shop #330: Mahila Samiti SHG Kendra* (850 m, 10 min walk, All-Women SHG)
  4. *Shop #215: Jan Aahar Kendra (Civil Hospital)* (1.7 km, 20 min walk, Transit Hub)
  5. *Shop #512: Old Railway Mandi Cooperative* (2.3 km, 28 min walk, Wholesale Hub)
- **🗺️ Interactive Vector Map:** Pure SVG district map with user GPS marker, shop pins, and live turn-by-turn walking route polyline.
- **💬 Offline SMS Booking for Keypad Feature Phones:** Syntax `RATION <CardNo> BOOK <ShopNo> <Slot>` sent to `56070` for citizens without smartphones.
- **📞 24x7 Government Helpline & Grievance Email:**
  - National Toll-Free: `1967` (24x7)
  - State Consumer Helpdesk: `1800-180-2087` (8 AM – 8 PM)
  - DFSO Inspector Direct: `+91 94120 48210`
  - Official Email: `grievance.pds@nic.in`
- **🖥️ Govt. e-PoS Dealer Terminal Simulator:** Interactive dual-view terminal showing real-time scanning, biometric verification, and digital vs. walk-in quota dispatch.
- **👥 3-Member Presentation Guide:** Built-in modal providing dedicated scripts, screen actions, and talking points for 3 students to present to teachers or juries.

---

## 👥 3-Member Presentation Roles

| Member | Focus | Key Action in App | Core Message |
| :--- | :--- | :--- | :--- |
| **Member 1** | **Problem & Empathy** | Switch *Old PDS vs RationSetu*, open *Nearby 5 Shops & Map*, show *Helpline 1967*. | *"Ramesh loses ₹500 every month waiting in 3-hour lines. We move the interaction to 7:30 AM before he leaves home."* |
| **Member 2** | **Solution & Feature Phone Access** | Select slot, lock quota, generate *#TK-482 QR*, open *Offline SMS Booking (56070)*. | *"Our single hero element reserves quota for 24 hours. Offline SMS ensures even families without smartphones are included."* |
| **Member 3** | **Critical Unknown & De-Risking** | Run *Test Friction (Scenario A)*, *Test Biometric Fallback (Scenario B)*, switch to *Govt. e-PoS Terminal*. | *"We stress-tested the dealer crowd bottleneck with a 70/30 algorithm and multi-tier biometric fallback for worn fingers."* |

---

## 🚀 How to Run the Prototype

### Option 1: Open Directly in Browser
Simply double-click [`index.html`](index.html) or open it with Google Chrome, Firefox, Safari, or Microsoft Edge.

### Option 2: Run via Local HTTP Server
```bash
# In the project root directory:
python3 -m http.server 8080
```
Then navigate to: **`http://localhost:8080`**

---

## 📁 Project Structure

```text
.
├── index.html               # Complete, self-contained interactive web prototype
├── DESIGN_THINKING_DOC.md   # Comprehensive Design Thinking specification document
└── README.md                # Project overview, methodology & presentation guide
```

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).
