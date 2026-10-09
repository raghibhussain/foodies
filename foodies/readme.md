# Foodies 🍕

A responsive restaurant / food landing page built with **plain HTML, CSS and Bootstrap 5** — no frameworks, no build step, and no custom JavaScript.

**Live demo:** https://lovely-crostata-679715.netlify.app

## Features

- Fully responsive layout (mobile, tablet and desktop) using the Bootstrap 5 grid
- Sticky navigation bar with smooth scrolling and active-section highlighting (Bootstrap Scrollspy)
- Hero section, highlights strip, About, Menu cards, FAQ accordion and promotional banner
- Contact / order form and newsletter signup handled by **Netlify Forms**, with honeypot spam protection
- Branded thank-you page shown after a form is submitted
- Accessible markup: semantic headings, image alt text and labelled form fields
- Icons from Bootstrap Icons

## Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Page structure |
| CSS3 (`style.css`) | Custom styling and brand colours |
| [Bootstrap 5.3.2](https://getbootstrap.com/) | Layout, components and interactivity (bundled locally) |
| [Bootstrap Icons](https://icons.getbootstrap.com/) | Icons (loaded from CDN) |
| [Netlify Forms](https://docs.netlify.com/forms/setup/) | Form submissions without a backend |

## Project Structure

```
.
├── index.html               # Main landing page
├── thank-you.html           # Page shown after a form submission
├── style.css                # Custom styles
├── media/                   # Images, logo and favicon
├── bootstrap-5.3.2-dist/    # Local copy of Bootstrap CSS & JS
└── README.md
```

## Running Locally

No installation is needed. Either:

1. Open `index.html` directly in your browser, **or**
2. Serve the folder with any static server, for example:
   ```bash
   npx serve .
   # or
   python3 -m http.server 8000
   ```

> Note: the forms only process submissions when the site is deployed on Netlify. Locally they will just redirect to `/thank-you`.

## Deployment

The site is static, so it can be deployed anywhere.

**Netlify (recommended, required for the forms):**
1. Push this repository to GitHub.
2. In Netlify, choose **Add new project → Import an existing project** and select the repo.
3. Leave the build command empty and set the publish directory to `.` (the repo root).
4. Deploy. Form submissions appear in the Netlify dashboard under **Forms**.

**GitHub Pages:** enable Pages in the repository settings and select the `main` branch root. (The pages will work, but form submissions require Netlify.)

## Pushing to GitHub

```bash
git init
git add .
git commit -m "Initial commit: Foodies landing page"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

## License

Free to use for personal and educational purposes.

## 👤 Author

**Raghib**
GitHub: [@raghibhussain](https://github.com/raghib hussain)
