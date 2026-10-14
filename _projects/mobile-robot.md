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
  .harvest-real { margin: 1.25rem 0 1.5rem; }
  .harvest-real img { width: min(100%, 640px); height: auto; display: block; }
  .harvest-real figcaption { margin-top: 0.45rem; font-size: 0.95rem; }
</style>

<div class="pickmate-logos">
  <img src="{{ '/assets/img/pickmate-zh.png' | relative_url }}" alt="智能采摘机器人 福农采摘伙伴">
</div>

采摘机器人的名字是**福农采摘伙伴**（FAFU PickMate），面向果园等农林场景。当前平台是一辆移动小车，用来把激光感知、定位建图、路径规划和底盘控制接到同一辆车上。

底盘是 AgileX Bunker Mini 2.0，激光雷达是 RoboSense Airy，计算在 Jetson 工控机上，软件基于 ROS 2 Humble。

机器臂使用的是自主研发的 6 轴具身智能机器臂，项目页见 [具身智能机器臂]({{ '/projects/embodied-arm/' | relative_url }})，公开代码在 [FAFU_station](https://github.com/FAFU-Robotics/FAFU_station) 和 [fafu_arm_sdk](https://github.com/FAFU-Robotics/fafu_arm_sdk)。

<figure class="harvest-real">
  <img src="{{ '/assets/img/harvest-robot-real.png' | relative_url }}" alt="采摘机器人真实样机，履带底盘与绿色六轴机械臂">
  <figcaption>真实样机</figcaption>
</figure>

### 平台

| 部分 | 配置 |
| --- | --- |
| 移动底盘 | AgileX Bunker Mini 2.0 |
| 机器臂 | 自主研发的 6 轴[具身智能机器臂]({{ '/projects/embodied-arm/' | relative_url }}) |
| 激光雷达 | RoboSense Airy |
| 车载计算 | NVIDIA Jetson |
| 软件 | ROS 2 Humble |

### 车上在跑的能力

- 读取激光点云，做建图和定位
- 把点云投成二维占用栅格
- 在栅格上规划路径，并驱动底盘绕开障碍

公开的底盘与雷达控制代码在 [chassis_lidar_driver](https://github.com/FAFU-Robotics/chassis_lidar_driver)。

### 演示视频

{% include demo_videos.liquid %}
