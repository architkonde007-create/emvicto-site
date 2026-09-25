# EMVICTO teaser site

A single-page "coming soon" teaser for EMVICTO, a wearable for endurance athletes. It's plain static HTML, CSS and JS with no build step.

## Files
- `index.html`: the whole site. The logo is embedded inside it as a data URI (CSS mask on `.logo`).
- `logo.png`: the EMVICTO wordmark, white on transparent. Kept as a source file.
- `favicon.svg`: a droplet icon.

## Design rules (don't change without asking)
- Dark, restrained, "tech product" look. Palette tokens live in `:root`. There's no bright accent. `--signal` is used only in tiny touches.
- Fonts: Geist and Geist Mono from Google Fonts.
- Hero: a canvas point-cloud droplet with a scan line. Keep it subtle.
- Section order: hero, statements, blurred readout, COMING SOON, early-access form, footer.

## Tasks to go live
1. **Waitlist form:** `FORM_ENDPOINT` in `index.html` is a placeholder (`https://formspree.io/f/YOUR_FORM_ID`). Replace it with the owner's real Formspree form endpoint, or set up an alternative the owner approves. Test that a submission arrives.
2. **Deploy to Vercel** as a static site (no framework, output = repo root).
3. **Connect the domain `emvicto.com`**, registered at GoDaddy. Add `emvicto.com` and `www.emvicto.com` in Vercel, redirect www to the apex, then give the owner the exact DNS records Vercel shows so they can add them in GoDaddy DNS.
4. Nice-to-have: an OG share image (1200×630, dark with the logo) and `robots.txt`.
