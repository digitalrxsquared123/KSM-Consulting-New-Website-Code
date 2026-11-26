# Site-wide content (header, navigation, footer)

Taken from the live site on 2026-11-26. The header and footer are identical on every page
(checked across all 47 sitemap URLs).

> **No phone number, email address or postal address appears anywhere on the live site**
> (not in the header, footer, contact page or structured data). Only social links are shown.

## Header

- **Logo:** `brand/Logo-truncated-transparent-BG.webp`, shown at 250×119, alt text "KSM Consulting", links to the home page.
- **Button (right side):** "Get in touch" → `/contact-us/`
- **Accessibility:** "Skip to content" link at the top of every page.
- On mobile the menu collapses behind an "Open menu" / "Close menu" button.

### Main navigation ("Header menu")

| Label | Link | Sub-menu |
|---|---|---|
| Home | `/` | – |
| About us | `/about-us/` | Website examples → `/website-examples-for-business/` |
| Services | `/digital-growth-marketing-services/` | – |
| Methodology | `/digital-marketing-methodology/` | – |
| Blog | `/blog/` | Privacy Policy → `/privacy-policy/` |
| Contact Us | `/contact-us/` | – |

## Footer

### Column 1 – About

**KSM Consulting**

Leverage our full suite of digital growth marketing services from content infused website development to SEO to paid campaign management and more and get your business on the fast track.

Social links (shown as icons, labelled):

- LinkedIn → https://www.linkedin.com/company/ksm-consulting-digital/
- Facebook → https://www.facebook.com/ksmconsultingllc

### Column 2 – Company ("Footer menu 1")

- About us → `/about-us/`
- Contact Us → `/contact-us/`
- Privacy Policy → `/privacy-policy/`

### Column 3 – Services ("Footer menu 3")

- Services → `/digital-growth-marketing-services/`
- Methodology → `/digital-marketing-methodology/`

### Column 4 – Resources ("Footer menu 2")

- Blog → `/blog/`
- Website examples → `/website-examples-for-business/`

### Bottom bar (below a divider line)

- **Copyright line:** © 2026 · Powered by KSM Consulting
- **Links ("Footer menu 4"):** Privacy Policy → `/privacy-policy/` · Contact Us → `/contact-us/`

## Tracking and third-party scripts (for reference)

- **Google Tag Manager:** container `GTM-M3R2DX6V` (on every page).
- **Google Site Kit** plugin is installed.
- **Contact form conversion event:** after a successful contact-form submission, the site pushes
  `{ event: 'cf7submission', formId, formTitle }` to the GTM `dataLayer`. Any GTM conversion
  tags that rely on this event will need an equivalent on the new site.
- **Google reCAPTCHA v3** is loaded on pages with the contact form (site key `6LcmOuIhAAAAAIRyOTryIXETPcxDVYZzOUOXOIz2`).
