# AFSA organization website

Bilingual landing page for **AFSA — Smart Agriculture** (editorial / magazine style, aligned with the in-app Bloom login aesthetic).

## Live site

**https://ai-for-smart-agriculture.github.io/**

- English default; **中文** toggle in the header  
- Hero image carousel  
- **Download** — Mainland China IPs → [Gitee APK](https://gitee.com/yhlkxkzs/afsa-android-release/releases/download/v1.1.2/AFSA.apk); others → [GitHub public mirror APK](https://github.com/ai-for-smart-agriculture/afsa-android-releases/releases/download/v1.1.2/AFSA.apk) (no login). Geo IP via ipapi.co / ipinfo.io; GitHub probe timeout falls back to Gitee.  

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
| `assets/hero/*.jpg` | Hero carousel backgrounds (bundled; no external CDN) |
| `.nojekyll` | Disable Jekyll on GitHub Pages |

Optional: add `assets/hero.jpg` and point `.cover` background to your own photography.

---

## Related links

| | URL |
|---|---|
| App source | https://github.com/ai-agriculture-circuits-and-systems/app_v1 |
| Intl. APK mirror | https://github.com/ai-for-smart-agriculture/afsa-android-releases/releases |
| China APK mirror | https://gitee.com/yhlkxkzs/afsa-android-release/releases |
