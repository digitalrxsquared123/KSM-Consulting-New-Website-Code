# Forms on the live site

Checked every page on 2026-11-26. There is **one form** on the live site, built with
Contact Form 7 (form ID 4531, version 6.2.5). It appears on two pages:

- `/contact-us/` – the real contact page
- `/form-page-testing/` – a test page (same form). **Not moving to the new site** *(owner decision 2026-11-26)*.

No other forms exist (no newsletter signup, search box or comment forms are shown).

## Contact form

Matches the WordPress export entry **"Contact Us Page Form Revised"**
(`markdown/custom/wpcf7_contact_form/contact-form-1_copy/index.md`).

| # | Label (as shown) | Field name | Type | Required | Placeholder | Limits |
|---|---|---|---|---|---|---|
| 1 | FIRST NAME* | `first-name` | text | **Yes** | First Name* | max 400 chars |
| 2 | LAST NAME* | `last-name` | text | **Yes** | Last Name* | max 400 chars |
| 3 | SUBJECT | `subject` | text | No | Subject | max 400 chars |
| 4 | JOB TITLE | `job-title` | text | No | Job Title | max 400 chars |
| 5 | COMPANY | `company` | text | No | Company | max 400 chars |
| 6 | PHONE | `phone-number` | tel | No | Phone | max 400 chars |
| 7 | EMAIL* | `email` | email | **Yes** | Email* | max 400 chars |
| 8 | COMMENTS | `textarea-29` | textarea (5 rows) | No | Enter your comments here | max 2000 chars |

- **Button text:** Submit
- **Layout note:** First Name and Last Name sit together in one row.
- **Spam protection:** Google reCAPTCHA v3 (invisible – no checkbox).
- **On success:** message "Thank you for your message. It has been sent." is shown, and a
  `cf7submission` event is sent to Google Tag Manager.

### Validation / error messages (the ones relevant to these fields; full list in the export file)

- One or more fields have an error. Please check and try again.
- Please fill out this field.
- Please enter an email address.
- Please enter a telephone number.
- This field has a too long input.
- There was an error trying to send your message. Please try again later.

### Emails sent (from the WordPress export – not visible on the live site)

**1. Notification to site owner**

- **To (new site):** raj@ksmconsulting.org *(confirmed by owner 2026-11-26)*
- **To (old WordPress site):** `[_site_admin_email]` – the WordPress admin email.
- **Subject:** New Inquiry on KSM Consulting [subject]
- **Reply-To:** the visitor's email
- **Body:** First Name, Last Name, Subject, Job Title, Company, Phone, Comments, Email

**2. Auto-reply to the visitor**

- **To:** the visitor's email
- **Subject:** Your inquiry on KSM Consulting [subject]
- **Body:**

  > Hi [first-name],
  >
  > Thanks for your form submission. We will be in touch with you soon.
  >
  > Team KSM Consulting
  >
  > -- This email is a receipt for your contact form submission on our website ([_site_title] [_site_url]) in which your email address was used. If that was not you, please ignore this message.

## Older forms in the export (not used on any live page)

- **"Contact form 1"** (`contact-form-1`) – CF7 default form: Your name*, Your email*, Subject*, Your message (optional).
- **"Contact Us Page Form"** (`contact-us-page-form`) – earlier version of the live form (field `your-subject` instead of `subject`; auto-reply says "Our team will be in touch with you soon.").
