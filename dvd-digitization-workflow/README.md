# 📀 DVD Digitization Workflow

A detailed log of Allen Bartley’s DVD media archive, digitized and organized across genres, formats, and personal interests. This list reflects hundreds of titles curated with care, narrative respect, and playback-friendly structure.

> *Every folder tells a story. Every format preserves a legacy.*

---

## 🧠 Folder Structure Philosophy

- **Format Authenticity**: Original `.avi`, `.mp4`, `.mkv`, `.wmv`, and `.flv` files maintained.
- **Playback Clarity**: Disc splits, multipart mini-series, and specials labeled for sequence control.
- **Genre Integrity**: Sorted by thematic grouping—animation, horror, comedy, sci-fi, fan content.
- **Nostalgic Touches**: Care Bears, classic anime OVAs, MLP fan works, convention panels, and legacy trailers.

---

## 📁 Library Categories

### 🎥 Classic & Cult Films
*The Rocky Horror Picture Show*, *Clerks*, *Dogma*, *Office Space*, *Scott Pilgrim vs. The World*, *Big Trouble In Little China*, *The Fifth Element*, *Labyrinth*, *The Dark Crystal*, *Willy Wonka and the Chocolate Factory*

### 🧟 Horror & Suspense
*A Nightmare on Elm Street Collection*, *Friday the 13th Collection*, *Halloween Collection*, *Hellraiser I–VIII*, *The Evil Dead Trilogy*, *Stephen King's The Shining (1997)*, *The Stand*, *Rose Red*, and *It (1990)*

### 📺 TV Series & Mini-Series
*The IT Crowd (Seasons 1–4 + Specials)*, *Doctor Who (Modern Series & Specials)*, *The Real Ghostbusters*, *Darkwing Duck*, *The Adventures of Teddy Ruxpin*, *Chobits*, *Claymore*, *The Colony (Seasons 1 & 2)*

### 🧠 Anime Archive
*Lupin the III (25+ Movies, Specials & OVAs)*, *Ranma ½ (All 7 Seasons, Movies & OVAs)*, *Tenchi Muyo (GXP & Ryo-ohki)*, *Wolf and Spice (Seasons 1 & 2)*, *Miyazaki Films (Spirited Away, Princess Mononoke, etc.)*

### 🎭 Fan Works & Internet Culture
*The Gamers: Dorkness Rising*, *Dr. Horrible’s Sing-Along Blog*, *Rifftrax*, *Fallout: Equestria (Fan Animations)*, *PAX: Acquisitions Inc. Panels*, *Children of the Night & Lullaby for a Princess (MLP Fan Animations)*

### 📚 Personal Archives
*Holiday Specials (Rudolph, Frosty, etc.)*, *Classic Animated Christmas Specials (He-Man, The Snowman)*, *Acquisitions Incorporated PAX Live Games (2014 & 2015)*

---

## 🛠️ Tools & Workflow

File inventory generated using a custom batch script designed to scan media formats and produce a clean text export of all DVD titles.

```bat
@echo off
REM ============================================================================
REM  Media Inventory Script for DVD Digitization Project
REM  Author: Allen Bartley (with AI assistance)
REM  Purpose: Scans a specified directory for video files and outputs a
REM           list of full paths to an inventory text file.
REM ============================================================================

REM --- Configuration ---
SET "SCAN_DIRECTORY=%~dp0"
REM Sets the directory to scan. %~dp0 defaults to the script's own directory.
REM For a different directory, change it e.g., SET "SCAN_DIRECTORY=E:\Documents\Videos"

SET "OUTPUT_FILE=DVD-Inventory.txt"
REM Sets the name of the output file.

REM A list of file extensions to search for.
SET "FILE_TYPES=*.mp4 *.avi *.mkv *.flv *.wmv"

REM --- Script Execution ---
echo.
echo  Scanning for media files...
echo  ---------------------------------
echo  Source Directory: %SCAN_DIRECTORY%
echo  Output File:      %OUTPUT_FILE%
echo  ---------------------------------
echo.

REM Deletes the old inventory file if it exists to start fresh.
IF EXIST "%OUTPUT_FILE%" (
    DEL "%OUTPUT_FILE%"
)

REM The main loop. It searches recursively (/r) through the scan directory
REM for each file type specified in the FILE_TYPES variable.
REM '%%F' is the variable that holds the full path of each found file.
FOR /R "%SCAN_DIRECTORY%" %%F IN (%FILE_TYPES%) DO (
    REM Appends the full path of the found file to the output file.
    echo %%F >> "%OUTPUT_FILE%"
)

echo.
echo  Scan complete. Inventory saved to %OUTPUT_FILE%
echo.
```
The output can be piped into Markdown-friendly formats or parsed into future inventory modules.

For other tools and scripts, see [`/tools`](../tools).

---

## ✨ Next Steps

- [ ] Expand listing with searchable index by title or franchise  
- [ ] Add subfolder views to showcase organizational logic  
- [ ] Integrate genre tagging tool or visual breakdown  
- [ ] Publish workflow to GitHub as part of systems literacy showcase

This is the first layer of a personal preservation project—and just the beginning.

---
