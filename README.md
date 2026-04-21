# XI-MC 2026 ReVamp

A Windows utility for **Final Fantasy XI** / **Horizon XI** players: browse and preview in-game `.bgw` music, export to WAV, and replace tracks with your own audio — converted to stock-style BGMStream — with backups and a simple UI.

## Download

**Installer (latest):** [**XI-MC-2026-ReVamp-Setup.exe**](XI-MC-2026-ReVamp-Setup.exe) (v1.2.35)

Run the installer, then launch **XI-MC 2026** from the Start Menu (folder: **XI-MC 2026 ReVamp**).  
The first-time wizard explains what the program does, what gets installed, and a short disclaimer.

<!-- RELEASE_NOTES_START -->
### Changes in v1.2.35

- **Workflow change:** Ship with **manual** **`1 - REBUILD APP`** → **`2 - Build Installer`** → **`3 - Publish Public Release`** (no chained “run all three” batch). Step **3** normalizes **README.md** (UTF-8, no BOM), copies **`installer_output\XI-MC-2026-ReVamp-Setup-<version>.exe`** to the repo-root **`.exe`**, commits with subject **Release v…** (version from Inno **`MyAppVersion`**) and **this entire block** as the commit body, pushes, and creates/updates the **GitHub Release** — no manual file copies.
- **Catch-up:** The last **GitHub** release with full notes was **v1.2.25**. **v1.2.35** ships the installer plus **everything listed below** from **v1.2.26** through **v1.2.35**.
- **Going forward:** Bump **`#define MyAppVersion`** in **`installer\XI-MC-2026-ReVamp.iss`** by **0.01**, match this README (download line + notes) and **`MusicMaker.py`**, then run **1 → 2 → 3**.

### Changes in v1.2.34

- **MyMusic removed:** No scanning or logic under `polplugins\DATs\MyMusic\ROM`. Workflow is **horizonmusic** (or retail) pack paths plus `…\music\data\Backup\`, and **AppData** `custom_stash` + manifest for convert/reapply.
- **Auto-Detect preview:** `custom_stash` → Horizon pack → retail (no MyMusic).
- **Custom column (C):** Manifest + pack edits, including **R\*** from `.retail` markers next to pack `.bgw` under horizonmusic and retail.

### Changes in v1.2.26 through v1.2.33

- **v1.2.33:** **R\*** after restart for pack-only retail overrides (no MyMusic manifest); **122/135** and **122/162** `.retail` keys mirrored to folder **123** for Kazham / Heaven's Tower dedupe.
- **v1.2.32:** **Use Retail Version Here:** restore **R\*** by scanning `.retail` next to pack `.bgw` under horizonmusic and retail.
- **v1.2.31:** Track list **Files:** filter (All / Retail Only / HXI Only / Custom Only) from R H C; saved as `avail_filter` in `ximc_config.json`.
- **v1.2.30:** **Heaven's Tower (162):** same **122/123** + **sound/sound2** pairing as Kazham (135); single list row **123/162**; `tracks.csv` uses one **123/162** row.
- **v1.2.29:** **HorizonXI** / **Retail Original** preview uses `Backup\` when it differs from live (no separate Backup source in the UI); **Horizon Override** renamed to **HorizonXI**.
- **v1.2.28:** Auto-Detect order evolved (superseded by v1.2.34 stash-first behavior).
- **v1.2.27:** Optional explicit backup sources (superseded by v1.2.29 automatic backup preview).
- **v1.2.26:** If a fixed Source has no file, fall back to Auto-Detect order and update the dropdown instead of erroring.

### Changes in v1.2.25

- **Kazham:** When both `sound/135` and `sound2/135` exist, the track list shows one row (folder 123) with merged R/H/C; preview paths search the right pack order for Horizon vs retail.
- **Yuhtunga Jungle:** Stray `sound/134` (122/134) on disk is ignored so it does not duplicate **123/134** (Yuhtunga is sound2 only in the list).
- **Track names:** HXI slots **617** (Delkfutt's Tower) and **623** (Quicksand Caves) use proper names in `tracks.csv`.

<!-- RELEASE_NOTES_END -->

## Requirements

- Windows (64-bit)
- A legitimate FFXI / Horizon XI installation (the app needs your game paths)

## Disclaimer

Fan-made tool for **personal use only**. Not affiliated with Square Enix or Horizon XI.  
Final Fantasy XI is a trademark of Square Enix Co., Ltd. This project does not distribute game assets or music. Use at your own risk; keep backups of your game files.

## Repository

This public repository contains **only** this README and the current Windows installer. It does not include source code, batch files, or the app source tree — those stay on the maintainer’s machine.

Repository: **https://github.com/ferrisaj87/XI-MC-2026-ReVamp**
