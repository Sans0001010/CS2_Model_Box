# 📦 CS2 BOX for Blender

![Blender](https://img.shields.io/badge/Blender-3.6+-orange.svg)
![License](https://img.shields.io/badge/License-GPL_3.0-green.svg)
![Language](https://img.shields.io/badge/Language-Python-blue.svg)

> **中文版** | 🌐 **[English](README_en.md)**

---

**CS2 BOX** 是一款为 Blender 打造的高效反恐精英 2 (CS2) 模型导入辅助插件。
它极大地简化了从 VPK 提取到 Blender 资产生成的流程，让你只需点击几下即可完美呈现 CS2 资产！

## ✨ 核心特性

<img src="https://github.com/user-attachments/assets/7a20860d-044b-4ec3-9087-a0ac19a5b18b" align="right" width="180" alt="CS2 BOX UI 面板">

* 👤 **模型一键导入**
    * 略缩图可视化选择导入，目前支持探员(ag2)，武器。
    
* 🔫 **一键化功能**
    * 一键更换探员模型手套
    * 一键切换提取 **CS2 高清重制版 (HD)** 或保留经典 CSGO 低模。
    
* 🦴 **一键生成控制器 (ARP 集成)**
    * 无缝接入 Auto-Rig Pro (ARP) 插件。选中骨架后，一键读取预设并生成专业的角色骨骼控制器。

<br clear="both">

## 🛠️ 环境准备

1.  **Blender 3.6** 或更高版本。
2.  **[Source2Viewer-CLI.exe](https://github.com/ValveResourceFormat/ValveResourceFormat/releases)**：用于反编译 VPK 核心文件 (必须)。
3.  **Auto-Rig Pro (ARP)**：仅在使用“一键生成控制器”功能时需要 (可选)。

## 📦 安装与配置

1. 下载最新的 `.py` 脚本或 `.zip` 压缩包。
2. 打开 Blender，进入 `编辑` > `偏好设置` > `插件` > `安装`，选择文件并启用。
3. **关键步骤：** 展开插件设置面板，配置以下绝对路径：
   * `Source2Viewer-CLI.exe 路径` (选择: `Source2Viewer-CLI.exe`)
   * `CS2 VPK 路径` (如: `pak01_dir.vpk`)
   * `资源缓存目录`
   * `ARP 预设文件路径` (可选)
4. 在 3D 视图中按 `N` 键调出侧边栏，找到 **CS2 Importer** 面板，点击 **[加载资源缓存]** 即可开始使用！

---
*Created & Maintained by SANS*
