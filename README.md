# 👾 FLAKY: Escape the Pipeline

[![Play Live](https://img.shields.io/badge/PLAY_NOW-Live_on_GitHub_Pages-63c74d?style=for-the-badge&logo=github)](https://princelyroyan.github.io/flaky/)
[![Built With](https://img.shields.io/badge/Built_With-Gemini_Argon-2ce8f5?style=for-the-badge&logo=google)](https://princelyroyan.github.io/flaky/)
[![Architecture](https://img.shields.io/badge/Architecture-Single_HTML_File-feae34?style=for-the-badge)](#technical-highlights)

> *"Never trust a test that passes on the first try."*

**FLAKY: Escape the Pipeline** is a retro 8-bit auto-running action-platformer built entirely inside a **single, self-contained HTML file** with zero external images, audio files, or libraries. 

### 🕹️ [Play the Game Here (Mobile & Desktop)](https://princelyroyan.github.io/flaky/)

---

## 📖 The Plot

It’s **4:55 PM on Friday the 13th**. You are **Tess**, a Senior SDET at a tiny startup. 

The game opens with a short typewriter-style story intro that sets the scene: the office empties out, one last commit lands, and the pipeline starts glitching as the Heisenbug wakes up. Tap to fast-forward a page, tap again to continue, or hit **SKIP** to jump straight to the title screen. You can watch it again any time with **REPLAY STORY INTRO** on the title screen.

Just before the weekend, the CI/CD pipeline is corrupted by a rogue AI called **"The Heisenbug,"** causing tests to pass and fail at random. Tess must fight through all 5 stages of the pipeline, squash bugs, stabilize flaky tests, and destroy the giant red **"Friday Deploy"** button before untested code ships to production and takes the whole company down.

---

## 🎮 Controls (Touch & Mouse)

Designed for portrait mode (`360x640` logical resolution) on mobile browsers:

* **JUMP Button (bottom left) or Tap / Hold Anywhere on Screen:** Jump (Hold for a higher jump)
* **FIRE Button (bottom right):** Fire an `assert()` projectile. Hold it down to auto-fire
* **Swipe Down:** Slide under high hazards and bullets

Both buttons are multi-touch friendly: keep one thumb on FIRE while the other works JUMP and slides.

**Telling gifts from threats:** power-ups pulse with a bright neon halo and a `+` tag, while every enemy carries a flashing red `!` warning sign above it.

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

## 🏅 Shareable Badge

Beat the final boss and the victory screen offers **SHARE MY BADGE**: a 1080×1080 pixel-art certificate ("Certified Friday Deploy Blocker") with your name, stats, rank and all five pipeline stages green. Lose a run and the game-over screen offers a **FAIL CARD** instead ("Pipeline failed at stage N. Rerun on Monday.").

* **Ranks:** finish with all 3 tests intact for `PRINCIPAL WEEKEND GUARDIAN`, 2 for `SENIOR SDET`, otherwise `JUNIOR SDET`.
* **On phones** the share button opens the native share sheet with the image attached, so LinkedIn, WhatsApp, Instagram and friends are one tap away.
* **On desktop** it downloads the PNG and copies a ready-made caption (with the game link and hashtags) to your clipboard to paste into a LinkedIn post.
* Your name is remembered on the device so you only type it once. Everything is generated in the browser, nothing is uploaded anywhere.

---

## 🛠️ Technical Highlights

* **Zero External Assets:** Every sprite, icon, and background is rendered procedurally in JavaScript using a strict 16-color NES-inspired hex palette (`PAL`) and cached to offscreen `<canvas>` elements for 60 FPS performance.
* **Web Audio API Chiptune Synthesizer:** The background music is a single-voice 8-bit cover of Beethoven's *Für Elise* (public domain), written as note names in the code and played on a `triangle` wave; the boss fight plays it an octave down on a `sawtooth`. All sound effects are synthesized in real time with zero `.mp3` or `.wav` files.
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

---

## 👤 Creator

Created by **Princely Royan Philip**.
