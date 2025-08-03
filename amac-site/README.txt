
AMac Charts — Netlify drag‑and‑drop package
===========================================

How to deploy
-------------
1) Upload the *folder* named `amac-site` (or the ZIP contents) to Netlify:
   - Netlify → Your Site → Deploys → "Upload a deploy"
   - Drag the *folder* that contains `index.html`.

2) Make sure `logo.png` sits next to `index.html` (already included).

3) Replace the Stripe links inside index.html:
   - Find `replace-with-your-monthly-link` and `replace-with-your-yearly-link`
   - Paste your real Stripe Checkout URLs.

4) Forms:
   - This page uses Netlify Forms (`contact` and `tv-username`).
   - After first submission, view them in Netlify → Site → Forms.
   - Submissions redirect to /thanks.html, which is included.

5) Custom domain + HTTPS:
   - Add your domain in Netlify → Domain management.
   - Update DNS: A records for the apex (75.2.60.5 and 99.83.190.102), and CNAME for `www` to your `*.netlify.app` URL.
   - Click "Verify DNS configuration" and wait for the SSL certificate to provision.
