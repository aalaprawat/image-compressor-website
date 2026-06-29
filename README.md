# Image Compressor Website

Static GitHub Pages website for **Image Compressor: MB to KB** by FrostByte Labs.

## What Was Created

- `index.html` landing page
- `privacy-policy.html` Play Store-ready draft privacy policy
- `terms.html` simple Terms of Use
- `contact.html` support page
- `404.html` themed not-found page
- SEO landing pages for image compression searches
- `assets/` app icon, favicon, onboarding bear assets, website hero banner, and optimized infographics
- `css/styles.css` responsive Material-inspired theme
- `js/main.js` mobile navigation and light/dark theme toggle
- `robots.txt` and `sitemap.xml`

## Local Preview

From the repository root:

```bash
python3 -m http.server 8080
```

Open:

```text
http://localhost:8080/
```

## GitHub Pages Deployment

Use the repository root because this is now a standalone static website repo.

1. Push the website folder/files to GitHub.
2. Go to Repository Settings.
3. Open Pages.
4. Select branch `main`.
5. Select `/root` folder.
6. Save.
7. The website will be available at `https://aalaprawat.github.io/image-compressor-website/`.

## Update Before Publishing

- Google Play link: update the Play Store URL in `index.html` if the app package or listing changes.
- Support email: update `hello.frostbyte@gmail.com` in `privacy-policy.html`, `terms.html`, and `contact.html` if needed.
- Privacy policy placeholders: review the draft notice, effective date, app name, developer name, Firebase disclosures, and contact email in `privacy-policy.html`.
- Sitemap and robots: already use `https://aalaprawat.github.io/image-compressor-website/`; update them only if the repository name changes.
- Screenshots and infographics: replace files in `assets/images/screenshots/` or add new files, then update the gallery image references in `index.html`.

## Theme Values Used

The website uses the Android Compose theme colors from `app/src/main/java/com/frostbyte/imagecompressor/ui/theme/Color.kt`:

- Blue primary: `#0459B0`
- Blue secondary: `#158FE0`
- Blue tertiary: `#56BFF4`
- Blue accent: `#7ACFFB`
- Blue light: `#74D4FA`
- Blue dark: `#03327E`
- Success: `#4CAF50`
- Error: `#E53935`

The light and dark surfaces follow the Android Material theme in `Theme.kt`, including `#FFFBFE`, `#1C1B1F`, and `#2A2A2E`.

## Privacy Notes

The current Android codebase includes Firebase Analytics and Firebase Crashlytics. The public policy mentions these services and keeps the image-processing claim scoped to compression: selected images are processed on-device and are not uploaded to FrostByte Labs servers for compression.
