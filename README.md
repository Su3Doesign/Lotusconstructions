# Lotus Constructions

The website of A. Naresh Kumar, Lotus Planners & Builders, Hyderabad. Served by GitHub Pages at
[lotusconstructions.in](https://lotusconstructions.in) (see `CNAME`).

Everything runs from one page, `index.html`. There is no build step: edit the file, commit, and Pages publishes it.

## What is on the site

- **The story.** Scroll the home page and a house is built from bare ground in 3D (three.js). Near the end the
  camera pulls back over the street, and the neighbours are the real Lotus projects below. Their name tags link
  to each project.
- **Portfolio** (`#/portfolio`). A walk down that street at golden hour, one building at a time, with the real
  render beside each 3D model. Below it is every render full size, with filters and a zoomable viewer.
  Each project has its own link, for example `#/portfolio/jamuna`.
- **Construction, Materials, Interiors** (`#/construction`, `#/materials`, `#/interiors`). Deeper pages on how the
  work is done.

## Adding or changing a project

1. Export the render as WebP in two widths and put it in `assets/work/`, named `<slug>-<width>.webp`
   (for example `assets/work/jamuna-720.webp` and `assets/work/jamuna-1229.webp`).
2. Add an entry to the `WORK` list in `index.html` (search for `var WORK=`). The fields are the name, type,
   floors, location, client, the image sizes, the pixel width and height, and the text.

The project then appears in "Selected work" on the home page, in the portfolio gallery and in the viewer.
The 3D street shows only the four projects that have been modelled (`LOTUS_SITES`). A new project needs its
own model before it can join the street.

## Contact details

The telephone and WhatsApp number (`+91 94403 40894`) comes from the credit block on the Lotus drawings. It is
set in three places in `index.html`: the contact list, `WHATSAPP_NUMBER`, and the `LOTUS` object. Search for
`9440340894` to change all of them at once.

## Assets

- `assets/work/` holds the renders and drawings, in WebP. The Noble School of Nursing elevation is redrawn from the
  vectors in its original PDF (`noble-drawing-*`). The original is kept too (`noble-original-2000.webp`).
- `assets/tex/` holds the Ganesha and flowering-tree motifs, cut from the renders and used on the 3D models.
- `assets/og.jpg` is the preview image shown when a link to the site is shared.
