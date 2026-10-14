---
layout: page
title: 移动小车
description: 激光雷达建图、定位与自主绕障
img: assets/img/mobile-robot.svg
importance: 1
category: 移动机器人
permalink: /projects/mobile-robot/
---

移动小车是团队的室内移动机器人平台，用来把激光感知、定位建图、路径规划和底盘控制接到同一辆车上。

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
