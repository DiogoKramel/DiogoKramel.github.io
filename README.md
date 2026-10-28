# DiogoKramel.github.io

Personal academic website of **Diogo Kramel**, Postdoctoral Fellow at the Industrial Ecology Programme, NTNU.

A plain static site (HTML + CSS, no build step), laid out like
[biancach.github.io](https://biancach.github.io/): a header with photo, bio and links, a list of research
projects with their publications and an illustration, a teaching/talks band, and a footer.

## Structure

```
.
├── index.html          # Main page: bio, research projects, teaching and selected talks
├── talks.html          # Full list of talks and presentations, by year
├── style.css           # All styling (responsive; stacks to one column under 768px)
├── CV.pdf              # Two-page CV generated from public data
├── icon.png            # Favicon
├── images/
│   ├── diogo.jpg       # Headshot (placeholder, replace with your photo)
│   ├── mariteam.svg    # Animated: ships moving along global routes
│   ├── scenarios.svg   # Animated: diverging emission pathways to 2050 (schematic)
│   ├── well-to-wake.svg
│   └── ocean.svg
└── .nojekyll           # Serve files as-is on GitHub Pages
```

## Publish on GitHub Pages

1. Create a public repository on GitHub named exactly `DiogoKramel.github.io`.
2. Push this folder to it:
   ```bash
   git remote add origin https://github.com/DiogoKramel/DiogoKramel.github.io.git
   git branch -M main
   git push -u origin main
   ```
3. In the repository, open **Settings → Pages**, set the source to **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. The site goes live at <https://diogokramel.github.io/> within a minute or two.

To preview locally: `python3 -m http.server` in this folder, then open <http://localhost:8000>.

## Editing

- **Photo:** overwrite `images/diogo.jpg` with a square photo (about 500 × 500 px).
- **Project figures:** the SVGs are schematic placeholders. Swap in real figures or GIFs from your papers
  (for example a MariTEAM emissions map) by changing the `src` of the matching `<img class="project-img">`.
- **New paper:** edit the "New paper!" block at the top of the project list, and add the entry to the matching project.
- **Publication format:** each entry is a `<li>` inside a `pub-sublist`; your name is wrapped in `<strong>`.
- **CV:** replace `CV.pdf` with your own whenever you like; the link in the bio stays the same.

## Sources

Content was compiled from public pages on 28 October 2026:

- NTNU employee profile: <https://www.ntnu.edu/employees/diogo.kramel>
- CLIMMS project page: <https://www.ntnu.edu/ept/climms>
- Nord_H2ub description: <https://www.nordicenergy.org/article/about-nord_h2ub>
- NTNU Open record of the PhD thesis: <https://hdl.handle.net/11250/3151029>
- Publication DOIs and talk handles as linked on the site
