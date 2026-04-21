# XI-MC 2026 ReVamp

A Windows utility for **Final Fantasy XI** / **Horizon XI** players: browse and preview in-game `.bgw` music, export to WAV, and replace tracks with your own audio — converted to stock-style BGMStream — with backups and a simple UI.

<!-- Keep permanently: heritage credit + comparison screenshots (do not remove). -->
This addon was inspired by the 2003 application **Ximc** by **Kaede** to expand its abilities!

**XI-MC 2026 ReVamp** was **rebuilt** to replicate **Ximc**’s core functionality and **expand** it for **Modern FFXI / HorizonXI Players**: browse and preview what you hear in **Vana’diel**, swap in your own tracks with proper backups, export to WAV, and shape the soundtrack around **your** journey.

<table>
  <tr>
    <td width="50%" valign="top" align="center">
      <strong>OG 2003</strong><br /><br />
      <img width="583" height="247" alt="Ximc (2003) by Kaede" src="https://github.com/user-attachments/assets/f45f2926-c4a7-4fba-bcb2-3c1e4528348b" />
    </td>
    <td width="50%" valign="top" align="center">
      <strong>2026 version</strong><br /><br />
      <img width="583" height="523" alt="XI-MC 2026 ReVamp" src="https://github.com/user-attachments/assets/e7ca7d58-100b-42ae-837b-5754fdf78964" />
    </td>
  </tr>
</table>

## Download

**Installer (latest):** [**XI-MC-2026-ReVamp-Setup.exe**](XI-MC-2026-ReVamp-Setup.exe) (v1.2.35)

Run the installer, then launch **XI-MC 2026** from the Start Menu (folder: **XI-MC 2026 ReVamp**).  
The first-time wizard explains what the program does, what gets installed, and a short disclaimer.

<!-- RELEASE_NOTES_START -->
### Changes in v1.2.35

- **Workflow updates:** Release packaging and download page only (no change to app behavior).

### Changes in v1.2.34

- **Paths & scanning:** The app no longer looks at the legacy MyMusic ROM folder. Browsing, preview, and writes use Horizon pack paths, retail, local backups, and your customs saved under AppData.
- **Preview (Auto-Detect):** Uses your saved customs first, then the Horizon pack, then retail.
- **Track list:** Retail overrides and custom edits (including markers next to pack files) show correctly in the list columns.

### Changes in v1.2.26 through v1.2.33

- **v1.2.33:** Retail override indicators stay correct after restart when you only changed pack files; Kazham and Heaven's Tower stay as single, merged rows in the list.
- **v1.2.32:** **Use Retail Version Here** correctly restores override markers after restart by finding sidecar files next to pack music.
- **v1.2.31:** **Files** filter on the track list (all tracks vs retail-only vs HXI-only vs your customs); your choice is remembered.
- **v1.2.30:** Heaven's Tower uses the same list and preview rules as Kazham (one merged row, correct behavior across sound folders).
- **v1.2.29:** Preview can pull from your **Backup** copy when that’s still the original stock file; the Horizon option is labeled **HorizonXI** for clarity.
- **v1.2.28–v1.2.26:** **Auto-Detect** and preview behave better when a chosen source file is missing (smarter fallbacks, fewer errors).

### Changes in v1.2.25

- **Kazham:** One merged row when the game has both sound folders; preview follows the right order for Horizon vs retail.
- **Yuhtunga Jungle:** Stray duplicate entries on disk no longer show up as an extra row.
- **Track names:** Delkfutt's Tower and Quicksand Caves show correct names in the list.

<!-- RELEASE_NOTES_END -->

## Requirements

- Windows (64-bit)
- A legitimate FFXI / Horizon XI installation (the app needs your game paths)

## Disclaimer

Fan-made tool for **personal use only**. Not affiliated with Square Enix or Horizon XI.  
Final Fantasy XI is a trademark of Square Enix Co., Ltd. This project does not distribute game assets or music. Use at your own risk; keep backups of your game files.

## Repository

This public repository contains **only** this README and the current Windows installer (no full source tree here).

Repository: **https://github.com/ferrisaj87/XI-MC-2026-ReVamp**
