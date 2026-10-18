# Yusufu A. Savage — Personal Portfolio

A responsive static portfolio built with HTML, CSS and a small amount of JavaScript. It is designed for deployment to Cloudflare Pages from GitHub.

## Files
- `index.html` — page content and metadata
- `styles.css` — layout, colours and responsive styling
- `script.js` — mobile navigation and current footer year
- `README.md` — setup and deployment notes

## Before publishing
1. In `index.html`, replace `YOUR.EMAIL@example.com` with your professional email address.
2. Replace `https://www.linkedin.com/` with your actual LinkedIn profile URL.
3. Review the CV, education, experience and project wording for accuracy.
4. Only publish information and work samples you are comfortable sharing publicly. Do not include private WFP documents, internal data or confidential project material.
5. If you want to add a CV download, put a PDF in the repository (for example `assets/Yusufu-Savage-CV.pdf`) only after checking that it contains no sensitive personal information, and link to it from the page.

## Deploy with GitHub + Cloudflare Pages
1. Create a GitHub repository, e.g. `yusufu-portfolio`.
2. Upload all files in this folder. Keep `index.html`, `styles.css` and `script.js` in the repository root.
3. In Cloudflare, open **Workers & Pages** → **Create application** → **Pages** → connect to Git.
4. Select the repository and configure:
   - Production branch: `main`
   - Framework preset: `None`
   - Build command: leave blank if accepted, otherwise use `exit 0`
   - Build output directory: `/` (or `.` if the dashboard requires a relative directory)
5. Deploy. Cloudflare will provide a `*.pages.dev` URL.

## Connect a custom domain
1. Buy or use a domain you own.
2. In the Cloudflare Pages project, choose **Custom domains** → **Set up a custom domain**.
3. Enter the domain and follow Cloudflare's instructions.
4. If using the apex domain (e.g. `example.com`), Cloudflare generally requires the domain to be added as a Cloudflare zone with nameservers pointed to Cloudflare. If using a subdomain (e.g. `www.example.com`) and keeping DNS elsewhere, follow Cloudflare's current CNAME instructions.
5. Wait for DNS and HTTPS provisioning, then test both desktop and mobile.

## Updating
Edit a file on GitHub and commit the changes. Cloudflare Pages automatically rebuilds and deploys from the connected production branch.

## Notes
This is a static site. It does not include a database, private admin panel, form backend or server-side processing. The email button opens the visitor's email application.
# yusufu-portfolio
