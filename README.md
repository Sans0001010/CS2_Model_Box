# 📦 CS2 BOX for Blender

![Blender](https://img.shields.io/badge/Blender-3.6+-orange.svg)
![License](https://img.shields.io/badge/License-GPL_3.0-green.svg)
![Language](https://img.shields.io/badge/Language-Python-blue.svg)

> **[English](#english-version)** | **[中文](#中文版)**

---

<a id="english-version"></a>
# 🇺🇸 English Version

**CS2 BOX** is an efficient and powerful Counter-Strike 2 (CS2) model importing add-on for Blender. 
It streamlines the entire pipeline—from decompiled VPKs to fully shaded, rig-ready assets in Blender. Say goodbye to manual material node setups, missing textures, and messy bone hierarchies!

## ✨ Core Features

* 🚀 **Dual-Engine Architecture**
    * **VRF Native Engine:** Lightning-fast parsing and automatic basic PBR node tree generation.
    * **SourceIO Engine:** Deep integration with SourceIO to fetch flawless model topology, weights, and advanced material structures.
* 🎨 **Auto PBR Material Reconstruction**
    * Automatically fetches and links Color, Normal, Roughness, Metallic, AO, and Emission textures from your cache directory.
* 👤 **Agent & Viewmodel (Arms) Separation**
    * Import the "Full Character Body" (3rd person) or just the "First-Person Arms" with smart culling of useless LODs and collision meshes.
    * **Modular Glove System:** Automatically removes default hands and equips special gloves (e.g., Bloodhound, Hand Wraps, Fingerless) with perfect armature parenting.
* 🔫 **Categorized Weapon Armory**
    * Visual grid preview for Firearms, Grenades, Knives, and Others.
    * Toggle between **CS2 HD Models** or classic CS:GO low-poly versions.
* 🦴 **1-Click Rig Generation (Auto-Rig Pro Integration)**
    * Seamlessly reads your ARP presets. Select the imported armature, click once, and instantly generate professional rigs.

## 🛠️ Prerequisites

1.  **Blender 3.6** or higher.
2.  **[VRF (Source 2 Resource Viewer)](https://vrf.steamdb.info/)**: Required for decompiling VPK files.
3.  **[SourceIO](https://github.com/REDxEYE/SourceIO)**: Recommended for optimal topology/weights.
4.  **Auto-Rig Pro (ARP)**: Optional, for the 1-click rig feature.

## 📦 Installation & Setup

1. Download the latest `.py` script or `.zip` release.
2. In Blender, go to `Edit` > `Preferences` > `Add-ons` > `Install` and select the downloaded file.
3. **CRITICAL:** Expand the add-on preferences and configure your absolute paths for:
   * `VRF Decompiler Path` (e.g., `Decompiler.exe`)
   * `CS2 VPK Path` (e.g., `pak01_dir.vpk`)
   * `Thumbnail Cache Directory`
   * `ARP Preset File Path` (Optional)
4. Open the 3D Viewport sidebar (`N` key), find the **CS2 Importer** tab, and click **[Load Resource Cache]**.

---

<a id="中文版"></a>
# 🇨🇳 中文版

**CS2 BOX** 是一款为 Blender 打造的高效反恐精英 2 (CS2) 模型导入辅助插件。
它极大地简化了从 VPK 提取到 Blender 资产生成的全流程，自动解决繁琐的材质节点连接、贴图丢失以及骨骼冗余问题，让你只需点击几下即可完美呈现 CS2 资产！

## ✨ 核心特性

* 🚀 **双引擎无缝切换**
    * **VRF 原生引擎:** 快速解析并自动生成基础 PBR 节点树，适合极速预览。
    * **SourceIO 引擎:** 调用 SourceIO 获得最完美的模型结构与权重，并在此基础上全自动注入高级材质。
* 🎨 **高阶 PBR 材质全自动重构**
    * 自动抓取缓存目录下的各项贴图（颜色、法线、粗糙度、金属度、AO、自发光），智能构建 Blender Shader 节点树。
* 👤 **探员与手模分离系统**
    * 支持“人物主体”与“第一人称手模”分离导入，智能剔除无用 LOD 模型。
    * **手套分离式挂载技术：** 一键剔除原生手部模型并穿戴指定手套，完美兼容绑带、无指等特殊手套拓扑。
* 🔫 **武器库与版本控制**
    * 按枪械、投掷物、刀具等分类可视化预览。
    * 支持切换提取 **CS2 高清重制版 (HD)** 或保留经典 CSGO 低模。
* 🦴 **一键生成控制器 (ARP 集成)**
    * 无缝接入 Auto-Rig Pro (ARP) 插件。选中骨架后，一键读取预设并生成专业的角色骨骼控制器。

## 🛠️ 环境准备

1.  **Blender 3.6** 或更高版本。
2.  **[VRF (Source 2 Resource Viewer)](https://vrf.steamdb.info/)**：用于反编译 VPK 核心文件 (必须)。
3.  **[SourceIO](https://github.com/REDxEYE/SourceIO)**：用于获取完美的导入拓扑和权重 (强烈推荐)。
4.  **Auto-Rig Pro (ARP)**：仅在使用“一键生成控制器”功能时需要 (可选)。

## 📦 安装与配置

1. 下载最新的 `.py` 脚本或 `.zip` 压缩包。
2. 打开 Blender，进入 `编辑` > `偏好设置` > `插件` > `安装`，选择文件并启用。
3. **关键步骤：** 展开插件设置面板，配置以下绝对路径：
   * `VRF Decompiler 路径` (如: `Decompiler.exe`)
   * `CS2 VPK 路径` (如: `pak01_dir.vpk`)
   * `缩略图缓存目录`
   * `ARP 预设文件路径` (可选)
4. 在 3D 视图中按 `N` 键调出侧边栏，找到 **CS2 Importer** 面板，点击 **[加载资源缓存]** 即可开始使用！

---
*Created & Maintained by SANS*
