# Kedar Chashtve — Portfolio

A single-page portfolio site for a Digital Marketing & Social Media Specialist.

## Folder structure
```
portfolio/
├── index.html
├── style.css
├── script.js
└── assets/
    ├── resume.pdf     ← add your real resume here
    └── profile.jpg    ← optional, not yet wired into the HTML
```

## Before you upload
1. Drop your actual **resume.pdf** into the `assets` folder — the download button on the hero section points to `assets/resume.pdf`, so the link will be broken until that file exists.
2. If you want a profile photo, add `profile.jpg` to `assets` and tell me — right now the HTML doesn't display it anywhere, it's just sitting in the folder.

## Get a live link with GitHub Pages (free, no extra setup)

1. Go to [github.com](https://github.com) and create a new repository (e.g. `portfolio`). Keep it **Public**.
2. Upload all the files from this folder (`index.html`, `style.css`, `script.js`, and the `assets` folder with your resume inside) — either drag-and-drop them in the GitHub web UI ("Add file" → "Upload files"), or via git:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/portfolio.git
   git push -u origin main
   ```
3. In the repository, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch", choose branch **main** and folder **/ (root)**, then click **Save**.
5. Wait a minute or two and refresh the page — GitHub will show your live URL, typically:
   ```
   https://YOUR_USERNAME.github.io/portfolio/
   ```

That link is permanent and updates automatically every time you push new commits to `main`.

## What was changed from your original code
- Added a `<meta name="description">` tag for better search/link previews.
- Added a mobile-responsive media query block at the bottom of `style.css` — the original had fixed large font sizes (e.g. `70px` h1) with no scaling for phones/tablets, which would overflow small screens.
- Everything else (loader, hero, blobs, skills cards, contact section) is unchanged from what you wrote.
