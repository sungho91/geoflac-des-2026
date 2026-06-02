# GeoFLAC/DES Workshop & Hackathon 2026

Website for the **GeoFLAC/DES Workshop & Hackathon** — KIGAM, November 2–6, 2026. In-person, free, open to everyone.

🔗 **Live site:** https://YOUR-GITHUB-ID.github.io/geoflac-des-2026/ *(update after publishing)*

## Edit the site
Everything is in a single file: [`index.html`](index.html). Open it in a browser to preview, edit the text/styles, and re-upload to publish.

### Things to fill in before launch
- [ ] Registration link (search `TODO` in `index.html` → the "Register now" button)
- [ ] Submission form link (search `TODO` → the "Open submission form" button)
- [ ] Contact email (replace `organizer@example.com`)
- [ ] Finalize the schedule details
- [ ] Update the live-site URL above

## Collecting talks (presenter submissions)
GitHub Pages is static, so it can't receive uploads itself. Google Drive/Forms and OneDrive
are blocked on the KIGAM network, so we use a free **Tally.so** form + email for large files:

1. Create a form at https://tally.so with: **Talk title**, **Abstract**, **Speaker name**,
   **Affiliation**, **Email**, and a **File upload** question for slides.
   - Tally's free plan caps uploads at **10 MB per file** (enforced automatically).
2. Publish, then copy the form link (`https://tally.so/r/XXXXXX`) into the
   "Open submission form" button in `index.html` (search `TODO`).
3. **Large files (videos, big decks > 10 MB):** presenters email them to slee91@kigam.re.kr.
   The site already has an "Email a large file" button (a pre-filled `mailto:` link) for this.

## Publishing accepted talks
Open `index.html`, find the `const TALKS = [ ... ]` list near the bottom, and add one block per talk:
```js
{
  title: "Your talk title",
  speaker: "Speaker Name",
  affiliation: "Institution",
  abstract: "Two or three sentences.",
  files: [ { label: "Slides (PDF)", url: "https://drive.google.com/..." } ] // optional
}
```
Re-upload `index.html` to update the live site. (To share a file, upload it to Google Drive, set sharing to "Anyone with the link", and paste that link as `url`.)

## Linking from your personal homepage later
Your personal site will live at `https://sungho91.github.io/`. Just add a link to
`https://sungho91.github.io/geoflac-des-2026/` from there to connect them.

## Publish with GitHub Pages
1. Create a repository on GitHub (e.g. `geoflac-des-2026`).
2. Upload `index.html` (and this README).
3. Repo **Settings → Pages → Build from branch → `main` / root → Save**.
4. Wait ~1 minute; your site is live at the URL above.
