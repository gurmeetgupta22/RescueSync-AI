# 🚨 RescueSync AI
### AI-Powered Road Safety & Emergency Response System

> *"Accidents may happen in seconds, but intelligent systems can save lives in those very seconds."*

---

## 📌 Overview

**RescueSync AI** is a hackathon project that proposes an edge AI chipset embedded directly into vehicles to address India's catastrophic road safety crisis. The system provides real-time hazard detection, automatic accident response, and continuous driver health monitoring — all without requiring an internet connection for core safety features.

This repository contains the **frontend-only website** built to present the project, featuring a fully interactive UI with embedded PPT slides, animated data visualizations, and a futuristic dark design inspired by the project's chalkboard presentation theme.

---

## 🌐 Live Website

Open `index.html` directly in any modern browser — no server or build step required.

```
rescuesync-ai/
└── index.html   ← Open this file
```

---

## 🎯 The Problem

India records one of the highest numbers of road accidents globally:

| Metric | Figure |
|---|---|
| Annual road deaths | 1,50,000+ |
| Accidents per year | 4.7 Million |
| Avg. urban emergency response | 15–20 minutes |
| Avg. rural emergency response | 45+ minutes |
| Hazard-related fatal accidents | ~35% of all fatalities |

**Root causes addressed by RescueSync AI:**
- Poor road conditions (potholes, open drains, construction zones)
- Delayed emergency response — the "golden hour" wasted
- Lack of real-time hazard alerts for drivers
- Absence of automated accident detection systems
- No driver health monitoring for fatigue or medical events

---

## 💡 Inspiration

Both real-life incidents that inspired this project occurred in **Delhi**:

1. **A car driver died** after his vehicle fell into an uncovered sewer on a poorly lit road
2. **A biker lost his life** after falling into an unmarked open pothole during night hours

These were preventable. RescueSync AI is designed to make sure they don't happen again.

---

## 🧠 The Solution — RescueSync AI Chipset

An **edge-AI system** embedded directly into vehicles with the following pipeline:

```
Vehicle Platform
      ↓
Sensor Array (LiDAR + Camera + IMU + Biometric)
      ↓
RescueSync AI Chip  ←— Core on-device inference (<50ms)
      ↓
Alert System (Haptic + Audio + Visual)
      ↓
Emergency Response (Auto SOS + GPS dispatch)
```

**Key design decisions:**
- All AI inference runs **on-device** — no cloud latency for safety-critical decisions
- **Multi-sensor fusion** for accuracy in all weather/lighting conditions
- **2W power consumption** — compatible with two-wheelers via the 12V vehicle system
- **IP67 + MIL-STD-810** target for India's extreme conditions

---

## ⚙️ Core Features

### 1. 🔍 AI Hazard Detection
- Scans roads **200m ahead** using computer vision + LiDAR
- Detects potholes, debris, animals, open manholes, sudden obstacles
- Provides **4–6 seconds of advance warning** via haptic + audio alerts

### 2. 💥 Accident Detection
- IMU sensors detect sudden deceleration, rollover, and impact events
- **97% accuracy** in simulation testing
- Within **8 seconds** of confirmed accident: GPS + occupant data auto-transmitted to emergency services

### 3. ❤️ Health Monitoring
- Steering-wheel biometric sensors: heart rate, SpO2, skin conductance
- Detects fatigue, stress, microsleep, and medical emergencies
- Optional family / fleet manager notifications

---

## 🌐 Smart Enhancements

| Feature | Description |
|---|---|
| ☁️ Cloud Hazard Mapping | Anonymized hazard data from all vehicles builds a real-time national road safety layer |
| 🏛️ Government Integration | API integration with NHAI, state PWDs, Smart City platforms for automatic maintenance requests |
| 🛡️ False Alert Prevention | Dual-validation (sensor + CV must agree) keeps false positives below 2% |
| 📱 Fleet Management API | Real-time driver health + route safety dashboard for commercial fleets |

---

## 📊 System Performance Benchmarks

| Metric | Value |
|---|---|
| Hazard Detection Accuracy | 97% |
| Accident Detection Accuracy | 98% |
| AI Inference Latency | < 50ms |
| System Uptime Target | 98% |
| Power Consumption | 2W |

---

## 📈 Expected Impact by 2030

- **45%** reduction in road fatalities
- **8x** faster emergency response
- **60%** fewer hazard-related accidents
- **10M+** vehicles protected
- **₹12,000 Crore** estimated economic savings

---

## ⚠️ Risk Analysis

| Risk | Mitigation |
|---|---|
| **Cost** | Target ₹5,000–8,000/unit at scale via government subsidies + B2B fleet contracts |
| **Rural connectivity** | Core features fully offline; cloud syncs when reconnected |
| **Data privacy** | Biometrics processed locally; cloud data anonymized + opt-in; DPDP Act 2023 compliant |
| **Hardware reliability** | IP67 + MIL-STD-810 rated; tested for dust, heat, monsoons, vibration |

---

## 🖥️ Website — Technical Details

### Stack
- **HTML5** — semantic structure
- **CSS3** — custom properties, flexbox, grid, animations, glassmorphism
- **Vanilla JavaScript** — no frameworks, no dependencies (except Chart.js)
- **Chart.js** (CDN) — accident data visualization

### Features Built
| Feature | Implementation |
|---|---|
| Loading screen | CSS radar sweep animation + JS fade-out after 2.8s |
| Particle field | Canvas API — 60 particles with connection lines |
| Network canvas | Canvas API — animated nodes in enhancements section |
| Scroll reveal | Intersection Observer API |
| Animated counters | requestAnimationFrame easing |
| Circular progress bars | SVG stroke-dashoffset animation |
| Chart | Chart.js dual-axis bar + line |
| PPT modal viewer | Inline base64 images, thumbnail strip, keyboard nav |
| Flow diagram | CSS + animated pulse dots |
| Responsive design | CSS Grid + Flexbox, mobile-first breakpoints |

### Design System
| Token | Value |
|---|---|
| Background | `#141414` — `#1a1a1a` — `#222222` |
| Text primary | `#f0ece4` (warm chalk white) |
| Text secondary | `#a8a09a` (chalk dust grey) |
| Accent red | `#d64444` |
| Accent blue | `#7aabcc` |
| Font — Headings | Bebas Neue |
| Font — Body | Rajdhani |
| Font — Mono/Labels | Share Tech Mono |

> The color palette and typography are directly inspired by the **chalkboard sketch aesthetic** of the project's PowerPoint presentation.

### PPT Integration
All 10 slides from `Accident.pptx` are converted to JPEG and embedded as **inline base64** in the HTML file — making it fully self-contained with zero external file dependencies.

**Slide list:**
1. RescueSync AI (Title)
2. Introduction
3. Research Survey
4. Inspiration
5. What is the Solution?
6. Core Features
7. Smart Enhancements
8. The Difference
9. Expected Impact
10. Thank You

---

## 🚀 How to Run

```bash
# No installation needed. Just open in a browser:
open index.html

# Or with a local server (optional):
npx serve .
python -m http.server 8000
```

Works in all modern browsers: Chrome, Firefox, Safari, Edge.

---

## 📁 File Structure

```
rescuesync-ai/
├── index.html        # Complete self-contained website (~7MB with embedded PPT)
└── README.md         # This file
```

> The website is intentionally a single file for portability — no assets folder, no build process, no server required.

---

## 👥 Team

**RescueSync AI** — Built for Hackathon 2025

*An AI-powered road safety initiative for India.*

---

## 📄 License

This project was created for a hackathon. All content is for demonstration and educational purposes.

---

*Built with ❤️ to make Indian roads safer.*
