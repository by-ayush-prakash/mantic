# Mantic Publishing

manticpublishing.com

Mantic publishes books that break the mainstream narrative. We break and build
the idea with the author until the argument holds.

## The site

Three static pages. No build step, no dependencies, no JavaScript. Each page is
self-contained: the CSS is inlined, so any file works on its own.

| File | Page |
|---|---|
| `index.html` | Home. The sentence, and nothing else. |
| `standards.html` | What we look for. |
| `about.html` | About. |

`_redirects` sends the old `/authors.html` path to `/standards.html` (Netlify).

Favicons: `favicon.svg` is the real one, `favicon.png` and
`apple-touch-icon.png` are fallbacks.

## Editing

Open the file and edit the HTML. There is nothing to compile and nothing to
install.

Type is Newsreader for prose, Archivo for the wordmark, Inter for small caps.
All three load from Google Fonts. Colours live in the `:root` block at the top
of each file, so a palette change means editing three files.

## Deploying

Netlify builds from `main` and publishes automatically. Push and it goes live.

```
git add -A
git commit -m "..."
git push
```

Publish directory is the repo root. There is no build command.
