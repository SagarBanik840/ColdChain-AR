# ColdChain-AR // Volumetric Thermal Breach Detection
### Next-Gen Pharmaceutical Logistics in Spatial Computing (WebXR for Meta Quest 3S)
**Event:** Young Innovators STEM Lab (YISL) — AR/VR Workshop  
**Venue:** K.R. Mangalam University  
**Target Device:** Meta Quest 3S (Full-Color Passthrough WebXR) & WebXR Cross-Platform Fallback  
**Deployment Stack:** Pure Single-File WebXR (`index.html`) using Pinned A-Frame 1.6.0  

---

## 🚀 Live Demo & Deployment
- **Live URL:** `https://YOUR_USERNAME.github.io/coldchain-ar/` *(Replace with your GitHub username upon fork/push)*
- **Demo Ready in < 60 Seconds:** Open the link in **Meta Quest Browser** on Quest 3S, tap **Enter AR**, and the holographic packing table anchors directly onto your physical floor.

---

## 🧊 The Operational Bottleneck & Problem Statement

> **The Industrial Reality:** Over $35 Billion USD worth of temperature-sensitive vaccines and biological medicines are wasted globally each year due to cold-chain failures during storage and transit.

### Why 2D Screens Fundamentally Fail ("Spatial Necessity")
- **The Flat Screen Trap:** Warehouse logistics handlers rely on flat 2D spreadsheets and single-point digital data loggers. These sensors are mounted on container walls or near door gaskets where forced reefer airflow circulates.
- **Deceptive Sensor Averages:** Because outer boundary sensors stay cool (4.5°C to 5.8°C), 2D software registers the entire shipment as `COMPLIANT [OK]`.
- **The Hidden 3D Hotspot:** In real-world cargo pallets, tightly packed carton geometries trap stagnant, warm air pockets in the internal core ($X \in [1..3], Y \in [1..2], Z \in [1..3]$). The interior core stagnates and climbs to **11.4°C+**, silently denaturing millions of doses with zero 2D alert.
- **The Spatial Necessity:** You cannot fix a 3-dimensional thermodynamic packing error using a 2-dimensional spreadsheet. Logistics personnel must be able to **slice into the pallet, inspect volumetric airflow traps, and position cold-pack phase-change materials in 3D space** before transit begins.

---

## 🔬 Core Solution: ColdChain-AR

**ColdChain-AR** is a browser-deployable WebXR digital twin built for the **Meta Quest 3S**. It renders a **100-cell volumetric pallet ($5 \times 4 \times 5$ matrix)** on an ergonomic spatial workbench:

1. **Split-Screen Cognitive Contrast:**
   - **Left Wing Hologram:** Traditional *2D Excel Spreadsheet Log* showing wall sensors averaging `5.8°C (PASS ✔)` — exposing the deceptive false sense of security.
   - **Right Wing Hologram:** *3D Volumetric Telemetry* revealing that 14 internal vaccine vials have breached critical thermal thresholds (`11.4°C BREACH ✖`).
2. **Interactive 3D Cold Pack Placement:** Handlers use Quest 3S Touch Plus laser pointers to remove trapped air pockets and place cold-chain phase-change blocks (limited by an authentic **8-pack payload budget**).
3. **Instant Deterministic Thermodynamic Engine:** Recomputes a 48-hour multi-substep heat diffusion simulation in < 3ms on every user click, rendering live temperature shifts across 0h, 12h, 24h, 36h, and 48h.
4. **Layer Slicing & 3D Exploded View:** One-click spatial tools allow handlers to slice horizontal layers (`Top Cut`, `Core Y:1-2`, `Base Y:0`) or expand spacing to reach deep inside the pallet.

---

## ⚡ 60-Second Competition Pitch & Judge Demo Script

