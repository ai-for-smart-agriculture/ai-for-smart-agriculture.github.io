# AFSA 组织官网 · 艺术杂志风

部署在 **`ai-for-smart-agriculture`** 组织下的 GitHub Pages 介绍页。

视觉与 App 内「编辑部 / Bloom 登录」一致：**柔光田园、杂志排版、衬线刊头、暖绿米白**。

## 上线

1. 在组织下新建仓库 **`ai-for-smart-agriculture.github.io`**（Public）
2. 推送本目录 `index.html`、`.nojekyll`、可选 `assets/` 自定义配图
3. Settings → Pages → Branch **main** → Folder **/ (root)**

访问：**https://ai-for-smart-agriculture.github.io/**

## 替换封面摄影（推荐）

当前封面使用 Unsplash 田园图作为占位。若与 App 素材统一，可将编辑部图（如 `brand_mist_orchard.jpg`）放入 `assets/hero.jpg`，并在 `index.html` 的 `.cover` 背景改为：

```css
url("assets/hero.jpg") center/cover no-repeat
```

## APK 下载

按钮指向 app_v1 最新 Release，发版后自动更新，无需改页面。
