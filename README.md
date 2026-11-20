# MyDesk

A personal desk: to-do list, Remember board, goals, calendar, diary (tap or voice), habits, insights graphs, music / movies / chess trackers, focus timer, breathing exercise, light/dark/dusk themes, PIN lock, backup & restore. Works on phone and laptop and can be installed like an app.

## Privacy: how "other people can use it but can't see my stuff" works

There is no server and no database. Everything is stored in the browser's own `localStorage` on each person's device. When a friend opens your link, they get their own empty MyDesk. They cannot see yours, and you cannot see theirs.

- Optional PIN lock (Settings) hides the app on a shared computer. It is a screen lock, not encryption.
- Data lives in one browser on one device. Use Settings → **Download backup** now and then, and **Restore** to move to another device. Clearing browser data erases it.

## Deploy (free, takes ~2 minutes)

You need these 4 files in one folder: `index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`.

**Netlify Drop (easiest):** go to https://app.netlify.com/drop and drag the folder onto the page. You get a public link right away.

**GitHub Pages:** create a repo, upload the 4 files, then Settings → Pages → Deploy from branch → `main` / root.

**Vercel / Cloudflare Pages:** import the repo or upload the folder. No build command, output directory is the root.

Open the link on your phone and choose **Add to Home Screen** (or the install icon in Chrome on laptop) to use it like an app.

## Customising

Everything is in `index.html`. Colours are the CSS variables at the top (`--accent`, `--lav`, ...). Daily quotes are the `QUOTES` list and the diary tags are the `TAGS` list.
