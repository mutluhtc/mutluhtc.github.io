# Hatice Mutlu — GitHub Pages website

This folder contains a ready-to-publish static website for:

`https://mutluhtc.github.io`

## Publish it

1. Log in to GitHub.
2. Create a **public** repository named exactly:

   `mutluhtc.github.io`

3. Upload everything inside this folder to the repository:
   - `index.html`
   - `style.css`
   - `script.js`
   - `assets/favicon.svg`

4. Commit the files to the `main` branch.
5. Open the repository's **Settings → Pages**.
6. Under **Build and deployment**, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
7. Save.

The site should then appear at `https://mutluhtc.github.io`.

## Edit the content

Open `index.html` in a text editor. Search for these comments:

- `Add LinkedIn, Google Scholar, ORCID, or a CV link here.`
- `Replace this note with your publication list`
- `Add the professional email address`

You can safely edit the visible text without changing the HTML structure.

## Add a CV

1. Put your PDF in the same folder and name it `cv.pdf`.
2. Add this link where you want the CV button to appear:

```html
<a class="button secondary" href="cv.pdf">Download CV</a>
```

## Add a profile photograph

The current site uses an `HM` monogram. To use a photograph:

1. Add the image as `assets/profile.jpg`.
2. Replace:

```html
<div class="profile-monogram" aria-hidden="true">HM</div>
```

with:

```html
<img class="profile-photo" src="assets/profile.jpg" alt="Portrait of Hatice Mutlu">
```

Then add the following to `style.css`:

```css
.profile-photo {
  width: 132px;
  height: 132px;
  margin: 0 auto 24px;
  border-radius: 50%;
  object-fit: cover;
}
```

## Preview locally

Double-click `index.html`, or run a small local server:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.
