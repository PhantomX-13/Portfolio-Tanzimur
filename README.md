# Portfolio: MD. Tanzimur Rahman

Personal portfolio website of **MD. Tanzimur Rahman**, a Computer Science & Engineering undergraduate at American International University-Bangladesh (AIUB).

| | |
|---|---|
| **Live site** | https://phantomx-13.github.io/Portfolio-Tanzimur/ |
| **Mirror** | https://portfolio-tanzimur.vercel.app |
| **Hosting** | GitHub Pages (via GitHub Actions) and Vercel |
| **Type** | Single-page site, one `index.html`, no build step |

## Sections

Home, About, Video, Education, Skills, Experience, Projects, Research, Courses & Programs, Events & Community, Resume, Contact.

## Features

- Responsive layout for desktop and mobile
- Dark and light theme, with the choice remembered in the browser
- In-browser viewing of the research poster and paper (PDF), and resume download
- Image lightbox for certificates

## Tech Stack

| Area | Technology |
|---|---|
| Markup and styling | HTML, CSS |
| Logic | JavaScript, React 18 (UMD build from the unpkg CDN) |
| JSX compilation | Babel Standalone (in the browser) |
| Fonts | Google Fonts: Space Grotesk, Inter |

## Repository Structure

```text
index.html            # Entire site: styles, React components and content
.nojekyll             # Tells GitHub Pages to serve files as-is
.github/workflows/    # GitHub Actions workflow for Pages deployment
```

## Run Locally

Open `index.html` in a browser, or serve it with a local server:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

> [!NOTE]
> An internet connection is needed for the CDN scripts and fonts.

## Updating and Deploying

All content lives in the React components inside `index.html`. Images, the resume and the research PDFs are embedded as base64 strings, so replacing `index.html` is enough to publish an update.

```bash
git add index.html
git commit -m "Update portfolio"
git push origin main
```

Pushing to `main` triggers the GitHub Actions workflow, which publishes the site to GitHub Pages in about one to two minutes. The same repository is also deployed on Vercel.

> [!NOTE]
> The text, images, certificates, resume and research documents in this repository are personal content. Please do not reuse them without permission.
