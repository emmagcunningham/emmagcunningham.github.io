# Emma G. Cunningham — Personal Site

A single-page academic site built from your CV, teaching evaluations, and
cover letter — sized for a tenure-track search committee to skim quickly:
research focus up top, teaching evidence (including your eval scores and a
few student quotes), then publications, talks, awards, service, and mentorship.

## Structure

```
.
├── index.html
├── style.css
├── img/
│   └── profile.jpg     # placeholder — swap for a real headshot
└── files/
    └── Cunningham_CV.pdf  # your uploaded CV, linked from the About section
```

## Before you publish — please check

- **Anticipated PhD completion**: your CV (dated today) says June 2027; your
  cover letter (from last year) said May 2026. The site uses **2027**, from
  the more recent document — double check this is still accurate.
- **Email**: I used `egcunningham@wisc.edu` from your CV/cover letter header.
- **Google Scholar link**: I linked a Google Scholar *search* for your name
  since I don't have your exact profile URL — replace it with your real
  profile link once you have one.
- **Photo**: replace `img/profile.jpg` with an actual headshot.
- **Lab links**: "Learning and Transfer Lab" and "Brain and Learning Lab" in
  the Research section currently link to `#` — add the real lab URLs.
- **Mentee list**: the full 50+ name list is tucked into a collapsible
  "Mentored research assistants" toggle near the bottom of the Mentorship
  section so it doesn't overwhelm the page — expand it to check names/spelling.

## Customize

Everything else is plain text in `index.html` — search for the section by
its `<h2>` heading (About, Research, Teaching, Publications, Presentations,
Awards & Service, Mentorship) and edit directly.

Colors and fonts are CSS variables at the top of `style.css` — change
`--accent` to adjust the accent color (currently a deep teal).

## Deploy on GitHub Pages

1. Create a new GitHub repository (e.g. `emmagcunningham.github.io` for a
   user site, or any name for a project site).
2. Push these files to the repository's default branch:
   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/emmagcunningham/your-repo.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**, and under "Build and
   deployment" set **Source** to "Deploy from a branch", branch `main`,
   folder `/ (root)`.
4. Your site will be live at `https://emmagcunningham.github.io/your-repo/`
   (or `https://emmagcunningham.github.io/` if the repo is named
   `emmagcunningham.github.io`).

## Local preview

Open `index.html` directly in a browser, or run:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.
