# Burt Labs Services

One-page site for local computer repair serving Ellis County, Texas.

Live URL: [services.burtlabs.org](https://services.burtlabs.org)

The whole site is `index.html` plus images in `assets/`. GitHub Pages deploys from `main`.

Custom domain: `CNAME` → `services.burtlabs.org`

At DNS for `burtlabs.org`:

```
services    CNAME    josephburt.github.io
```

## Contact form

The form posts to [FormSubmit](https://formsubmit.co) and delivers to `services@heyitsburt.com`. After submit, visitors return to the same page with a confirmation.

The first submission sends a confirmation email to that address. Click the confirm link once.

## Future: $1 review fee

When you want a $1 review fee, create a Stripe Payment Link and only show the form after a successful `$1` payment.

## Local preview

```
python3 -m http.server 8080
```
