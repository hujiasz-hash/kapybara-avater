---
title: 卡皮巴拉（Capybara）全套设计资产库总指南
version: v1.1
author: 胡嘉
date: 2026-09-22
---

# 卡皮巴拉（Capybara）全套设计资产库总指南

## 版本
| 版本 | 日期 | 作者 | 改动点 |
| --- | --- | --- | --- |
| v1.0 | 2026-09-22 | 胡嘉 | 整合归档所有卡皮巴拉设计资产（GitHub 风格 OctoBara、像素桌宠、表情包、壁纸与头像） |
| v1.1 | 2026-09-22 | 胡嘉 | 扩充 OctoBara 头像至 12 款（新增代码审查、深夜极客、重构拆弹、AI魔法、智驾巡航、温泉放空） |
| v1.2 | 2026-10-01 | 胡嘉 | 新增 GitHub Invertocat 风格极简黑白头像（07 原版母本精简提纯、双模圆形徽章与多尺寸适配） |

## 链接
- 库内：- 无
- 飞书：- 无

---

## 一、 资产库统一目录架构

本目录统一归档胡老师所有关于**卡皮巴拉（Capybara / OctoBara）**的全部设计与美术资产，位于：  
📁 **绝对路径**：[`/Users/hujia/Desktop/Working/2026-09_capybara-design/`](file:///Users/hujia/Desktop/Working/2026-09_capybara-design/)  
*(同时支持快捷软链访问：[`/Users/hujia/Desktop/Working/capybara_design/`](file:///Users/hujia/Desktop/Working/capybara_design/))*

```
2026-09_capybara-design/
├── 01_octobara_github_asset_pack/   # GitHub 风格 OctoBara 完整开发者资源包 (Phase 1 ~ Phase 4)
│   ├── 01_master_mascot/            # 超清透明母本、贴纸母本、macOS Squircle 图标、微尺寸 Favicon
│   ├── 02_avatars/                  # 十二款高频研发状态头像矩阵 (多线程/心如止水/CPU烧了/架构师/在做了/准点下班/CR/夜猫/重构/AI/智驾/温泉)
│   ├── 03_animated_gifs/            # 轻量透明动图 (敲键盘/禅定呼吸/宕机发抖，微信/飞书规范)
│   ├── 04_terminal_ascii/           # macOS 终端 ANSI TrueColor 彩色启动屏脚本 (octobara.sh)
│   ├── 05_readme_and_stickers/      # GitHub Profile 动态模板与 A4 实体贴纸切模打印版
│   └── 06_minimal_github_avatars/   # GitHub Invertocat 极简黑白头像矩阵（原版母本提纯、双模徽章、多尺寸适配）
│
├── 02_github_concept_explorations/  # GitHub 风格三大方向设计探索原稿
│   ├── 01_方向一_极简单色剪影_InvertoCapy.jpg
│   ├── 02_方向二_跨界章鱼水豚_OctoBara.jpg
│   └── 03_方向三_macOS现代极客App图标.jpg
│
├── 03_pixel_desktop_pet/            # 原版像素桌宠资产（对接 kapybara-buddy 应用）
│   ├── 00_像素桌宠_动作表一_基础视线.png
│   ├── 00_像素桌宠_动作表二_打工与互动.png
│   ├── 00_像素桌宠_动作表三_萌态与技能.png
│   ├── animation_frames/            # 147 帧归一化动作分解序列帧
│   ├── 桌宠动图_*.gif               # 桌面宠物三组动作预览动图
│   └── 01 ~ 18 透明/带底动作单图    # 基础正视、踱步、打盹、敲键盘、泡温泉、吃橘子等 18 套动作
│
├── 04_emoji_pack/                   # 打工人「佛系与发疯」全套 15 款表情包
│   ├── raw_emojis/                  # 纯图版（在做了、收到、咖啡续命、精神状态良好等）
│   ├── with_text/                   # 气球软糖胖胖体带字版表情包
│   └── raw_emojis/fonts/            # 表情包配套设计字体
│
└── 05_avatars_and_wallpapers/       # 头像与壁纸库
    ├── 头像_01_清新抹茶薄荷绿.jpg   # 荷叶水豚圆形徽章头像
    └── capybara_wallpapers/         # 8 款多主题高清桌面壁纸
```

---

## 二、 核心项目关联索引

1. **桌宠软件实现工程**：
   - 目录：[`/Users/hujia/Desktop/Working/2026-09_kapybara-buddy/`](file:///Users/hujia/Desktop/Working/2026-09_kapybara-buddy/)
   - 说明：Tauri + AI 浮窗桌面伴侣，核心动画直接引用 `03_pixel_desktop_pet/` 中的像素动作帧。
2. **总交付技术报告**：
   - 报告：[20260922_OctoBara极客开发者全套资源包设计与交付报告.md](file:///Users/hujia/Desktop/Working/2026-09_capybara-design/20260922_OctoBara极客开发者全套资源包设计与交付报告.md)
   - 记录了从像素风水豚到 GitHub OctoBara 的推导过程、响应式 LOD 图标设计体系与技术指标。
