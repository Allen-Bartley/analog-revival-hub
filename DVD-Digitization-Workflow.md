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

```text
/Movies
    /Animated
        - FernGully (1992) [tt0104254].mp4
        - The Fantastic Mr. Fox (2009) [tt0432283].mp4
        /Daria
            - Is It Fall Yet (2000) [tt0286244].mp4
            - Is It College Yet (2002) [tt0320819].mp4
    /Live Action
        - 10 Things I Hate About You (1999) [tt0147800].mp4

/TV_Shows
    /Animated
        /Darkwing Duck
            - Season folders or episode files…
    /Live Action
        /The IT Crowd
            - Season folders or episode files…
```
**Naming convention:**  
`Title (Year) [IMDb_ID].mp4` — Helps with media scraper accuracy and Plex-style integration.

---

## 📼 Special Project: *50 Sci-Fi Classics Box Set*

Digitizing each film individually from a budget anthology gift set.  
- Encoding same as above  
- Stored temporarily in `Videos` library for post-sorting  
- Will be integrated into archive once tagging and titles are finalized

---

## 📚 Reflections

Digitizing DVDs has been both practical and personal—especially when dealing with inherited media. It’s less about resolution and more about preservation. By accepting the source for what it is (often 480p with fuzzy prints), I’ve built a library that honors family film history and supports easy playback across devices.

---

🛠️ *Part of the Analog Revival Hub. From discs to digital with intention and structure.*
