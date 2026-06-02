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
GitHub Pages is static, so it can't receive uploads itself. Use a free **Google Form**:
1. Create a form at https://forms.google.com with questions: **Talk title**, **Abstract**, **Speaker name**, **Affiliation**, and a **File upload** question for slides (PDF/PPT).
2. Copy the form's share link into the "Open submission form" button in `index.html` (search `TODO`).
3. Submissions collect automatically in a linked Google Sheet (files go to your Drive).

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
