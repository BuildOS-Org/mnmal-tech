# Minimal Technologies

Marketing website for **Minimal Technologies Limited**, a Ghana-based studio that builds mobile apps, web apps and business systems.

The site is a single static page with a "tilted sheet of glass" HUD look. Navigating between pages slides the glass sideways, and scrolling moves a page up toward the horizon.

## Pages

| Section | Anchor |
| --- | --- |
| Home | `#home` |
| Services | `#services` |
| Industries | `#industries` |
| Process | `#process` |
| About | `#about` |
| Contact | `#contact` |

## Project structure

```
.
└── docs/
    └── index.html   # the entire site: HTML, CSS and JS in one file
```

The site lives in `docs/` so it can be served directly with GitHub Pages.

## Tech

- Plain HTML, CSS and JavaScript. There is no build step, framework or dependencies.
- Google Fonts: Michroma, Barlow and Share Tech Mono.
- Respects `prefers-reduced-motion`.

## Running locally

Open `docs/index.html` in a browser, or serve the folder:

```sh
cd docs
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

The site is deployed from the `main` branch using GitHub Pages:

1. Go to **Settings → Pages** in the repository.
2. Set the source to **Deploy from a branch**, with branch `main` and folder `/docs`.

## Editing

All content, styles and scripts are in `docs/index.html`. Each page of the site is a section with its own `id` (for example `h-home` and `h-services`). Edit the copy there directly.
