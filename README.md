# Oikos CoLiving — Landing Page

Single-file landing page (index.html) with all images embedded. No build step needed.

## Kerjain di Claude Code
Dari Terminal:
```bash
cd oikos-landing-project
claude            # buka Claude Code di folder ini
```

## Push ke GitHub
```bash
git init
git add .
git commit -m "Oikos landing page"
gh repo create oikos-landing --public --source=. --push
```

## Deploy ke Netlify
Pilih salah satu:

**A. Netlify CLI (paling cepat dari terminal)**
```bash
npm i -g netlify-cli
netlify login          # sekali saja, buka browser
netlify deploy --prod  # pilih "Create & configure a new site"
```
Setelah selesai, URL live muncul (mis. https://oikoscoliving.netlify.app).

**B. Netlify + GitHub (auto-deploy tiap push)**
1. app.netlify.com → Add new site → Import from GitHub → pilih repo `oikos-landing`.
2. Publish directory: `.`  → Deploy.
3. Tiap `git push`, Netlify auto-deploy.

## Update konten
Edit `index.html` (atau minta Claude Code), commit, push → live otomatis (opsi B) atau `netlify deploy --prod` (opsi A).
