# Aurick Das — Academic Portfolio

Personal academic portfolio, live at **https://aurick165.github.io**

## How to deploy (one time)

1. On GitHub, create a new **public** repository named exactly:

   ```
   Aurick165.github.io
   ```

   (It must match your GitHub username — that's what makes GitHub serve it at the root URL.)

2. Push this folder to it:

   ```bash
   cd Aurick165.github.io
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/Aurick165/Aurick165.github.io.git
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages** → confirm Source is "Deploy from a branch", branch `main`, folder `/ (root)`.

4. Wait 1–2 minutes, then visit **https://aurick165.github.io**

## How to update the site

Edit `index.html` (all content is plain HTML — publications, research, etc. are clearly labeled sections), then:

```bash
git add . && git commit -m "Update content" && git push
```

The live site refreshes automatically within a minute or two.

## Notes

- No build step, no dependencies — a single static `index.html`.
- Fonts load from Google Fonts; everything else is self-contained.
- To add a CV: drop `cv.pdf` in this folder, push, and link to it with `<a href="cv.pdf">CV</a>`.
