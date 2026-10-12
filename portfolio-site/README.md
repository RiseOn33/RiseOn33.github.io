# Portfolio site

Plain HTML and CSS. No build tools, no frameworks. Hosted free on GitHub Pages.

## Put it online (one time, ~5 minutes)

1. Sign in to GitHub and create a **new repository** named exactly `your-username.github.io`
   (replace `your-username` with your GitHub username). Make it **Public**.
2. On the new repo page, click **"uploading an existing file"**.
3. Unzip this folder on your computer and drag **everything inside it** (index.html, css/, projects/, images/, README.md) into the upload area. Click **Commit changes**.
4. Go to **Settings → Pages**. Under "Build and deployment", source should be **Deploy from a branch**, branch **main**, folder **/ (root)**. Save if it isn't already.
5. Wait a minute or two, then visit `https://your-username.github.io`.

To update the site later, edit a file on GitHub (pencil icon) or upload a replacement, then commit. It redeploys automatically.

## Folder layout

```
index.html                 Home page: about, experience, projects, skills, education, contact
css/style.css              All styling (colors and fonts are at the top)
projects/
  project-template.html    Blank write-up. Copy this for each new project.
images/                    Put your photos here
resume.pdf                 Add your résumé here (the About section links to it)
```

## How the home page is organized

Sections, top to bottom: About, Experience (most recent first), Projects (card grid),
Skills (grouped), Education (with relevant coursework), Contact.
Text with a dashed underline is placeholder copy: replace it and delete `class="ph"`.
To add another job, project card, or course, copy an existing block and edit it.

## Things to edit first

- **Your content**: filled in from your résumé. Remaining placeholders have a dashed underline.
- **Headshot**: add `images/headshot.jpg` and swap it into the hero (see the comment there).
- **Contact links**: the `#contact` section in index.html (email, GitHub, LinkedIn).
- **Résumé**: upload your PDF as `resume.pdf` in the root folder.

## Adding a project

1. Copy `projects/project-template.html` to a new name, like `projects/buck-converter.html`, and fill it in.
2. In index.html, copy one `<a class="pcard">` block in the Projects section, point its `href` at the new page, and update the text.

## Adding photos

Put images in `images/`, then replace a placeholder:

```html
<!-- on index.html project cards: replace <div class="slot">...</div> with -->
<img class="media" src="images/cubesat.jpg" alt="Printed 1U frame on the bench">

<!-- on project pages (note the ../) -->
<img src="../images/cubesat.jpg" alt="Printed 1U frame on the bench">
```

Resize photos to about 1600 px wide before uploading so pages load fast on phones.

Check with SSRL before posting lab design files or anything sensitive.
