# 🎨 DsPico Cover Converter

An efficient, browser-based utility to convert game covers into the **8-bit BMP format** required by the **DsPico**. This tool streamlines your workflow by automatically identifying ROM headers and organizing your assets directly on your SD card.

## 🚀 Features

* **Dual Mode Workflow:**
    * **Normal Download:** Quickly convert images and download them as individual files or a ZIP archive.
    * **Auto SD Card Save:** Seamlessly map your covers to your ROM library and let the tool organize everything on your SD card.
* **Intelligent Header Analysis:** Automatically extracts the 4-character **GameID** from `.nds` and `.gba` files.
* **Automated File Structure:** Automatically organizes files into the correct subdirectories:
    * `_pico/covers/gba/` (GameID.bmp)
    * `_pico/covers/nds/` (GameID.bmp)
    * `_pico/covers/user/` (Full original filename.bmp)
* **Optimized Conversion:** Ensures perfect 128x96 8-bit BMP output with proper color palette mapping.
* **Browser-Based:** No installation required. Runs directly in Chrome, Edge, or Opera.

## 📂 SD Card Structure

Once you use the **Auto SD Card Save** feature, the tool generates this structure on your SD card:

```text
_pico/
└── covers/
    ├── gba/       # GBA ROMs (named by GameID, e.g., AGFE.bmp)
    ├── nds/       # NDS ROMs (named by GameID, e.g., YJBP.bmp)
    └── user/      # Other ROMs (full filename retained, e.g., Super Mario.nes.bmp)
