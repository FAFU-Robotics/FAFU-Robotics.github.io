---
layout: page
title: 采摘机器人
description: 福农采摘伙伴 / FAFU PickMate，面向农林场景
img: assets/img/pickmate-zh.png
importance: 4
category: 当前工作
permalink: /projects/mobile-robot/
---

<style>
  .pickmate-logos { display: grid; gap: 1.25rem; margin: 0 0 1.5rem; }
  .pickmate-logos img { width: min(100%, 720px); height: auto; }
  .harvest-poster { margin: 0 0 1.5rem; }
  .harvest-poster img { width: min(100%, 960px); height: auto; display: block; }
  .harvest-poster figcaption { margin-top: 0.45rem; font-size: 0.95rem; }
</style>

<div class="pickmate-logos">
  <img src="{{ '/assets/img/pickmate-zh.png' | relative_url }}" alt="智能采摘机器人 福农采摘伙伴">
</div>

采摘机器人的名字是**福农采摘伙伴**（FAFU PickMate），面向果园等农林场景。当前平台是一辆移动小车，用来把激光感知、定位建图、路径规划和底盘控制接到同一辆车上。

<figure class="harvest-poster">
  <img src="{{ '/assets/img/harvest-platform.png' | relative_url }}" alt="果园自主采摘机器人，柑橘自主采摘研发样机">
  <figcaption>果园自主采摘机器人 / 柑橘自主采摘研发样机</figcaption>
</figure>

### 平台

| 部分 | 配置 |
| --- | --- |
| 移动底盘 | AgileX Bunker Mini 2.0 |
| 机器臂 | 自主研发的 6 轴[具身智能机器臂]({{ '/projects/embodied-arm/' | relative_url }})（[FAFU_station](https://github.com/FAFU-Robotics/FAFU_station)、[fafu_arm_sdk](https://github.com/FAFU-Robotics/fafu_arm_sdk)） |
| 激光雷达 | RoboSense Airy |
| 车载计算 | NVIDIA Jetson |
| 软件 | [WRSAgentOS](https://github.com/chenhaox/WRSAgentOS)、[WRS2](https://github.com/chenhaox/WRS2) |

### 演示视频

{% include demo_videos.liquid %}
