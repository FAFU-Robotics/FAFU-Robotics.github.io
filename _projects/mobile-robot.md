---
layout: page
title: 采摘机器人
description: 面向农林场景的采摘机器人，含移动底盘的建图、定位与绕障
img: assets/img/mobile-robot.svg
importance: 4
category: 当前工作
permalink: /projects/mobile-robot/
---

这个方向研发采摘机器人，面向果园等农林场景。当前平台是一辆移动小车，用来把激光感知、定位建图、路径规划和底盘控制接到同一辆车上。

底盘是 AgileX Bunker Mini 2.0，激光雷达是 RoboSense Airy，计算在 Jetson 工控机上，软件基于 ROS 2 Humble。

### 平台

| 部分 | 配置 |
| --- | --- |
| 移动底盘 | AgileX Bunker Mini 2.0 |
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
