# GitHub Portfolio — Setup & GitHub Pages Instructions

This package contains both a **GitHub README** (`README.md`) and a **static website** (`index.html`) — they share the same content and the same `assets/` folder. Upload everything as-is and follow the steps below.

## Package contents

```
gh_portfolio/
├── README.md              ← Renders when someone visits your GitHub repo
├── index.html             ← Renders as your live website via GitHub Pages
├── INSTRUCTIONS.md        ← This file
└── assets/
    ├── profile/           ← Your profile photo
    ├── certificates/      ← Employment certificates (PDFs + thumbnails)
    └── projects/          ← Per-project image folders (15 projects)
```

---

## Part 1 — Create the GitHub repository

For a **profile-level portfolio** (README shows on your main github.com profile):

1. Go to https://github.com/new
2. Name the repository **exactly the same as your GitHub username**
3. Make it **Public**
4. Do **NOT** check "Add README", "Add .gitignore", or "Choose a license" — keep it empty
5. Click **Create repository**

For a **project-style portfolio** (separate from your profile):
- Same as above, but name the repo whatever you like (e.g. `hardware-portfolio`)

## Part 2 — Upload everything

1. On the empty repo page, click **"uploading an existing file"**
2. Drag the **entire contents** of the unzipped `gh_portfolio/` folder into the upload area — that's the `README.md`, `index.html`, `INSTRUCTIONS.md`, and the `assets/` folder
3. Wait for everything to upload
4. Scroll down, commit message "Initial portfolio upload", click **Commit changes**

Once committed, your README is already live on the repo page.

---

## Part 3 — Enable GitHub Pages (your live website)

This is what turns `index.html` into a real website.

1. On your repo page, click the **Settings** tab (top-right of the repo page)
2. In the left sidebar, click **Pages**
3. Under "Build and deployment":
   - **Source:** *Deploy from a branch*
   - **Branch:** *main* (or *master*, whichever yours is) → **/ (root)**
4. Click **Save**
5. Wait ~30 seconds, then refresh the Pages settings screen
6. You'll see a banner: **"Your site is live at..."** with a URL

**Your live URL will be:**

- If you used your username as repo name → `https://<your-username>.github.io/`
- Otherwise → `https://<your-username>.github.io/<repo-name>/`

This is the URL to put on your resume.

---

## Part 4 — Updating content later

Whenever I send you an updated `README.md` or `index.html`:

1. Go to the file on GitHub → click the pencil icon to edit
2. Select everything (Ctrl+A) → delete
3. Paste in the new content
4. Commit changes
5. GitHub Pages re-deploys automatically in ~30 seconds

To replace images: go into the right `assets/projects/<project-folder>/`, delete the old file, upload the new one with the same name.

---

## Notes

- The website (`index.html`) and the README share the same images and PDFs from the `assets/` folder, so you never need to upload anything twice.
- The site is fully responsive — it looks good on phones too.
- No build tools, no JavaScript frameworks, no dependencies — just one HTML file. It will keep working for years with zero maintenance.
- If you want to add a custom domain later (e.g. `yourname.com`), GitHub Pages supports that in the same Settings → Pages screen.
