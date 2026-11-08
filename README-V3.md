# Chozhan Foundation V3 — GitHub Pages upgrade

## Deploy safely
1. In GitHub, create a backup branch or download your currently working repository before uploading.
2. Extract this ZIP. Upload **the contents** of the folder to the repository root (alongside `index.html`), not the folder itself.
3. **Keep the existing CNAME file** if GitHub Pages uses `chozhan.org`. This package deliberately does not replace it.
4. Commit and wait for GitHub Pages. Hard refresh and test homepage, Gallery, Volunteer, Tamil switch, and WhatsApp on desktop/mobile.
5. If the layout breaks, revert the commit in GitHub.

## What works
- Existing working design and logo retained; logo width constrained to 60px.
- Tamil/English switch: existing key-content translations plus additional interface and page-heading translations. **Not all long-form copy is translated**; review remaining English text before describing the site as fully bilingual.
- Gallery placeholders are retained until approved real images are provided.
- Gallery events section loads verified events from `events.json`. Empty list displays the existing no-events notice.
- Contact WhatsApp: https://wa.me/917305449549
- Contact email: chozhan.org@gmail.com
- Address: 39, Ramanathan Nagar, Koothapakkam, Cuddalore – 607002, Tamil Nadu, India.
- Impact statistics remain at zero; do not publish unsupported claims.

## Publish an event
Edit `events.json` in GitHub. Use `events-example.json` as a template. Enter verified title, ISO date (YYYY-MM-DD), location and description, then set `published` to true. **The example is NOT published.** Changes go live after committing. This is GitHub-managed event publishing, **not an admin dashboard**.

## Volunteer form
GitHub Pages is static and cannot securely store registrations or send server-side confirmation emails by itself. The existing volunteer form opens a mailto draft, and visitors must send it. Do not describe this as a stored online registration. To implement actual online registration, connect an approved backend/form service with privacy controls, spam prevention, and consent. Never put API secrets in this repository.

## SEO
Retains existing sitemap.xml, robots.txt, canonical and social metadata; added locale hints and theme color. Google indexing is not guaranteed. Verify domain and sitemap in Search Console. If your canonical domain changes, update metadata and sitemap.

## Privacy
Do not publish personal contact data, children's images, or volunteer information without appropriate consent. Event and gallery content should be approved before publication.
