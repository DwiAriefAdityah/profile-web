# Personal Data Portfolio

A responsive, static React portfolio for a data analyst and BI developer. The site uses Vite, React, Lucide icons, and custom CSS. It has no server-side requirements; profile content and project notes live in `src/main.jsx`.

## Run locally

1. Install Node.js (18 or newer).
2. In this folder, run `npm install`.
3. Run `npm run dev` and open the local URL Vite prints.
4. Run `npm run build` to create the production site in `dist/`.

## Edit your portfolio

- Open `src/main.jsx` and edit the `profile` values (name, email, phone, location, WhatsApp). LinkedIn is linked in the hero section.
- Update the `projects` array to edit titles, descriptions, technologies, and project details. Current entries are explicitly framed as examples or ongoing initiatives.
- Update the `skills` array to change skill categories and items. Proficiency scores are not shown.
- Update the `experience` list and `Timeline` section to edit roles, dates, responsibilities, education, and certificates.
- The hero portrait is `public/2.png`; replace that file to update the photo. Project visuals are CSS placeholders that can be replaced with screenshots.
- Replace `public/cv-dwi-arief-adityah.pdf` to update the downloadable CV; the hero button points to this file.
- The standalone, responsive CV summary is `public/cv.html`; after deployment it is available at `/cv.html` and includes a print / save as PDF control.
- Edit `index.html` title and description to match the final public identity.

## Deploy

The repository is configured for GitHub Pages at `DwiAriefAdityah/profile-web`. Push to the `main` branch to run `.github/workflows/deploy.yml`; it installs dependencies, builds the site, and publishes `dist/`. In the repository settings, set **Pages → Build and deployment → Source** to **GitHub Actions**. The expected site URL is `https://dwiariefadityah.github.io/profile-web/`. The standalone CV summary is at `/profile-web/cv.html`. The site uses email and WhatsApp links and does not need a backend.

For another static host, build with `npm run build` and publish the contents of `dist/`.
