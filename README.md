# Bhed Prabhed Kosh

A single-page website for **Bhed Prabhed Kosh** by Gitarthganga, a Jain reference book on the classifications (bhed-prabhed) of jiv. The book is shown as an embedded [Heyzine](https://heyzine.com) flipbook.

It is a plain static site (`index.html` + `styles.css`, no build step) deployed on Vercel. Every push to `main` deploys automatically.

## Changing the flipbook

1. In Heyzine, copy the new embed code (or just the new flipbook URL).
2. In `index.html`, replace the `<iframe>` inside `.book-frame` (keep `title="..."` on it for accessibility).
3. Update the same URL in the two "Open in full screen" / "open it here" links below it.
4. If the cover changed, update the `og:image` and `twitter:image` URLs in `<head>`.
5. Commit and push to `main`.

The iframe height is controlled in `styles.css` (`.book-frame iframe`), so the inline `height: 400px` from Heyzine's code is overridden automatically.

## Placeholders

- **Logo**: replace the `logo-placeholder` div in the header with `<img src="logo.png" alt="Gitarthganga logo" class="logo">`.
- **Contact**: edit the `contact` line in the footer.

## Run locally

```bash
npx serve .
```
