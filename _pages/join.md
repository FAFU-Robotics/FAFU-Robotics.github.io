---
layout: page
permalink: /join/
title: 加入
description: 招生、实习与合作
nav: true
nav_order: 6
---

**{{ site.data.lab.name_zh }}** 欢迎对移动机器人、激光感知、导航规划或机械臂感兴趣的同学。名额和截止日期以负责人回复为准。

## 我们在找什么样的人

- 研究生：有机器人、计算机、自动化、机械或相关背景
- 本科生 / 实习生：能稳定投入，愿意把实验和代码做到别人能复现
- 合作者：已有明确课题或设备，希望一起做

## 申请时请发送

1. 简历（PDF）
2. 成绩单，或一份能代表你的项目、论文、代码
3. 一段不超过一页的说明：你想做什么，为什么适合这个团队

邮件标题建议：`申请-博士/硕士/实习-姓名`

{% if site.data.lab.email and site.data.lab.email != "" %}
邮箱：`{{ site.data.lab.email }}`
{% else %}
公开邮箱还没填。确定后会出现在这里，也会出现在首页。
{% endif %}

## 合作

校内外课题组或产业界如果想合作，请说明目标和时间。{% if site.data.lab.pi and site.data.lab.pi != "" %}联系人：{{ site.data.lab.pi }}。{% endif %}
