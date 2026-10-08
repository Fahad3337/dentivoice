# Dentivoice landing page

Static landing page for Dentivoice, an AI voice receptionist for dental clinics.

- `index.html` is the page. `assets/` holds images, audio demos and the compiled CSS.
- Styling is Tailwind v3. Source is `src/input.css`; rebuild after changing classes:
  `npx tailwindcss@3 -i src/input.css -o assets/styles.css --minify`
  then bump `styles.css?v=N` in `index.html`.
- Local preview: `python3 -m http.server 8080`

## Deploy (Render)
Static Site, no build command, publish directory `.` (see `render.yaml`).
After the first deploy, set `canonical` / `og:url` in `index.html` to the live URL.
