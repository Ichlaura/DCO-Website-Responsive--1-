# DCO Dental Care Office — React website

Responsive client-ready website built with React + Vite. Includes three selectable hero designs (Modern Blue, Executive Blue, Midnight Gold), all original service/pricing content, client review, contact links, and premium footer.

## Run locally

Requires Node.js 20+.

```bash
npm install
npm run dev
```

Open the URL shown in the terminal (usually http://localhost:5173).

## Production build

```bash
npm run build
npm run preview
```

## Deploy to GitHub + Vercel

1. Create a new GitHub repository and upload the project contents (not `node_modules`).
2. In Vercel choose **Add New → Project**, import the repository.
3. Framework: **Vite**. Build command: `npm run build`. Output directory: `dist`.
4. Deploy. Vercel will redeploy on subsequent pushes.

## Deploy to Render

1. Push this project to GitHub.
2. In Render create a **Static Site** and connect the repository (or use the included `render.yaml` blueprint).
3. Build command: `npm install && npm run build`.
4. Publish directory: `dist`.
5. Deploy.

## Client handoff

- The small design picker at the very top changes the theme and remembers the choice in the browser.
- Once the client chooses, edit the `theme` initial value in `src/main.jsx` and remove the `design-picker` div to publish a single design.
- All original service prices and descriptions are preserved in `src/serviceDetails.json`; confirm prices with the client before going live.
- Contact links currently point to `dco.assistance@gmail.com`, `+1 630 999 5743`, WhatsApp, and `instagram.com/dco2_026/` from the provided site.
- The Pearly Smiles Dental review was reproduced from the supplied HTML; obtain the client's permission/confirmation for testimonial and rating claims before publishing.
- The Request Service buttons go to the contact section; no form or patient information is collected/stored.
- Hero images and brand assets are in `public/assets/`.
