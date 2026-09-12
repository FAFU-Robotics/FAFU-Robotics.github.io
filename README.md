# Your Lab

实验室主页基础模板。运行时来自 [al-folio](https://github.com/alshedivat/al-folio)，本仓库只保留课题组会改的内容。

导航：**研究 · 论文 · 成员 · 新闻 · 加入**

## 目录

```text
_config.yml              站点名、网址、功能开关
_data/lab.yml            实验室名称、负责人、邮箱、地址
_data/socials.yml        邮箱 / Scholar / GitHub 图标
_pages/about.md          首页
_pages/projects.md        研究列表
_pages/publications.md   论文页
_pages/profiles.md        成员页结构
_pages/people_*.md       每位成员简介
_pages/news.md           新闻页
_pages/join.md           招生页
_projects/               每个研究方向一篇
_bibliography/papers.bib 论文（BibTeX）
_news/                   新闻（按日期命名）
assets/img/              头像和研究配图
```

## 改内容先动这些

1. `_config.yml`：`title`、`url`、`baseurl`
2. `_data/lab.yml`：实验室名、PI、邮箱、地址
3. `_data/socials.yml`：联系方式图标
4. `_pages/people_*.md` 和 `_pages/profiles.md`：成员
5. `_projects/`：研究方向
6. `_bibliography/papers.bib`：论文
7. `_news/`：新闻
8. `assets/img/prof_pic.jpg`：头像

仓库名是 `FAFU-Robotics.github.io` 时：

```yaml
url: https://fafu-robotics.github.io
baseurl: ""
```

本地预览地址：http://localhost:8080/

## 本地预览

Docker Desktop 启动后，在本目录执行：

```powershell
docker compose up --build --pull never
```

浏览器打开：http://localhost:8080/

改文件后如果页面没刷新，执行 `docker compose restart`。

## 发布

仓库 **Settings → Pages → Build and deployment → Source** 选 **GitHub Actions**（不要选 Deploy from a branch）。

网站地址：https://fafu-robotics.github.io/
