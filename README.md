# Jorge Acuña Vallejos — Portfolio

A static, single-page portfolio site generated from project notes. Plain
HTML/CSS, no build step, no framework — deployable as-is via GitHub Pages.

## Structure

- `index.html` — the entire site: hero, About Me, Technical Skills,
  Education & Experience, Notable Projects (01–05), and Contact Info, all
  on one scrolling page.
- `assets/<slug>/` — images for each project.
- `assets/style.css` — shared stylesheet (dark navy background, amber
  accent, pill-style section labels).
- `assets/photo.jpg` — hero headshot. **Currently a placeholder** — drop
  your real photo in at this same path/filename to replace it.
- `.nojekyll` — tells GitHub Pages to serve files as-is (no Jekyll
  processing).

## Placeholder content — please edit

Several sections were generated with placeholder or best-guess content
since it wasn't present in the source project notes. Search `index.html`
for `PLACEHOLDER` comments to find them all. Specifically:

- **Hero tagline** — drafted; edit to your own voice.
- **About Me bio** — drafted from the Role/Tools/Domain lines across your
  5 project docs (real data), but the wording is mine — edit freely.
- **Technical Skills** — aggregated from the real "Tools Used" lines in
  your project docs, grouped into 4 columns. Add/remove as needed.
- **Education** and **Experience** — no data existed in the source notes
  at all, so these are empty placeholder entries (`[Your School / Program]`,
  `[Company Name]`, etc.). Replace with your real history.
- **Contact info** — email (jbav91@gmail.com) is real; phone/WhatsApp and
  LinkedIn are placeholders (`[Add your number]`, `[linkedin.com/in/...]`).
- **Download CV button** — currently links to `#`; point it at a real CV
  PDF once you have one hosted.
- **Photo** — `assets/photo.jpg` is a generated placeholder avatar, not a
  real photo.

## How this site is built

This repo is the **output** of a build process that reads from a separate,
read-only `Source` folder (one subfolder of notes/assets per project).
Only image files (`.jpg`, `.jpeg`, `.png`, `.gif`) are copied into
`assets/`; other file types found alongside project notes (video, code,
data files, credentials, installers, etc.) are intentionally excluded.
`.git`, `README.md`, `.gitignore`, `CNAME`, and `.nojekyll` are never
touched by the build.

## Deploying

Push this repo to GitHub and enable GitHub Pages (serving from the repo
root of the default branch). `.nojekyll` is already in place.
