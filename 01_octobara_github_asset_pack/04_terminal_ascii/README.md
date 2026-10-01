---
title: OctoBara 终端 ASCII 彩色启动横幅使用指南
version: v0.1
author: 胡嘉
date: 2026-09-22
---

# OctoBara 终端 ASCII 彩色启动横幅使用指南

## 版本
| 版本 | 日期 | 作者 | 改动点 |
| --- | --- | --- | --- |
| v0.1 | 2026-09-22 | 胡嘉 | 首版，提供 macOS/Linux 终端 ANSI TrueColor 极客启动屏脚本与配置方法 |

## 链接
- 库内：- 无
- 飞书：- 无

---

## 一、 脚本功能概览

`octobara.sh` 是一个专为 macOS / Linux 终端编写的高性能 Shell 启动脚本：
1. **ANSI TrueColor 高精度字符画**：采用现代终端半块字符（`▀` / `▄`），在仅 17 行的垂直空间内以 1:1 正方形点阵完美呈现 OctoBara（带蜜柑与触手）。
2. **实时系统与开发看板**：
   - 当前登录用户与机器名 (`User@Host`)
   - 操作系统与内核版本 (`macOS 26.x`)
   - 当前 Shell 与系统运行时间 (`Uptime`)
   - 智能 Git 仓库分支检测（如果在 Git 仓库内，显示当前所在分支并高亮）
3. **架构师禅定金句轮换**：每次打开终端随机抽取一条打工人与系统架构师金句。

---

## 二、 运行与体验

### 1. 手动直接运行
在终端中直接执行：
```bash
/Users/hujia/Desktop/Working/temp/octobara_asset_pack/04_terminal_ascii/octobara.sh
```

### 2. 配置为终端默认打开欢迎屏 (MOTD)
如果你希望每次打开 iTerm2、Terminal 或 VS Code 内置终端时都能看到这只可爱的 OctoBara，只需在 `~/.zshrc` 末尾添加一行：

```bash
echo 'source /Users/hujia/Desktop/Working/temp/octobara_asset_pack/04_terminal_ascii/octobara.sh' >> ~/.zshrc
```
保存后，新开任意终端窗口即可生效。
