
# About this fork

- fixes font rendering for duplicate characters, required for ligatures
  and alt charsets.

- fixes cmap generation (so copying and searching text work properly).
  the cmap wasn't originally broken, but the way it was generated didn't 
  work after we added the rendering fix above.

- adds softmask to SVG rendering for transparency groups.

# Building

We are using the esm version, so it's sufficient to build that:

> npm run build:es


