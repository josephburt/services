# Burt Labs Services

Static site for local computer repair serving Ellis County, Texas.

Live URL: [services.burtlabs.org](https://services.burtlabs.org)

## GitHub Pages

This repo deploys from `main` via `.github/workflows/pages.yml`.

Custom domain file: `CNAME` → `services.burtlabs.org`

At your DNS host for `burtlabs.org`, add:

```
services    CNAME    josephburt.github.io
```

If you already point `*.burtlabs.org` at GitHub Pages, no extra record is needed.

Then in the repo: **Settings → Pages → Custom domain** → `services.burtlabs.org`, and wait for HTTPS.

## Contact form

The form posts to [FormSubmit](https://formsubmit.co) and delivers to `services@heyitsburt.com`.

The first submission sends a confirmation email to that address. Click the confirm link once. After that, requests arrive as normal email.

## Local preview

Open `index.html` in a browser, or from this folder:

```
python3 -m http.server 8080
```
