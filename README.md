# Martin Yuan — Personal Website

A warm, lightweight academic portfolio for Zhaorun (Martin) Yuan. Built with semantic HTML, CSS, and a small amount of vanilla JavaScript. No build step, package installation, API keys, or runtime services are required.

## 本地预览

在此文件夹运行：

```sh
python3 -m http.server 8000
```

浏览器打开 `http://localhost:8000`。也可以直接打开 `index.html`。

## GitHub Pages 部署

1. 将本目录的文件提交并推送到 `martinnnYuan/Martin_Personal_Web` 的 `main` 分支。
2. 在仓库 **Settings → Pages → Build and deployment → Source** 中选择 **GitHub Actions**。
3. 在 **Actions** 中运行 **Deploy portfolio to GitHub Pages**（或再次推送 main）。
4. 工作流成功后，网站地址为：`https://martinnnyuan.github.io/Martin_Personal_Web/`。

所有本地资源使用相对路径，同时适用于项目子路径和用户主页根目录。无需修改现有的 `martinnnYuan.github.io` 仓库。工作流仅发布页面和 assets，不会发布 README、编辑器设置或原始研究材料。

也可使用无工作流部署：Settings → Pages → Deploy from a branch → main / (root)。两种方式任选一种。

## 内容维护

- `index.html`：英文简介、研究兴趣、Alynna、项目、经历和联系信息。
- `styles.css`：奶油色、植物绿和陶土色视觉；桌面、平板和手机布局；减少动态效果与打印适配。
- `script.js`：移动菜单、项目筛选、当前章节提示与页脚年份。
- `assets/`：Alynna 官方图片、Seattle 项目截图和 SVG favicon。
- `.github/workflows/pages.yml`：GitHub Pages 自动部署。

添加项目时，在 `.projects` 中添加一个 `.project`，设置 `data-category="mobility"`、`environment` 或 `data`（可使用空格组合）。项目筛选仅影响 Further Explorations；Alynna 始终显示。

## 内容依据与编辑边界

内容根据用户提供的英文简历与 Mindful Mobility research proposal 整理，并核对公开 GitHub 仓库和 Alynna App Store。提炼研究兴趣，未公开 proposal 全文、研究招募细节、个人住址、电话号码或原始简历文件。研究构想与已完成项目在文案中分别标明。

GitHub 仓库核查（2026-11-13）：

- `alynna_support`：并入 Alynna 专题，提供产品网站链接。
- `geog328_traffic_incident`：独立展示，注明团队项目。
- `mapboxtest`：列为小型地图标记实验。
- `martinnnYuan.github.io`：列为早期个人网站。
- `Martin_Personal_Web`：本站，无需重复列为另一个项目。
- 名称含 lab 的仓库已排除；`geog458_us_covid_map` 的 README 明确标注 **GEOG 458 Lab 03**，因此也排除。
- 其他简历项目可以阅读站内说明；没有验证的公开链接不添加假链接。

学术措辞保留方法边界：公交站点密度是可达性代理指标，Mindful Mobility 是研究方向，Alynna 不主张已验证的治疗效果。

## 图片来源

- Alynna 官方 App Store 图片与图标：<https://apps.apple.com/us/app/alynna/id6755222294>，© Locaphilia LLC。由 Apple 的公开产品数据接口获取，存储于本地以避免运行时依赖。
- Seattle 交通地图截图：用户的 <https://github.com/martinnnYuan/geog328_traffic_incident>，由该仓库 `assets/screenshot_mappage.png` 获取。
- 其余插画为本站 SVG/CSS 概念性视觉，不代表真实分析结果，项目配图已作标识。
