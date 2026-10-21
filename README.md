# Bassam Ashraf — Interactive Data & AI Portfolio

Responsive dark multi-page Next.js 15 + TypeScript website based on the uploaded CV.

## Requirements
- Node.js 20 or newer (Node.js 22 LTS recommended)
- npm

## Run locally (Windows PowerShell)
```powershell
cd path\to\bassam-portfolio
npm install
npm run dev
```
Open http://localhost:3000.

## Production build
```powershell
npm run build
npm run start
```

## Add your profile photo
Save your own photograph as `public/images/profile.jpg` (landscape or portrait works; crop uses object-fit: cover). Until then, the site shows a designed initials placeholder.

## Update project evidence
- Edit `lib/data.ts` to add verified model names, metrics, datasets, project details, repository URLs and screenshots.
- The analytics panel (`components/VerifiedAnalytics.tsx`) uses **documented counts only**: four CV projects and five evaluated ML models. It does not invent model scores.
- To add real model performance charts later, use your evaluation CSV or JSON and a chart library, and label each metric and validation split.
- Add GitHub and LinkedIn profile links after verifying the exact URLs.
- `public/resume.pdf` contains the supplied CV. Replace it with a revised PDF when necessary.

## Deployment on Vercel
1. Push the folder to a new GitHub repository (do not commit `.next` or `node_modules`).
2. Sign in to https://vercel.com and select **Add New → Project**.
3. Import the repository. Vercel should detect Next.js automatically.
4. Click **Deploy**. Optionally attach your own domain under Project Settings → Domains.

## Pages
`/`, `/about`, `/projects`, `/projects/[slug]`, `/skills`, `/experience`, `/contact`.

## Notes
- Contact uses a `mailto:` link, so there is no backend, API key, or unconfigured contact form.
- DEPI July–December 2026 is labeled ongoing as of October 2026.
- Illustrative project artwork is abstract CSS, not a screenshot of your actual work.
- Web fonts load from Google Fonts when online, with local system font fallbacks.
