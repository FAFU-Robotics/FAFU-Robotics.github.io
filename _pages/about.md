---
layout: about
title: About
permalink: /
subtitle: Robotic Perception and Manipulation

profile:
  align: right
  more_info: >
    <p><a href="https://chenhao.info">陈昊</a> · 副教授</p>
    <p>课题组负责人</p>
    <p><a href="/people/">成员介绍</a></p>
    <p><a href="https://github.com/FAFU-Robotics">GitHub</a></p>

selected_papers: false
social: true

announcements:
  enabled: true
  scrollable: true
  limit: 5

latest_posts:
  enabled: false
---

**{{ site.data.lab.name_zh }}**由[陈昊](https://chenhao.info)副教授负责，隶属于{{ site.data.lab.institution }}**{{ site.data.lab.parent_team }}**，依托{{ site.data.lab.affiliation }}。

### 在研课题

<style>
  .research-grid {
    clear: both;
    display: grid;
    grid-template-columns: 1fr;
    gap: 1rem;
    margin: 0.25rem 0 1rem;
  }
  .research-grid .col {
    width: auto;
    max-width: none;
    min-width: 0;
  }
  .research-grid a {
    color: inherit;
    text-decoration: none;
  }
  .research-grid .card-text {
    color: var(--global-text-color-light);
  }
  .research-grid .card-title {
    font-size: 1.15rem;
    font-weight: 650;
    line-height: 1.35;
    margin-bottom: 0.4rem;
  }
  .research-grid .card-img-top {
    height: 148px;
    object-fit: contain;
    background: color-mix(in srgb, var(--global-text-color) 4%, var(--global-card-bg-color));
  }
  @media (min-width: 768px) {
    .research-grid {
      grid-template-columns: repeat(3, minmax(0, 1fr));
    }
  }
</style>

<div class="research-grid">
{% assign featured = "mobile-robot,embodied-arm,robot-manipulation" | split: "," %}
{% for slug in featured %}
  {% assign project = site.projects | where: "slug", slug | first %}
  {% include projects.liquid %}
{% endfor %}
</div>

其余课题见 [项目]({{ '/projects/' | relative_url }})。

### 加入

想参与这些课题的同学，请看 [加入]({{ '/join/' | relative_url }})，邮件联系[陈昊](https://chenhao.info)。
