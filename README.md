# AFSA organization website

Bilingual landing page for **AFSA — Smart Agriculture** (editorial / magazine style, aligned with the in-app Bloom login aesthetic).

## Live site

**https://ai-for-smart-agriculture.github.io/**

- English default; **中文** toggle in the header  
- Hero image carousel  
- **Download (China)** → Gitee `yhlkxkzs/afsa-android-release`  
- **Download (International)** → `ai-for-smart-agriculture/afsa-android-releases` on GitHub  

---

## Deploy

Hosted on the org repo **`ai-for-smart-agriculture.github.io`** (GitHub Pages).

From the monorepo root:

```bash
python scripts/deploy_org_website.py
```

This copies `afsa-org-website/index.html` and `.nojekyll`, pushes to the Pages repo, and triggers a Pages rebuild.

Manual steps (first time):

1. Create public repo **`ai-for-smart-agriculture.github.io`** under the org  
2. Settings → Pages → Branch **main** → Folder **/ (root)**  

---

## Files

| File | Purpose |
|------|---------|
| `index.html` | Single-page site (HTML + CSS + JS) |
| `.nojekyll` | Disable Jekyll on GitHub Pages |

Optional: add `assets/hero.jpg` and point `.cover` background to your own photography.

---

## Related links

| | URL |
|---|---|
| App source | https://github.com/ai-agriculture-circuits-and-systems/app_v1 |
| Intl. APK mirror | https://github.com/ai-for-smart-agriculture/afsa-android-releases/releases |
| China APK mirror | https://gitee.com/yhlkxkzs/afsa-android-release/releases |
