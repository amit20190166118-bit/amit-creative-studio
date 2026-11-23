# Amit Creative Studio

A premium, single-page AI-powered cinematic advertising studio website. Built with pure HTML, CSS and vanilla JavaScript for GitHub Pages.

## Files
- `index.html` — semantic page structure, SEO metadata and schema.
- `style.css` — responsive luxury maroon, champagne and gold design.
- `script.js` — dynamic sections, filters, modals, pricing, form, animations.
- `config.js` — editable business content, services, packages, FAQs and portfolio.
- `assets/reels/` — add project thumbnail JPGs and MP4 videos here.
- `assets/og.jpg` — recommended 1200 × 630 social sharing image.
- `assets/favicon.png` — site favicon.

## Edit the website
Open `config.js` and edit the `window.STUDIO_CONFIG` object. Change the phone / WhatsApp number, email, Instagram URL, founder details, hero copy, service descriptions, industries, process steps, package prices, add-ons, FAQs, project titles and footer text there. USD prices are editable approximate conversions; update them to your preferred rates.

The project list is an array of four values per project: title, category, badge label and asset filename (without extension). Keep the filename slug consistent with the matching files in `assets/reels/`.

## Add or replace portfolio media
For a project with filename `gold-light`, upload:
- `assets/reels/gold-light.jpg` — thumbnail image.
- `assets/reels/gold-light.mp4` — video preview.

Repeat the same filename for each project slug in config.js. Images and videos are loaded only when needed. If a thumbnail or video is missing, the project card shows a designed gradient fallback and the modal explains which asset to add. You can also use optimized, compressed videos hosted externally by adapting the video source in script.js.

## Deploy on GitHub Pages
1. Create a GitHub repository, e.g. `amit-creative-studio`.
2. Upload `index.html`, `style.css`, `script.js`, `config.js`, and this README at the repository root.
3. Open repository **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch **main** and folder **/(root)**, then Save.
6. Wait for the Pages build to finish. The expected project URL is `https://amit20190166118-bit.github.io/amit-creative-studio/`.

## Custom domain
In **Settings → Pages → Custom domain**, enter your domain and save. Add the DNS records GitHub requests at your domain registrar (typically a CNAME for `www` pointing to `amit20190166118-bit.github.io`, and GitHub Pages A records for the apex domain). Enable **Enforce HTTPS** after DNS verification. Do not remove existing DNS records until you have confirmed the new records.

## File size guidance
GitHub has practical file-size limits; keep each video small and optimized for web (H.264 MP4, sensible resolution and bitrate). For larger reels, host videos on YouTube, Vimeo or Cloudinary and update the video source logic to use the hosted URL rather than committing large media files to Git.

## Before launch checklist
- [ ] Replace sample portfolio thumbnails and videos with your own approved work.
- [ ] Review USD prices and exchange-rate assumptions.
- [ ] Add real client testimonials only after receiving permission.
- [ ] Add a real 1200 × 630 Open Graph image and favicon.
- [ ] Verify contact details, links, WhatsApp messages and mobile layout.
- [ ] Add any required privacy / terms information for your business.
