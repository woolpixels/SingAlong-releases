# 一起唱 · SingAlong

macOS 桌面悬浮歌词工具。自动识别 Apple Music 与 Spotify 正在播放的歌曲，把同步歌词放在桌面上，跟随播放进度逐行滚动。无需账号，无需配置。

[![Latest release](https://img.shields.io/github/v/release/woolpixels/SingAlong-releases?label=release)](https://github.com/woolpixels/SingAlong-releases/releases/latest)
![Platform](https://img.shields.io/badge/platform-macOS%2013%2B-lightgrey)
![Players](https://img.shields.io/badge/Apple%20Music%20%7C%20Spotify-supported-brightgreen)

> 本仓库仅用于分发安装包与发布说明，不包含源代码。

## 目录

- [功能特性](#功能特性)
- [系统要求](#系统要求)
- [下载与安装](#下载与安装)
- [使用方法](#使用方法)
- [设置说明](#设置说明)
- [隐私说明](#隐私说明)
- [常见问题](#常见问题)
- [更新日志](#更新日志)
- [关于](#关于)
- [致谢](#致谢)

## 功能特性

- **悬浮歌词**：无边框窗口，随播放进度逐行高亮；小 / 中 / 大三档尺寸，可自由拖动，支持透明背景与一键回到屏幕中央。
- **自动识别**：读取 Apple Music / Spotify 当前的歌曲、歌手、播放进度与播放状态；歌词通过 [LRCLIB](https://lrclib.net/) 自动匹配，无需 API Key。
- **状态栏歌词**：可在菜单栏图标旁同步显示当前正在唱的一句，不需要时可关闭。
- **外观与主题色**：深色 / 浅色 / 跟随系统；高亮歌词颜色可选默认、红、橙、黄、绿、蓝、紫或跟随系统强调色。
- **启动行为**：可选「默认状态启动」或「继续上次的位置与状态」。
- **开机自动启动**：在菜单栏中一键开关。
- **每日播放记录**：记录当天完整播放完的歌曲（歌名、歌手、专辑、播放次数、累计听歌时长），并生成「今日歌词精选」。

## 系统要求

| 项目 | 要求 |
| --- | --- |
| 操作系统 | macOS 13 或更高版本 |
| 播放器 | Apple Music、Spotify |
| 网络 | 匹配歌词时需要联网 |

## 下载与安装

1. 前往 [Releases](https://github.com/woolpixels/SingAlong-releases/releases/latest) 下载最新版安装包（`.zip`）。
2. 解压后将「一起唱.app」拖入「应用程序」文件夹。
3. 首次运行时，macOS 会请求「自动化」权限，用于读取 Apple Music / Spotify 的当前播放信息，请选择**允许**。

## 使用方法

1. 打开「一起唱」，菜单栏会出现其图标。
2. 播放 Apple Music 或 Spotify 中的歌曲。
3. 匹配到同步歌词后，悬浮窗会开始随播放滚动。
4. 其他设置均可从菜单栏图标中调整。

## 设置说明

### 启动时

| 选项 | 行为 |
| --- | --- |
| 默认状态启动（默认） | 每次打开时关闭点击穿透、显示背景，并回到默认位置，避免窗口「看不见也点不到」。 |
| 继续上次的位置与状态 | 恢复上次退出时的窗口位置、点击穿透与透明背景状态。 |

悬浮窗位置会持续保存在本机，随时可通过菜单栏的「回到屏幕中央」找回窗口。

### 每日播放记录

- 仅记录完整播放完的歌曲，中途跳过的不计入。
- 记录保存在本机，不会上传。

## 隐私说明

一起唱不需要账号，也不会收集或上传个人数据。

- 不上传你的音乐文件，不在云端保存音乐内容。
- 播放信息仅用于歌词匹配与本地显示。
- 播放记录与当前歌词快照仅写入本机。
- 歌词匹配时，会向 LRCLIB 发送歌曲信息（歌名、歌手等）用于查询。

## 常见问题

**启动后看不到歌词窗口？**
从菜单栏选择「回到屏幕中央」；也可以将「启动时」设为「默认状态启动」。

**提示「找不到同步歌词」？**
歌词来自 LRCLIB，部分歌曲暂无同步歌词，此时会显示提示文案。

**没有识别到正在播放的歌曲？**
请确认已允许「一起唱」的「自动化」权限：系统设置 → 隐私与安全性 → 自动化。

**如何卸载？**
退出应用后，将「一起唱.app」移到废纸篓即可。如需清除本地数据，可删除 `~/Library/Application Support/SingAlong/`。

## 更新日志

完整版本记录见 [CHANGELOG.md](CHANGELOG.md)。

## 关于

| | |
| --- | --- |
| 应用 | 一起唱 · SingAlong |
| 当前版本 | v1.1.4 |
| 开发者 | Woolpixels |
| 官网 | [woolpixels.cc](https://woolpixels.cc/) |
| GitHub | [@woolpixels](https://github.com/woolpixels) |
| 小红书 | [Woolpixels](https://xhslink.cn/o/7EEkbW1Uyh8) |
| 邮箱 | odyssey.moment@outlook.com |

有任何问题或建议，欢迎随时联系。  
仅供个人学习与交流，请勿用于商业用途。

## 致谢

歌词数据来自 [LRCLIB](https://lrclib.net/)。

---

Copyright © 2026 Woolpixels
