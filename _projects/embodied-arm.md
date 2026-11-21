---
layout: page
title: 福农灵臂
description: FAFU Nimble，六自由度轻量化机械臂
img: assets/img/arm-logo.png
importance: 3
permalink: /projects/embodied-arm/
---

<style>
  .arm-logo { margin: 0 0 1.25rem; }
  .arm-logo img { width: min(100%, 720px); height: auto; background: #fff; }
  .arm-hero { margin: 0 0 1.5rem; }
  .arm-hero img { width: min(100%, 300px); height: auto; display: block; background: #fff; }
  .arm-hero figcaption { margin-top: 0.45rem; font-size: 0.95rem; }
  .arm-video {
    width: 100%;
    max-width: 960px;
    background: #111;
    border-radius: 8px;
  }
</style>

<div class="arm-logo">
  <img src="{{ '/assets/img/arm-logo.png' | relative_url }}" alt="福农灵臂">
</div>

**福农灵臂**（FAFU Nimble）是课题组自研的六自由度轻量化机械臂，装在[采摘机器人]({{ '/projects/mobile-robot/' | relative_url }})上。

<figure class="arm-hero">
  <img src="{{ '/assets/img/arm-hero.png' | relative_url }}" alt="福农灵臂样机">
  <figcaption>六自由度样机，末端是夹爪。</figcaption>
</figure>

### 样机

| 项目 | 参数 |
| --- | --- |
| 自由度 | 6 |
| 结构 | 轻量化串联臂 |
| 自重 | 约 3.75 kg |
| 关节峰值扭矩 | 最高 36 N·m |
| 末端最大速度 | 约 0.8 m/s |
| 重复定位精度 | ≤ ±1 mm |
| 工作电压 | 24 V |
| 通信 | FDCAN |

装到采摘机器人上时，末端是采摘执行器。

### 上位机

上位机是 [FAFU 机械臂站控](https://github.com/FAFU-Robotics/FAFU_station)，支持关节点动、笛卡尔点动、重力补偿拖动示教、作业程序编程和示教轨迹编辑，可连接真机或在仿真中运行。

<video class="arm-video" controls playsinline preload="metadata" poster="{{ '/assets/img/arm-station-poster.jpg' | relative_url }}">
  <source src="{{ '/assets/video/arm-station.mp4' | relative_url }}" type="video/mp4">
</video>

### 代码

- [FAFU_station](https://github.com/FAFU-Robotics/FAFU_station)
- [fafu_arm_sdk](https://github.com/FAFU-Robotics/fafu_arm_sdk)

真机动作见[校庆科技成果展上的自动做饭]({{ '/assets/video/arm-cooking-demo.mp4' | relative_url }})。