| Time | Presenter Action | Spoken Pitch / Script |
|---|---|---|
| **0:00 - 0:15** | Put Quest 3S on Judge (or show laptop mirror). Tap **Enter AR**. | *"Judges, look at this vaccine pallet on our table. On the left, you see the traditional 2D Excel log. It reads 5.8°C and marks the batch 'APPROVED'. In 99% of warehouses today, this shipment gets loaded onto a truck."* |
| **0:15 - 0:30** | Point laser at the Right Wing Panel; click **`48h`** on Time Scrubber. | *"Now look at the 3D reality on your right. As 48 hours pass on an Indian summer tarmac, the external sensors still look fine—but 14 internal vaccine boxes in the core have reached 11.4°C. The batch is spoiled, and 2D software had no idea."* |
| **0:30 - 0:45** | Click **`CORE (Y:1-2)`** or **`EXPLODE 3D`**. Point laser into the red core and click to place Cold Packs. | *"With ColdChain-AR, handlers don't guess. We slice into the core, click the stagnant air pockets, and deploy thermal cold packs from our 8-pack budget."* |
| **0:45 - 1:00** | Click **`AI AUTO-FIX`** (or place optimal packs). Watch core turn emerald green. | *"Instantly, our thermodynamic engine recomputes 48 hours of transit. Peak temp drops to 5.2°C. Breaches drop to zero. The shipment is truly safe. This is Spatial Computing solving a multi-billion-rupee logistics crisis."* |

---

## 🛠️ Step-by-Step GitHub Pages Deployment Guide

To deploy this single-file project live on HTTPS (required by WebXR) in under 2 minutes:

### 1. Initialize Git & Commit
Open terminal in this project directory:
```bash
git init
git add .
git commit -m "feat: ColdChain-AR WebXR prototype for Meta Quest 3S"
```

### 2. Create GitHub Repo & Push
Create a new public repository named `coldchain-ar` on your GitHub account, then run:
```bash
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/coldchain-ar.git
git push -u origin main
```

### 3. Enable GitHub Pages
1. Go to your GitHub repository in your browser: `https://github.com/YOUR_USERNAME/coldchain-ar`.
2. Click **Settings** (gear icon) -> **Pages** (in left sidebar).
3. Under **Branch**, select `main` and folder `/ (root)`, then click **Save**.
4. Within 60 seconds, your site is published at:
   ```
   https://YOUR_USERNAME.github.io/coldchain-ar/
   ```

---

## 🥽 Testing on Meta Quest 3S

1. **Put on your Meta Quest 3S headset**.
2. Open the built-in **Meta Quest Browser**.
3. Type in your GitHub Pages URL (e.g., `https://YOUR_USERNAME.github.io/coldchain-ar/`).
   * *Tip:* To ensure fresh loading without browser cache during live iteration, append `?v=1` (or `?v=2`) to the URL.
4. On the webpage, tap the **Enter AR** button in the bottom-right corner.
5. **Full-Color Passthrough:** The virtual lab walls disappear, and the packing table anchors into your physical room at waist height.
6. **Interaction:**
   - Use the **Right or Left Touch Plus Controller**.
   - Point the cyan laser beam at buttons or pallet voxels.
   - Squeeze the **Index Trigger** to interact (place/remove cold packs, change time, slice layers).
   - Feel the haptic pulses on your controller on every interaction.

### Desktop & Smartphone Fallback (Zero-Headset Judges)
If presenting on a projector or laptop:
- Open the URL in Google Chrome, Microsoft Edge, or Safari.
- Click and drag with your **mouse** to orbit the workstation.
- Use **WASD keys** to navigate.
- Click buttons and 3D voxels directly with your mouse cursor.
- Use the **Floating 2D Glassmorphism Dashboard** in the top-left corner for 1-click preset demonstrations.

---

## 🧮 Technical Architecture & Thermodynamic Physics Model

