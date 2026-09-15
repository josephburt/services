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

## Future: $1 review fee

The form is free today. When you want people to pay $1 before a request is reviewed:

1. Create a Stripe Payment Link for $1.
2. Set the success URL to `https://services.burtlabs.org/#contact?paid=1`.
3. Replace the form’s submit button with a “Pay $1 to send request” flow that only posts after that query string is present.

Keep the mailto fallback so existing customers can still write directly.

## Local preview

Open `index.html` in a browser, or from this folder:

```
python3 -m http.server 8080
```
