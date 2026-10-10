# Gallery images

This directory is maintained by the workshop organizers. Participants should submit an image, video, or
public link by email or through the
[gallery contribution issue](https://github.com/sungho91/geoflac-des-2026/issues/new?template=gallery-contribution.md)
instead of editing the website directly.

## Publishing a submission

Put DynEarthSol result images in this folder (PNG/JPG, ideally < 1 MB each, ~1200px wide).

Then register each image in the **Gallery** section of `../index.html`:
find `const GALLERY = [ ... ]` near the bottom and add one entry per image:

```js
{
  src: "gallery/my-result.png",
  caption: "3D coupled tectonic–surface model",
  credit: "Your Name, KIGAM"   // optional
}
```

Re-upload both the image and `index.html` to publish. Clicking a gallery image opens the full-size version.

## Published manuscript figures

- `des-gospl-coupling.png`: DES-goSPL coupling and landscape evolution, from Shyu et al. (2026), *DynEarthSol v2.0*.
- `des-ep-rsf-localization.png`: fault localization and stick-slip behavior in EP and EP-RSF models, from Shyu et al. (2026), *DynEarthSol v2.0*.

Source: <https://doi.org/10.5194/egusphere-2026-2922> (CC BY 4.0). The web images preserve the complete figures and were resized from the manuscript PDFs.
