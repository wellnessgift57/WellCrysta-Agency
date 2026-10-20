WELLCRYSTA WEBSITE — SETUP GUIDE (v3)
=====================================

WHAT'S INSIDE (all links are relative — keep this folder structure)
  index.html, about.html, contact.html, consultation.html, 404.html
  robots.txt, sitemap.xml, site.webmanifest     -> SEO / mobile install files
  images/                                        -> WebP photos (480/800/1200 px), logo, icons, social share image
     logo-full-light.png / logo-full-dark.png    -> full logo for print, social profiles, proposals
     mark.svg / mark-dark.svg                    -> logo emblem (light / dark backgrounds)
     og-image.jpg                                -> preview image when your link is shared on WhatsApp/LinkedIn/Facebook

HOW TO EDIT
  Design (CSS) and script (JS) are minified and inlined inside each .html file for the best PageSpeed score.
  To change wording, open the .html file in any text editor and edit the visible text.
  The site header, footer and WhatsApp number repeat on every page, so use Find & Replace across all 5 .html files.

STEP 1 — REPLACE PLACEHOLDERS (Find & Replace in all .html files)
  Phone, WhatsApp and email are already set (+91 90826 30433, wellnessgift57@gmail.com)
  "https://wellcrysta.com"          -> your final domain (canonical links, sitemap, structured data)
  "YOUR_WEB3FORMS_ACCESS_KEY"       -> contact.html + consultation.html (key from web3forms.com; enquiries go to your Gmail)
  "GTM-XXXXXXX"                     -> your Google Tag Manager ID (appears in the <html> tag of every page)

STEP 2 — PUBLISH
  Upload everything to the site root (GitHub Pages / Hostinger). index.html must be at the root.
  Make sure the site opens on https (SSL).

STEP 3 — SEO AFTER GOING LIVE
  - Google Search Console: add the domain, submit  https://YOURDOMAIN/sitemap.xml
  - Test structured data: search.google.com/test/rich-results

STEP 4 — TEST SPEED
  pagespeed.web.dev -> enter your live URL. Test the LIVE https site, not a local file.

TRACKING (GTM dataLayer events already built in)
  whatsapp_click, call_click, email_click, cta_consultation_click  (param: link_location)
  generate_lead (param: form_name = contact | consultation) — fires only on successful submit
  GTM loads on first scroll/tap or after 5 seconds, so it does not slow the first paint.

CHANGES IN THIS VERSION (v3.1: Home "What we do" heading now reads "Growth performance digital marketing services")

CHANGES IN v3
  Contact:  office location, working hours and map removed (also removed from footer and search-engine data)
  About:    "Our story" rewritten; "What we will never do" section removed
  Header:   "Services" now opens the "Our services" section on the Home page (from every page)
  Home:     "How a customer finds and books you" moved above "The real problem"
            "Meta Pixel + Conversions API" removed everywhere (13 deliverables remain)
            "The WellCrysta Growth Path" -> "The WellCrysta Foundation Plan"
            "100% key events" and "14 deliverables" text removed (hero cards removed)
            moving line removed
            "Ads don't fail. Foundations do." rephrased (no direct mention of ads)
            Foundation Setup: "Custom quote after free audit" removed
