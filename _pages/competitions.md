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
    gap: 1.15rem;
    margin: 0.15rem 0 1.15rem;
  }
  .comp-card {
    border: 1px solid var(--global-divider-color);
    border-radius: 10px;
    background: color-mix(in srgb, var(--global-text-color) 4%, var(--global-card-bg-color));
    padding: 1rem 1.15rem 1.05rem;
  }
  .comp-card .comp-title {
    margin: 0 0 0.8rem;
    padding-bottom: 0.7rem;
    border-bottom: 1px solid var(--global-divider-color);
    font-size: 1.2rem;
    font-weight: 600;
    line-height: 1.45;
  }
  .comp-fields {
    margin: 0;
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
  }
  .comp-row {
    display: grid;
    grid-template-columns: 5.5rem minmax(0, 1fr);
    column-gap: 0.85rem;
    align-items: baseline;
  }
  .comp-fields dt {
    margin: 0;
    font-size: 0.92rem;
    font-weight: 600;
    line-height: 1.5;
    color: var(--global-text-color-light);
  }
  .comp-fields dd {
    margin: 0;
    font-size: 1rem;
    line-height: 1.55;
    overflow-wrap: anywhere;
  }
  .comp-photo {
    margin: 0.95rem 0 0.1rem;
  }
  .comp-photo img {
    width: min(100%, 840px);
    height: auto;
    display: block;
    border-radius: 6px;
  }
  .comp-photo figcaption {
    margin-top: 0.45rem;
    font-size: 0.92rem;
    line-height: 1.45;
    color: var(--global-text-color-light);
  }
  @media (max-width: 640px) {
    .comp-card {
      padding: 0.9rem 0.85rem 0.95rem;
    }
    .comp-row {
      grid-template-columns: 1fr;
      row-gap: 0.08rem;
    }
    .comp-fields {
      gap: 0.7rem;
    }
  }
</style>

<div class="comp-list">
  <article class="comp-card">
    <h2 class="comp-title">轻量级双臂具身操作系统：RDK-S100 端侧 VLA 模型</h2>
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
      <figcaption>第十九届「挑战杯」</figcaption>
    </figure>
  </article>

  <article class="comp-card">
    <h2 class="comp-title">具身智控无针注射机器人：基于视觉混合伺服的动态畜牧免疫系统</h2>
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
  </article>

  <article class="comp-card">
    <h2 class="comp-title">仿真驱动的自研 LRMate 200iD 多方块拣选-堆放系统</h2>
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
      <figcaption>仿真驱动的自研 LRMate 200iD 多方块拣选-堆放系统</figcaption>
    </figure>
  </article>
</div>

指导教师：[陈昊](https://chenhao.info)
