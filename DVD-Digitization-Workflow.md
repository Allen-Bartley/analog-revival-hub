# 📀 DVD Digitization Workflow

### *Preserving personal film archives with GPU-accelerated encoding and structured media curation.*

This module outlines my typical process for digitizing DVDs using HandBrake, with a focus on speed, quality preservation, and organizing content into a structured library for long-term access. Whether it’s discount box sets or inherited collections, I aim to create usable digital copies that respect the original source and fit neatly into my archival ecosystem.

---

## 🧩 Summary

- **Goal:** Convert physical DVDs into digitally accessible files for personal library playback and archival organization.
- **Tools Used:** HandBrake + NVIDIA NVEnc hardware acceleration
- **Source Material:** Personal collection, inherited discs, discount genre box sets (e.g., *50 Sci-Fi Classics*)
- **Philosophy:** Prioritize completeness and efficiency over unnecessary upscaling or format inflation

---

## 🛠️ Hardware & Software

| Item                      | Role                                                   |
|---------------------------|--------------------------------------------------------|
| External DVD Drive        | USB-powered disc reading and ripping                   |
| Desktop PC (RTX 3060)     | Accelerated encoding via NVEnc hardware                |
| HandBrake                 | Open-source video transcoder used for all conversions  |

---

## ⚙️ Encoding Settings

- **Video Encoder:** H.264 (NVIDIA NVEnc)
- **Preset:** Fast 480p30 (Modified)
- **Quality:** Constant Quality RF 20
- **Audio:** Default stereo track (usually AC3 or AAC, preserved as-is)
- **Subtitles:** None unless deemed essential
- **Output Format:** `.mp4` for broad compatibility

---

## 📁 Folder Structure

All digitized media lives on an external archive drive organized as follows:

