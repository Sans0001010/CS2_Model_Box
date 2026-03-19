# 📦 CS2 BOX for Blender

![Blender](https://img.shields.io/badge/Blender-3.6+-orange.svg)
![License](https://img.shields.io/badge/License-GPL_3.0-green.svg)
![Language](https://img.shields.io/badge/Language-Python-blue.svg)

> **[中文版](README.md)** | 🌐 **English**

---

**CS2 BOX** is an efficient Counter-Strike 2 (CS2) model importing companion add-on for Blender. 
It greatly simplifies the workflow from VPK extraction to Blender asset generation, letting you present perfect CS2 assets with just a few clicks!

## ✨ Core Features

<img src="https://github.com/user-attachments/assets/7a20860d-044b-4ec3-9087-a0ac19a5b18b" align="right" width="150" alt="CS2 BOX UI Panel">

* 👤 **1-Click Model Import**
    * Visual import selection with thumbnails. Currently supports agents (ag2) and weapons.
    
* 🔫 **Automated 1-Click Features**
    * 1-Click agent glove replacement.
    * 1-Click toggle to extract **CS2 High-Definition (HD)** meshes or keep classic CS:GO low-poly models.

* 🦴 **1-Click Rig Generation (ARP Integration)**
    * Seamless integration with the Auto-Rig Pro (ARP) add-on. Select the armature, click once, and instantly load presets to generate professional character rigs.

<br clear="both">

## 🛠️ Prerequisites

1.  **Blender 3.6** or higher.
2.  **[Source2Viewer-CLI.exe](https://github.com/ValveResourceFormat/ValveResourceFormat/releases)**: Required for decompiling core VPK files (Mandatory).
3.  **Auto-Rig Pro (ARP)**: Only required if using the "1-Click Rig Generation" feature (Optional).

## 📦 Installation & Setup

1. Download the latest `.py` script or `.zip` release.
2. Open Blender, go to `Edit` > `Preferences` > `Add-ons` > `Install`, select the downloaded file, and check the box to enable it.
3. **CRITICAL STEP:** Expand the add-on preferences panel and configure the following absolute paths:
   * `Source2Viewer-CLI.exe Path` (Select: `Source2Viewer-CLI.exe`)
   * `CS2 VPK Path` (e.g., `pak01_dir.vpk`)
   * `Resource Cache Directory`
   * `ARP Preset File Path` (Optional)
4. In the 3D Viewport, press `N` to open the sidebar, find the **CS2 Importer** tab, and click **[Load Resource Cache]** to get started!

---
*Created & Maintained by SANS*
