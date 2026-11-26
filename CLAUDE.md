# KSM Consulting – New Website

## Goal
Build a brand-new, fully custom static website for ksmconsulting.org
using the content in /wp-export. New design only — no content changes.

## About me
I'm not a developer, but I understand the basics (I work mainly in WordPress).
- Explain terminal commands in plain language before asking me to run them.
- Keep explanations short and step-by-step.
- Ask before making big structural decisions.

## Where the content is
- /wp-export/markdown – page and post content (one folder per page/post, with its images)
- /wp-export/urls.md – full list of live URLs
- /wp-export/seo.md – SEO title and meta description for each page
- /wp-export/site-wide.md – header, navigation and footer content (phone, email, address, social links)
- /wp-export/forms.md – every form, its fields, recipient email and thank-you message
- /wp-export/brand – logo, favicon, Open Graph and other brand images
- /wp-export/html – saved rendered HTML of every live page (backup reference)

## Content rules (strict)
- Do NOT rewrite, shorten, or "improve" any wording. Use text exactly as in /wp-export.
- Keep every page and the same URL slugs (see /wp-export/urls.md).
- Use SEO titles and meta descriptions from /wp-export/seo.md.
- Use header, navigation and footer content from /wp-export/site-wide.md.
- Rebuild forms as listed in /wp-export/forms.md.
- Use images from /wp-export/markdown and /wp-export/brand.
- If page content in /wp-export/markdown looks incomplete, use the saved HTML in /wp-export/html.
- If content is missing or unclear, ask me rather than inventing it.
- Never change anything on the live WordPress site.

## Design
- Modern, professional look for a WordPress development & digital
  marketing consultancy serving small businesses and CEO-level clients.
- Mobile-first, fast, accessible (good contrast, alt text, keyboard-friendly).
- Propose 2–3 design directions and let me choose before building.

## Tech
- Static site built with Astro, using the Markdown content in /wp-export/markdown.
- Blog posts as Markdown files so new posts can be added easily.
- Contact form via Web3Forms or Formspree (no server code — Hostinger serves static files only).
- Include a sitemap and robots.txt.
- Keep page titles, meta descriptions and Open Graph tags on every page.

## Hosting – Hostinger
- Hostinger (Apache/LiteSpeed) serves the files in the built /dist folder.
- Put any redirects from old WordPress URLs in an .htaccess file in /public
  so it is included in every build.
- Deployment for now: I run `npm run build` and upload the contents of /dist
  to public_html via Hostinger File Manager.
- Test on a subdomain (new.ksmconsulting.org) before going live; block search
  engines from the test subdomain.

## Working style
- Commit-sized steps: finish one piece, tell me what changed, then move on.
- Before calling the site done, compare the text on every page against
  /wp-export and list any differences.
