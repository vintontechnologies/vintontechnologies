# Installation — Vincent Kyalo GitHub Profile

## 1. Open the profile repository

Visit https://github.com/Vinnie-kyalo and open the repository named `Vinnie-kyalo` (the special profile repository must match your GitHub username). If it does not exist yet, create a public repository named exactly `Vinnie-kyalo`.

## 2. Copy the files into the repository

Keep this structure:

```text
Vinnie-kyalo/
├── README.md
├── INSTALLATION.md
└── assets/
    ├── about-me.svg
    ├── skills-and-tools.svg
    ├── projects-and-github.svg
    └── contact-me.svg
```

Upload the supplied `README.md`, `INSTALLATION.md`, and the four SVG files inside `assets/`. Commit the changes to the default branch.

## 3. Update contact placeholders

Edit `README.md` and `assets/contact-me.svg` to replace `[Add LinkedIn profile URL]` and `[Add professional email]` with details you choose to publish. Do not commit private contact information unless you want it public.

## 4. Portrait and GitHub SVG compatibility

`assets/about-me.svg` currently embeds the supplied portrait as a base64 data URI, making the SVG self-contained. GitHub may sanitize or block embedded SVG image data and some SVG animation features. If the portrait does not appear on GitHub, upload your photo to the repository (for example, `assets/vincent-kyalo.jpg`) and replace the `<image ... xlink:href="data:image/jpeg;base64,..."/>` value with a repository-hosted raw image URL, such as the raw URL for that committed image. Keep in mind that GitHub may still limit SVG features for security.

The panels use SVG-native animation elements (`animate`, `animateTransform`, and `animateMotion`). GitHub can restrict animations or other active SVG features in README rendering, so the panels may appear partly or fully static there even though the source files contain real animation. Test the rendered README after committing.

## 5. If animation is restricted

The SVGs remain individually usable as files. For a reliable animated preview, open an SVG locally in a modern browser. For a README that must animate consistently, use a hosted GIF or video preview instead, and link the image to the full SVG or a project page. GitHub README images themselves do not provide a guaranteed way to run arbitrary SVG animation.

## 6. Verify

- Confirm the four filenames and `assets/` paths match the README.
- Open each SVG locally in a browser.
- Check the repository README preview on desktop and mobile.
- Verify the GitHub link; replace any contact placeholders before publishing.


## Animated GIF panels

The repository includes these animated panels, which GitHub can display in the profile README:

- `assets/about-me.gif`
- `assets/skills-and-tools.gif`
- `assets/projects-and-github.gif`
- `assets/contact-me.gif`

The matching `.svg` files are retained as editable source artwork.
