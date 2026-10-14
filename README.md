# 👾 FLAKY: Escape the Pipeline

[![Play Live](https://img.shields.io/badge/PLAY_NOW-Live_on_GitHub_Pages-63c74d?style=for-the-badge&logo=github)](https://princelyroyan.github.io/flaky/)
[![Built With](https://img.shields.io/badge/Built_With-Gemini_Argon-2ce8f5?style=for-the-badge&logo=google)](https://princelyroyan.github.io/flaky/)
[![Architecture](https://img.shields.io/badge/Architecture-Single_HTML_File-feae34?style=for-the-badge)](#technical-highlights)

> *"Never trust a test that passes on the first try."*

**FLAKY: Escape the Pipeline** is a retro 8-bit auto-running action-platformer built entirely inside a **single, self-contained HTML file** with zero external images, audio files, or libraries. 

### 🕹️ [Play the Game Here (Mobile & Desktop)](https://princelyroyan.github.io/flaky/)

---

## 📖 The Plot

It’s **4:55 PM on a Friday**. You are **Tess**, a Senior SDET at a tiny startup. 

Just before the weekend, the CI/CD pipeline is corrupted by a rogue AI called **"The Heisenbug,"** causing tests to pass and fail at random. Tess must fight through all 5 stages of the pipeline, squash bugs, stabilize flaky tests, and destroy the giant red **"Friday Deploy"** button before untested code ships to production and takes the whole company down.

---

## 🎮 Controls (Touch & Mouse)

Designed for portrait mode (`360x640` logical resolution) on mobile browsers:

* **Tap / Hold Anywhere on Screen:** Jump (Hold for a higher jump)
* **FIRE Button (bottom right):** Fire an `assert()` projectile. Hold it down to auto-fire
* **Swipe Down:** Slide under high hazards and bullets

The FIRE button is multi-touch friendly: keep one thumb on it while jumping and sliding with the other.

---

## 🏗️ The 5 Pipeline Stages & Enemies

| Stage | Environment | Enemies & Hazards | Stage Boss |
| :--- | :--- | :--- | :--- |
| **1. Commit Stage** | Onboarding Grid | **Typo Bugs**, Floating **NullPointers** | `LINTER DAEMON` |
| **2. Build Stage** | Dependency Hell Pits | **Version Conflicts** (`<<`), **Memory Leak Slimes** (grow over time) | `NODE_MODULES BLOB` |
| **3. Unit Test Stage** | Fast & Tight Rooms | **Flaky Test Ghosts** (only hittable when 100% solid) | `HEISENBUG PHANTOM` |
| **4. Integration Stage** | Moving Platforms | **Race Conditions** (must hit both within 1.0s!), **504 Timeout Spiders** | `DEADLOCK DEMON` |
| **5. E2E Stage** | Long Endurance Run | **The Product Manager** (can't be shot, jump over!), **The Customer** (can't be shot, slide under!), Spiders, Ghosts | `SELECTOR HYDRA` & **`FRIDAY DEPLOY`** |

### 🚨 Final Boss: FRIDAY DEPLOY (3 Phases)
1. **Phase 1:** Dodge high and low `HOTFIX` bullet-hell barrages while chipping away its health.
2. **Phase 2:** Shoot all 3 **Code Review (`PR1`, `PR2`, `PR3`)** switches to get `LGTM!` approvals.
3. **Phase 3:** Expose and destroy the pulsing **`ROLLBACK`** core before it ships to prod!

---

## ⚡ Power-Ups

* ☕ **Coffee:** 5-second speed boost.
* 🛡️ **Mock Shield:** Blocks one hit of damage.
* 🔄 **Retry x3:** Grants an extra life (`Retry passed! +1 ✓`).
* 📊 **Test Data:** Temporary triple-shot `assert()` spread.
* 🟢 **Code Coverage Orb:** Boosts your Coverage % score toward 100%.
* 💻 **"It Works On My Machine" (Easter Egg):** Rare laptop drop that grants temporary invincibility.

---

## 🛠️ Technical Highlights

* **Zero External Assets:** Every sprite, icon, and background is rendered procedurally in JavaScript using a strict 16-color NES-inspired hex palette (`PAL`) and cached to offscreen `<canvas>` elements for 60 FPS performance.
* **Web Audio API Chiptune Synthesizer:** Background music loops and retro sound effects (`square`, `triangle`, and `sawtooth` waves) are synthesized in real time with zero `.mp3` or `.wav` files.
* **Installable PWA in One File:** Uses inline SVG Data URIs for app icons, an inline `data:application/manifest+json` Web App Manifest, and a Blob-registered Service Worker so it can be installed full-screen on **iOS** and **Android**.

---

## 📱 How to Install as an App on Your Phone

1. Open **[https://princelyroyan.github.io/flaky/](https://princelyroyan.github.io/flaky/)** on your phone.
2. **On Android (Chrome):** Tap the three-dot menu (`⋮`) $\rightarrow$ **Add to Home screen** $\rightarrow$ **Install**.
3. **On iOS (Safari):** Tap the **Share** button $\rightarrow$ **Add to Home Screen**.

---

## 🚀 Running Locally

No `npm install`, no build step, and no `node_modules` black hole required:

```bash
git clone [https://github.com/princelyroyan/flaky.git](https://github.com/princelyroyan/flaky.git)
cd flaky
# Open index.html in any browser!
