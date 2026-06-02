# GeoFLAC/DynEarthSol Workshop & Hackathon 2026

Website for the **GeoFLAC/DynEarthSol Workshop & Hackathon** — KIGAM, **November 2–6, 2026**. In-person, free, open to everyone.

- 🔗 **Live site:** https://sungho91.github.io/geoflac-des-2026/
- 📦 **Repository:** https://github.com/sungho91/geoflac-des-2026
- ✉️ **Contact:** slee91@kigam.re.kr

The whole site is one file — [`index.html`](index.html) (HTML + CSS + a little JS, light theme). Images live in [`gallery/`](gallery/).

## How to publish a change
Edit `index.html`, then from this folder:
```bash
git add -A
git commit -m "describe your change"
git push
```
GitHub Pages rebuilds in ~1 minute. (Hard-refresh with `Ctrl+F5` if you don't see the change.)

## Forms (registration & talks)
GitHub Pages is static and can't store submissions, and Google/OneDrive are blocked on the KIGAM
network — so we use free **Tally.so** forms, linked from the site buttons:

| Button | Form |
|--------|------|
| **Register now** | https://tally.so/r/obv1MN |
| **Submit a talk** / Open submission form | https://tally.so/r/J9Mx2X |

- Tally's free plan caps file uploads at **10 MB/file**. Large files (videos): presenters use the
  site's **"Email a large file"** button (pre-filled `mailto:` to slee91@kigam.re.kr).
- Submissions appear in each form's **Submissions** tab in Tally. (Email notifications go to the
  Tally account's Gmail; forward to slee91@kigam.re.kr or just check the dashboard.)

## Publishing accepted talks
Find `const TALKS = [ ... ]` near the bottom of `index.html` and add one block per talk:
```js
{
  title: "Talk title",
  speaker: "Speaker Name",
  affiliation: "Institution",
  abstract: "Two or three sentences.",
  files: [ { label: "Slides (PDF)", url: "https://..." } ] // optional
}
```
An empty `TALKS` list shows a "no talks yet" message automatically.

## Adding gallery images
Only post images you own or have permission to share. Then:
1. Put the image (PNG/JPG, < 1 MB, ~1200px) in [`gallery/`](gallery/).
2. Add an entry to `const GALLERY = [ ... ]` near the bottom of `index.html`:
   ```js
   { src: "gallery/my-result.png", caption: "Short caption", credit: "Your Name, KIGAM" }
   ```
See [`gallery/README.md`](gallery/README.md).

## Section map (what's on the page)
About · About DynEarthSol · Gallery · Schedule · Before you come (build DynEarthSol) ·
Hackathon agenda · Talks · Call for Presentations · Venue · Travel & Stay · Register · FAQ

## Notes & constraints
- **All site text is in English.**
- **KIGAM network:** Google (Maps/Drive/Forms) and OneDrive are blocked. Hotel/map links use
  **Naver Map**; the site advises international visitors to use Naver Map / KakaoMap, Kakao T, and T-money.
- **No public Wi-Fi on-site** (security policy) — attendees should prepare offline.
- Tutorials use **DynEarthSol**; the build is **not** covered, so attendees build it beforehand
  (repo: https://github.com/GeoFLAC/DynEarthSol). The hackathon agenda follows the
  [2026 roadmap (issue #43)](https://github.com/GeoFLAC/DynEarthSol/issues/43).
- `Figures/` and `*.pptx` are git-ignored (working files, not for the public site).

## Still to do (optional)
- [ ] Abstract for the "Progress in LagHost" talk (currently a placeholder)
- [ ] Add more gallery images as results come in
- [ ] Finalize detailed schedule / tutorial topics

## How it's deployed
GitHub Pages serves the `main` branch (root) at the live URL above. To re-check: repo
**Settings → Pages**. Linking from a future personal site (`https://sungho91.github.io/`) is as
simple as adding a link to the live URL.
