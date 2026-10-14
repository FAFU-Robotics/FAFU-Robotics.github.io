---
layout: page
title: 竞赛
permalink: /competitions/
description: 学生竞赛
nav: true
nav_order: 4
---

<style>
  .comp-list {
    max-width: 930px;
    display: flex;
    flex-direction: column;
    gap: 0.9rem;
    margin: 0.1rem 0 1rem;
  }
  .comp-card {
    border: 1px solid var(--global-divider-color);
    border-radius: 10px;
    background: color-mix(in srgb, var(--global-text-color) 4%, var(--global-card-bg-color));
    padding: 0.85rem 1rem 0.9rem;
  }
  .comp-head {
    display: flex;
    align-items: baseline;
    justify-content: space-between;
    column-gap: 1.25rem;
    margin: 0 0 0.6rem;
    padding-bottom: 0.5rem;
    border-bottom: 1px solid var(--global-divider-color);
  }
  .comp-card .comp-title {
    margin: 0;
    flex: 1 1 auto;
    min-width: 0;
    font-size: 1.12rem;
    font-weight: 650;
    line-height: 1.4;
  }
  .comp-date {
    flex: 0 0 auto;
    margin: 0;
    font-size: 0.92rem;
    font-weight: 500;
    line-height: 1.4;
    color: var(--global-text-color-light);
    white-space: nowrap;
  }
  .comp-fields {
    margin: 0;
    display: flex;
    flex-direction: column;
    gap: 0.32rem;
  }
  .comp-row {
    display: grid;
    grid-template-columns: 5.5rem minmax(0, 1fr);
    column-gap: 0.75rem;
    align-items: baseline;
  }
  .comp-fields dt {
    margin: 0;
    font-size: 0.9rem;
    font-weight: 600;
    line-height: 1.45;
    color: var(--global-text-color-light);
  }
  .comp-fields dd {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.45;
    overflow-wrap: anywhere;
  }
  .comp-photo {
    margin: 0.7rem 0 0;
  }
  .comp-photo img {
    width: min(100%, 420px);
    height: 240px;
    object-fit: cover;
    object-position: center;
    display: block;
    border-radius: 6px;
  }
  @media (max-width: 640px) {
    .comp-card {
      padding: 0.8rem 0.8rem 0.85rem;
    }
    .comp-head {
      column-gap: 0.7rem;
    }
    .comp-card .comp-title {
      font-size: 1.05rem;
    }
    .comp-row {
      grid-template-columns: 1fr;
      row-gap: 0.04rem;
    }
    .comp-fields {
      gap: 0.5rem;
    }
  }
</style>

<div class="comp-list">
  <article class="comp-card">
    <header class="comp-head">
      <h2 class="comp-title">仿真驱动的自研 LRMate 200iD 多方块拣选-堆放系统</h2>
      <p class="comp-date">2026.8</p>
    </header>
    <dl class="comp-fields">
      <div class="comp-row">
        <dt>赛事名称</dt>
        <dd>第二十八届中国机器人与人工智能大赛</dd>
      </div>
      <div class="comp-row">
        <dt>赛事类型</dt>
        <dd>机器人任务挑战赛 · 挑战赛</dd>
      </div>
      <div class="comp-row">
        <dt>名次</dt>
        <dd>全国三等奖、福建省二等奖</dd>
      </div>
      <div class="comp-row">
        <dt>参赛人</dt>
        <dd>张熙、俞泺佳、李昕瑜</dd>
      </div>
    </dl>
    <figure class="comp-photo">
      <img src="{{ '/assets/img/competition-lrmate.png' | relative_url }}" alt="仿真驱动的自研 LRMate 200iD 多方块拣选-堆放系统，黄色 FANUC 机械臂在竞赛场地中">
    </figure>
  </article>

  <article class="comp-card">
    <header class="comp-head">
      <h2 class="comp-title">具身智控无针注射机器人：基于视觉混合伺服的动态畜牧免疫系统</h2>
      <p class="comp-date">2026.7</p>
    </header>
    <dl class="comp-fields">
      <div class="comp-row">
        <dt>赛事名称</dt>
        <dd>第二十八届中国机器人与人工智能大赛</dd>
      </div>
      <div class="comp-row">
        <dt>赛事类型</dt>
        <dd>机器人任务挑战赛 · 创新赛</dd>
      </div>
      <div class="comp-row">
        <dt>名次</dt>
        <dd>全国二等奖、福建省一等奖</dd>
      </div>
      <div class="comp-row">
        <dt>参赛人</dt>
        <dd>张熙、胡晗颖、李伟鹏</dd>
      </div>
    </dl>
    <figure class="comp-photo">
      <img src="{{ '/assets/img/competition-injection.png' | relative_url }}" alt="具身智控无针注射机器人的视觉-力学混合伺服演示，机器人末端对准猪只标记">
    </figure>
  </article>

  <article class="comp-card">
    <header class="comp-head">
      <h2 class="comp-title">轻量级双臂具身操作系统：RDK-S100 端侧 VLA 模型</h2>
      <p class="comp-date">2025.10</p>
    </header>
    <dl class="comp-fields">
      <div class="comp-row">
        <dt>赛事名称</dt>
        <dd>第十九届「挑战杯」全国大学生学术科技竞赛</dd>
      </div>
      <div class="comp-row">
        <dt>赛事类型</dt>
        <dd>人工智能挑战赛</dd>
      </div>
      <div class="comp-row">
        <dt>名次</dt>
        <dd>特等奖</dd>
      </div>
      <div class="comp-row">
        <dt>参赛人</dt>
        <dd>张熙、王溢宁、罗锦皓、丘滨辉、康泽坤</dd>
      </div>
    </dl>
    <figure class="comp-photo">
      <img src="{{ '/assets/img/competition-challenge-cup.png' | relative_url }}" alt="轻量级双臂具身操作系统：RDK-S100 端侧 VLA 模型，学生在第十九届「挑战杯」5 号讲台前">
    </figure>
  </article>
</div>

指导教师：[陈昊](https://chenhao.info)
