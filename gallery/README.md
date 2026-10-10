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