### 1. The 100-Cell Volumetric Matrix
The pallet is structured as a discrete $5 \times 4 \times 5$ spatial lattice ($X \in [0..4], Y \in [0..3], Z \in [0..4]$):
- **Vaccine Case ($T_0 = 5.0^\circ\text{C}$):** Phase-tolerant biological vials requiring $2.0^\circ\text{C} \le T \le 8.0^\circ\text{C}$.
- **Cold Pack ($T_{\text{ice}} = 0.6^\circ\text{C}$):** High-density phase-change thermal sink clamped to near-zero with conduction coefficient $k = 0.12$.
- **Stagnant Air Gap ($T_0 = 16.5^\circ\text{C}$):** Unpacked air trapped during warehouse loading with low thermal conductivity ($k = 0.02$) creating an insulating barrier that prevents internal heat dissipation.

### 2. Realistic Convective Perimeter vs. Core Stagnation
Standard thermal diffusion models mistakenly cool the core first because outer faces contact ambient heat. ColdChain-AR implements realistic refrigerated transport physics:
$$\Delta T_i = \sum_{j \in \mathcal{N}(i)} k_{ij} (T_j - T_i) \cdot \Delta t$$
- **Boundary Condition 1 (Chiller Reefer Flow):** Outer corners and edge loggers receive forced cold air circulation ($T_{\text{reefer}} = 4.8^\circ\text{C}$), keeping external wall loggers safely green.
- **Boundary Condition 2 (Solar Ambient Leakage):** Pallet side walls exchange heat with exterior container ambient ($T_{\text{ambient}} = 35.0^\circ\text{C}$).
- **Core Heat Trapping:** Interior cells ($X \in [1..3], Y \in [1..2], Z \in [1..3]$) have no convective circulation, causing metabolic and trapped packaging heat to accumulate up to $11.4^\circ\text{C}$.

### 3. Procedural Audio Synthesizer (Web Audio API)
Zero external audio files (`.mp3` / `.wav`) are needed. All acoustic cues are synthesized procedurally in pure JavaScript:
- **Button Blip:** $850\text{ Hz}$ triangle wave ($60\text{ ms}$).
- **Voxel Toggle:** Double-tone chirp ($520\text{ Hz} \to 740\text{ Hz}$).
- **Budget Exceeded / Error:** Low sawtooth warning buzz ($180\text{ Hz} \to 140\text{ Hz}$).
- **Optimal Compliance Fanfare:** Ascending 4-note major arpeggio ($C_5 - E_5 - G_5 - C_6$).

---

## 📊 Anti-Cliché & Workshop Constraints Compliance

| Workshop Constraint | Implementation in ColdChain-AR |
|---|---|
| **Single HTML File Mandate** | 100% self-contained in `index.html`. Zero local asset folders, zero external `.glb` models, zero `.mp3` dependencies. |
| **Mandatory A-Frame Stack** | Built with pinned **A-Frame 1.6.0** with custom spatial components (`voxel-pallet`, `interactive-button`, `hud-controller`, `quest-ar-handler`). |
| **Target: Meta Quest 3S** | Native WebXR `immersive-ar` passthrough support, `local-floor` ergonomics, dual Touch Plus controller lasers, and physical haptics. |
| **Spatial Necessity Over Novelty** | Directly demonstrates why 2D screens fail (outer sensors pass while inner core breaches) and why 3D volumetric interaction is functionally essential. |
| **Under 60s Demoability** | Instant presets (`Bad Pack`, `AI Auto-Fix`, `Freeze Demo`) allow judges to experience the full problem and solution in seconds. |
| **Rapid Prototyping Budget** | Clean, deterministic JS physics model executing in < 3ms without heavy GPU shader bottlenecks. |

---

## 👥 Authors & Acknowledgments
- **Project:** ColdChain-AR Prototype
- **Workshop:** Young Innovators STEM Lab (YISL) — AR/VR Workshop
- **Institution:** K.R. Mangalam University
- **License:** MIT License — Open for educational and industrial research.
