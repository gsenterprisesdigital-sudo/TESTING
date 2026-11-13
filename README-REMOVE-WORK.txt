# GS ENTERPRISES DIGITAL — WEBSITE CLEANUP INSTRUCTIONS

Repository: gsenterprisesdigital-sudo/TESTING

Website: https://gsenterprisesdigital-sudo.github.io/TESTING/

## 1. PURPOSE

This document explains how to remove unwanted Our Work and Privacy Policy pages and navigation links while preserving the existing website design and functionality.

Do not replace the current website with older HTML files.

## 2. MAIN WEBSITE PAGES

Maintain these four main pages:

- index.html — Homepage
- services.html — Services
- about.html — About Us
- contact.html — Contact Us

Keep the header, footer, branding, navigation and responsive layout consistent across all four pages.

## 3. REMOVE OUR WORK

- Search all HTML files for `work.html`.
- Remove navigation links pointing to `work.html` where Our Work is no longer required.
- Check desktop navigation, mobile menu and footer links.
- Remove `work.html` from the repository if it is still present and no longer needed.
- Remove its URL from `sitemap.xml`.
- Do not remove unrelated services or portfolio information unless specifically required.

## 4. REMOVE OLD PRIVACY PAGE

- Search all HTML files for `privacy.html`.
- Remove obsolete Privacy Policy navigation links.
- Remove `privacy.html` from the repository if the separate page is no longer required.
- Remove its URL from `sitemap.xml`.

Important: The website uses enquiry forms and analytics. Keep appropriate privacy notices and disclosures wherever legally required. Removing an old page does not remove these obligations.

## 5. FEATURES THAT MUST REMAIN WORKING

Preserve the following:

- GS Enterprises Digital logo and branding.
- Homepage layout and animations.
- Desktop and mobile navigation.
- Services links and cards.
- About and Contact pages.
- View Our Deck Google Drive link.
- Blogger automatic blog updates.
- Existing Tally enquiry form.
- Google Analytics integration.
- Back-to-top button.
- Responsive mobile and tablet layouts.

Do not unintentionally remove or overwrite these features during cleanup.

## 6. UPDATE SITEMAP.XML

Use the correct GitHub Pages base URL:

https://gsenterprisesdigital-sudo.github.io/TESTING/

Keep only valid, published website pages in the sitemap.

Example sitemap for the four main pages:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://gsenterprisesdigital-sudo.github.io/TESTING/</loc>
  </url>
  <url>
    <loc>https://gsenterprisesdigital-sudo.github.io/TESTING/services.html</loc>
  </url>
  <url>
    <loc>https://gsenterprisesdigital-sudo.github.io/TESTING/about.html</loc>
  </url>
  <url>
    <loc>https://gsenterprisesdigital-sudo.github.io/TESTING/contact.html</loc>
  </url>
</urlset>
```

Do not include deleted or missing pages.

## 7. UPDATE ROBOTS.TXT

For a public website, use the correct sitemap location:

```text
User-agent: *
Allow: /

Sitemap: https://gsenterprisesdigital-sudo.github.io/TESTING/sitemap.xml
```

If TESTING is only a staging website, review search indexing requirements separately before publication.

## 8. GITHUB UPDATE PROCEDURE

1. Open the TESTING repository.
2. Select the file that needs updating.
3. Click the Edit (pencil) icon.
4. Make only the required changes.
5. Review the edited code carefully.
6. Click Commit changes.
7. Confirm the commit to the main branch.

To delete an obsolete file:

1. Open the file in GitHub.
2. Select the Delete file option from file actions.
3. Review the deletion.
4. Commit changes.

Deleting a navigation link does not delete the corresponding HTML page.

## 9. FINAL WEBSITE TESTING

After committing changes, verify:

- Homepage opens correctly.
- Services page opens correctly.
- About page opens correctly.
- Contact page opens correctly.
- Logo returns to the homepage.
- Mobile menu opens and closes correctly.
- No unwanted Our Work or Privacy Policy links appear.
- Removed pages are no longer publicly served.
- View Our Deck link works.
- Blogger posts load correctly.
- Tally form opens and submits successfully.
- Enquiry notifications are received.
- No broken internal links remain.
- Sitemap contains only valid URLs.
- Website displays properly on mobile and desktop.

## 10. IMPORTANT NOTES

- Keep a backup before making major changes.
- This README file is documentation only.
- Editing this README does not automatically change the website.
- Previously deployed files must be deleted separately when necessary.
- Avoid replacing updated pages with older ZIP or HTML versions.
- Recheck the published GitHub Pages website after deployment.

## FINAL OBJECTIVE

Maintain a clean, responsive and professional four-page GS Enterprises Digital website with working navigation, enquiry submissions, Blogger integration, Google Analytics, Google Drive deck link and correct SEO configuration.

Remove obsolete pages and links without damaging the existing website.
