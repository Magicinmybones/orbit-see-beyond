# Orbit — See beyond now

Static landing page ("Everything you need to discover, understand, and explore
what is out there."), deployed on Cloudflare Pages.

## Structure

```
public/
  index.html                        the page
  assets/
    fonts/inter-var.woff2           Inter variable, latin subset (was inlined as base64)
    images/sky.webp                 hero sky backdrop (was inlined as base64)
```

The source HTML shipped both assets as base64 `data:` URIs (394 KB single file).
Both were extracted to `public/assets/`, so `index.html` is now 21 KB and the
font and image are cached separately by the browser.

## Local preview

```bash
npm install
npm run dev
```

## Deploy

```bash
npm run deploy
```
