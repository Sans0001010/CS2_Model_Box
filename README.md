# 📦 CS2 BOX for Blender

![Version](https://img.shields.io/badge/Version-0.0.23-blue.svg)
![Blender](https://img.shields.io/badge/Blender-3.6+-orange.svg)
![License](https://img.shields.io/badge/License-GPL_3.0-green.svg)

**CS2 BOX** 是一款为 Blender 打造的极致反恐精英 2 (CS2) 模型导入辅助插件。
它集成了强大的双引擎解析架构，彻底解决了传统导入流程中繁琐的材质节点连接、贴图丢失以及骨骼冗余问题，让你只需点击几下，即可在 Blender 中完美呈现 CS2 的探员、手套与武器！

---

## ✨ 核心特性 (Core Features)

* 🚀 **极致双引擎无缝切换**
    * **VRF 原生引擎 (极速):** 快速解析并自动生成基础 PBR 节点树，适合快速预览。
    * **SourceIO 引擎 (极致):** 调用 SourceIO 获得最完美的模型结构与权重，**(V23版本已彻底修复底层 API 调用崩溃的史诗级 Bug)**，实现 100% 精准唤醒并全自动注入高级材质。
* 🎨 **高阶 PBR 材质全自动重构**
    * 自动抓取缓存目录下的 Color、Normal、Roughness、Metallic、AO 和 Emission 贴图。
    * 智能构建 Blender Shader 节点树，一键还原游戏内真实质感。
* 👤 **探员与独立手模系统**
    * 支持“人物主体”与“第一人称手模”分离导入。
    * 智能剔除无用 LOD (lod1-5)、阴影模型和碰撞体。
    * **手套分离式挂载技术：** 自动剔除原生手部模型，一键穿戴并匹配目标骨架，完美兼容各类特殊手套（如绑带、九头蛇、无指手套）。
* 🔫 **武器库与版本控制**
    * 按枪械、投掷物、刀具等分类可视化预览。
    * 支持切换提取 **CS2 高清重制版 (HD)** 或保留经典 CSGO 低模。
* 🦴 **一键生成控制器 (ARP 集成)**
    * 无缝接入 Auto-Rig Pro (ARP) 插件。
    * 选中骨架后，一键读取预设并生成专业的角色骨骼控制器。

---

## 🛠️ 环境准备 (Prerequisites)

为了让 CS2 BOX 发挥全部实力，请确保你的环境中已安装以下工具：

1.  **Blender 3.6** 或更高版本。
2.  **[Source 2 Resource Viewer (VRF)](https://vrf.steamdb.info/)**：用于反编译 VPK 核心文件 (必须)。
3.  **[SourceIO](https://github.com/REDxEYE/SourceIO)**：用于获取最完美的导入拓扑和权重 (强烈推荐)。
4.  **Auto-Rig Pro (ARP)**：仅在使用“一键生成控制器”功能时需要 (可选)。

---

## 📦 安装说明 (Installation)

1.  在 GitHub Release 页面下载最新的 `CS2_BOX.zip` 源码包（或直接下载 `.py` 脚本）。
2.  打开 Blender，进入 `编辑 (Edit)` > `偏好设置 (Preferences)` > `插件 (Add-ons)`。
3.  点击右上角的 `安装 (Install)`，选择下载的文件并勾选启用。
4.  **关键步骤：展开插件设置面板，配置以下路径：**
    * `VRF Decompiler 路径` (如: `Decompiler.exe` 的绝对路径)
    * `CS2 VPK 路径` (如: `pak01_dir.vpk` 的绝对路径)
    * `缩略图缓存目录` (存放 JSON 索引和临时文件的文件夹)
    * `ARP 预设文件路径` (如使用一键绑定功能)

---

## 🚀 快速上手 (Quick Start)

1.  在 3D 视图中按 `N` 键调出侧边栏，找到 **CS2 Importer** 面板。
2.  点击 **[加载资源缓存]**，初始化图标与数据索引。
3.  **导入探员/手套**：
    * 选择阵营 (CT/T) 和探员头像。
    * 选择导入引擎 (推荐 SourceIO) 与导入模式 (探员主体/手模)。
    * 点击 **[一键导入探员]**。
    * 如需更换手套，选中刚导入的骨架，在手套列表中选择目标，点击 **[替换手套]**。
4.  **导入武器**：
    * 切换至【武器/道具】模式。
    * 选择分类并点击对应武器图标。
    * 点击 **[导入选中武器]**。

---

## 📝 更新日志 (Changelog)

**v0.0.23**
* **[Fix]** 彻底修复调用 SourceIO 插件时由于 `hasattr` 被 Blender API 欺骗导致的崩溃报错问题，采用 `dir()` 直接读取注册表，完美兼容最新版 SourceIO。
* **[Add]** 引入高阶 PBR 材质重构系统，支持 AO 贴图正片叠底与自发光通道。
* **[Add]** 完善手套逻辑，支持 `fingerless` 等特殊材质判断和模型替换。

---

## 🤝 贡献与反馈 (Contributing)

如果你在使用过程中遇到 Bug 或有新的功能想法（例如武器磨损系统、印花系统等），欢迎提交 [Issue](issues) 或发起 Pull Request。

*由 SANS 创作 & 维护 (Assisted by Gemini)*
