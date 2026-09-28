# Lotus Constructions

The website of A. Naresh Kumar, Lotus Planners & Constructions, Hyderabad. Served by GitHub Pages at
[lotusconstructions.in](https://lotusconstructions.in) (see `CNAME`).

Everything runs from one page, `index.html`. There is no build step: edit the file, commit, and Pages publishes it.

## What is on the site

- **The story.** Scroll the home page and a house is built from bare ground in 3D (three.js). Near the end the
  camera pulls back over the street, and the neighbours are real Lotus projects. Their name tags link
  to each project.
- **Portfolio** (`#/portfolio`). A walk down an eleven-building street at golden hour, one building at a time,
  with the real render, photograph or presentation board beside each 3D model. Below it is every project full
  size, with filters and a zoomable viewer.
  Each project has its own link, for example `#/portfolio/jamuna`.
- **Construction, Materials, Interiors** (`#/construction`, `#/materials`, `#/interiors`). Deeper pages on the quality
  behind the work.

## Adding or changing a project

1. Export the image as WebP in two widths and put it in `assets/work/`, named `<slug>-<width>.webp`
   (for example `assets/work/jamuna-720.webp` and `assets/work/jamuna-1229.webp`).
2. Add an entry to the `WORK` list in `index.html` (search for `var WORK=`): the name, type, floors, the image
   sizes, the pixel width and height, and the text. `kind` sets the badge (`render`, `photo`, `model` or `board`).
   `home:false` keeps a project off the home page. `views` adds more images to the viewer, such as a road view
   and an aerial view.

The 3D street shows the eleven modelled projects (`LOTUS_SITES`); `WALK` sets the order of the stops.

## What stays off the site

The site shows the work, not the paperwork or the method. Before anything is published:

- Leave out client names, addresses and localities, survey and plot numbers, plot areas and room dimensions,
  signatures, stamps and dates. Remove them from images too (name plates, title blocks, captions).
- Do not publish working drawings: floor plans, site plans, structural drawings or specifications. Projects that only
  have drawings are shown as 3D presentation boards (a road view and an aerial view of the model).
- Credit outside artists privately, not on the page.
- Describe results and standards, not procedures, quantities or test schedules.

Anything that was published earlier stays in this repository's history. To remove it completely, make the
repository private or ask GitHub Support to purge it.

## Contact details

- Telephone and WhatsApp: `+91 94403 40894`. It is set in the contact list, `WHATSAPP_NUMBER`, the `LOTUS` object
  and the structured data. Search for `9440340894` to change all of them at once.
- Email: `nareshamidyala@gmail.com`. Search for it the same way.

## Assets

- `assets/work/` holds the renders, the site photographs (Apple Hospitals, Devanshika Homes), the presentation
  boards with their road and aerial views, and the redrawn Noble elevation, all in WebP.
- `assets/tex/` holds the Ganesha and flowering-tree motifs, cut from the renders and used on the 3D models.
- `assets/og.jpg` is the preview image shown when a link to the site is shared.
