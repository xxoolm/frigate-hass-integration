<!-- markdownlint-disable first-line-heading -->
<!-- markdownlint-disable no-inline-html -->

<img src="https://raw.githubusercontent.com/blakeblackshear/frigate-hass-integration/master/images/frigate.png"
     alt="Frigate icon"
     width="35%"
     align="right"
     style="float: right; margin: 10px 0px 20px 20px;" />

[![GitHub Release](https://img.shields.io/github/release/blakeblackshear/frigate-hass-integration.svg?style=flat-square)](https://github.com/blakeblackshear/frigate-hass-integration/releases)
[![Build Status](https://img.shields.io/github/actions/workflow/status/blakeblackshear/frigate-hass-integration/build.yaml?branch=master&style=flat-square)](https://github.com/blakeblackshear/frigate-hass-integration/actions/workflows/build.yaml)
[![Test Coverage](https://img.shields.io/codecov/c/gh/blakeblackshear/frigate-hass-integration?style=flat-square)](https://app.codecov.io/gh/blakeblackshear/frigate-hass-integration/)
[![License](https://img.shields.io/github/license/blakeblackshear/frigate-hass-integration.svg?style=flat-square)](LICENSE)
[![hacs](https://img.shields.io/badge/HACS-default-orange.svg?style=flat-square)](https://hacs.xyz)

# Frigate Home Assistant 集成（中文增强版）

本仓库是在上游项目基础上的中文增强版本，面向简体中文用户进行了实体名称、单位与日志的在地化。核心功能保持与上游一致。本中文版本所在分支：`frigate-hass-integration-zh`。

**项目特点**

- 丰富的媒体浏览器（带缩略图与层级导航）
- 传感器实体：相机/检测/进程/跳帧等 FPS、对象数量、活动数量、声音强度、运行状态与时间等
- 二进制传感器：对象占用、声音触发、运动等
- 相机实体：实时流与最近检测对象快照
- 开关实体：录制、检测、快照、对比度增强
- 服务：手动事件、PTZ 控制、录像导出等
- 支持多 Frigate 实例

## 安装（与上游一致）

Easiest install is via [HACS](https://hacs.xyz/):

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=blakeblackshear&repository=frigate-hass-integration&category=integration)

`HACS -> Integrations -> Explore & Add Repositories -> Frigate`

注意：

- HACS 仅负责安装，不会自动“配置”集成。安装完成后需前往 `设置 > 集成` 添加 Frigate。
- 需先安装并配置 `mqtt` 集成（其为 Frigate 工作所必需，且需手动配置）。

进阶用户的手动安装方式：将 `custom_components/frigate` 复制到 Home Assistant 的
`custom_components` 目录下。

完整安装与使用说明请参阅上游的 [Frigate 文档](https://docs.frigate.video/integrations/home-assistant/)。

### Media Browsing

请在 Home Assistant 中启用 [media_source](https://www.home-assistant.io/integrations/media_source/) 以显示媒体浏览器。

### Lovelace Card

你也可以搭配使用 [Frigate Lovelace 卡片](https://github.com/dermotduffy/frigate-hass-card)。

<img src="https://raw.githubusercontent.com/blakeblackshear/frigate-hass-integration/master/images/lovelace-card.png">

## 文档

完整用法请参阅 [Frigate 官方文档](https://docs.frigate.video/integrations/home-assistant/)。

## 原作者与版权声明

- 本项目基于上游开源仓库 `blakeblackshear/frigate-hass-integration` 进行中文增强与本地化改动。
- 原作者：Blake Blackshear（以及维护者见下）
- 版权与许可：沿用上游的 MIT License（见本仓库 `LICENSE`）。在再发布或分发时，请保留原版权与许可声明。

## 维护者（上游项目）

## 维护者（上游）

- [Blake Blackshear](https://github.com/blakeblackshear/)
- [Dermot Duffy](https://github.com/dermotduffy/)
- [Nick Mowan](https://github.com/NickM-27)

## 使用 AI 的说明

- 本中文增强版在改写文案时借助了 AI 辅助翻译与审校工具；所有更改均由维护者人工复核，确保不影响功能与 API。
- 若你在生产环境中使用，请自行评估与测试；如发现翻译歧义、术语不一致或影响使用的情况，欢迎提交 Issue/PR。
