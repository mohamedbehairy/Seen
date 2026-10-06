SEEN MEDIA — BILINGUAL WEBSITE DEMO
===================================

PROJECT OVERVIEW
Seen Media (سين للإعلام والدعاية) is presented in this demo as a creative
agency serving brands in the United Arab Emirates and the GCC. The website
introduces digital marketing, content production, and event coverage
through a single-page English and Arabic experience.

The brand message is "Be seen. Be remembered." The design combines deep
green backgrounds, light sections, large typography, cinematic imagery,
and Seen's logo and visual identity assets.

This is a static front-end demo with working language switching, filters,
service selection, and contact handoff. It has no backend, CMS, database,
account system, or server-side inquiry storage.

PAGE CONTENT
1. Header: Seen branding, section navigation, language switch, contact CTA,
   and collapsible mobile navigation.
2. Hero: full-width photograph, bilingual headline, Seen logo, introductory
   copy, and links to start a project or explore services.
3. Brand ticker: animated messages introducing Seen's positioning.
4. About: cinematic storytelling and data-driven marketing, with a
   word-by-word scroll highlight. Local SVG flags represent the UAE,
   Saudi Arabia, Qatar, Kuwait, Bahrain, and Oman.
5. Services: expandable descriptions for Digital Marketing, Content
   Production, and Event Coverage. Opening a service closes the others.
   Service links preselect the relevant option in the inquiry form.
6. Industries: restaurants and cafes, clinics, personal care and cosmetics,
   sports academies, and health and wellness products. Filters show all
   sectors, hospitality, health and beauty, or sport.
7. Portfolio: eight showcase entries with independent filters and a live
   visible-project count:
   - Websites: Alfanar, Maadaniyah, and QDVC.
   - Company profiles: Aura Events, Ewan Real Estate, and Breeze Solutions.
   - Visual identity: The Seen signature and Made to be remembered.
   Entries display images and captions, without project detail pages.
8. Contact and footer: contact information, inquiry form, service and
   portfolio links, WhatsApp and email links, and back-to-top navigation.

LANGUAGES AND TYPOGRAPHY
- English is the default language on a first visit.
- The selected language is saved as "seen-language" in localStorage when
  browser storage is available.
- Arabic switches the document language and direction to Arabic/RTL.
  Copy, labels, image alternatives, page title, and selected logos update.
- Arabic uses Alexandria, loaded through Google Fonts.
- The current Google Fonts link requests Alexandria and Comfortaa.
  English CSS declares DM Sans for body text and Manrope for headings.
  Those two families are not loaded by this link, so Arial/sans-serif
  fallbacks apply when they are unavailable on the device.
- Translations are stored in HTML data attributes and JavaScript arrays.

INTERACTIONS AND ACCESSIBILITY
- Responsive grids, mobile menu, and scroll-dependent header styling.
- Section reveals and scroll-driven philosophy text highlights.
- Decorative cursor, card tilt, and magnetic buttons on fine-pointer devices.
- Reduced-motion preferences disable decorative animation and movement.
- Skip-to-content link, semantic sections, labeled form controls, translated
  accessibility labels, filter pressed states, and portfolio status updates.
- Browser form validation with Arabic feedback in Arabic mode.
These features are implemented; no formal accessibility audit is included.

PROJECT INQUIRY FLOW
Visitors can select multiple services and one industry, then enter:
- Name, email address, and project description (required).
- Company / brand and phone number (optional).

The form validates fields and builds a brief in the selected language.
"Continue on WhatsApp" opens a prepared message for 201158189622.
"Use email instead" opens a mailto draft addressed to info@seen.ae.
The visitor reviews and sends the message in the chosen application.
The website does not send the inquiry itself or confirm delivery.

Displayed contact information:
- Email: info@seen.ae
- Phone: +9710555332714
- Positioning: United Arab Emirates · Serving the GCC

TECHNOLOGY AND FILE STRUCTURE
The project uses HTML, CSS, and vanilla JavaScript. No npm dependencies,
framework, compilation, or build step are required.

index.html                 Page structure, bilingual copy, and font links.
style.css                  Brand styling, typography, responsive layouts,
                           RTL rules, animation, and reduced-motion rules.
app.js                     Language switching, menus, accordions, filters,
                           form handoff, and scroll/pointer effects.
assets/logo.png            Seen Media logo.
assets/mark.png            Seen brand mark and favicon.
assets/identity.webp       Visual identity showcase.
assets/stationery.webp     Branded stationery showcase.
assets/portfolio/          Website and company-profile showcase images.
assets/flags/              Six local SVG flags and their LICENSE.txt.
asset-sources.json         External image sources, photographers, license
                           labels, and recorded download statuses.
README.txt                 Project description and operating instructions.

RUN LOCALLY
For a quick preview, open index.html in a modern browser.
For a local HTTP preview, run the following from the project directory
if Python is installed:

    python -m http.server 8000

Then open http://localhost:8000 in your browser.
Press Ctrl+C in the terminal to stop the server.

EXTERNAL ASSETS AND INTERNET ACCESS
Logos, portfolio images, visual identity images, and flags are local files.
The hero and five industry photographs load from images.unsplash.com.
Fonts load from fonts.googleapis.com and fonts.gstatic.com.
Internet access is needed for those photographs and web fonts; system
fonts are used when the requested fonts cannot load.

asset-sources.json records source pages and attribution details for the
remote photographs. Its download_status entries describe earlier download
attempts, not live network checks. Flag license information is included
in assets/flags/LICENSE.txt. No general project license file is included;
the footer displays Seen Media's copyright notice.

CUSTOMIZATION
- Edit English and Arabic copy together in index.html using data-en and
  data-ar. Preserve translated image and accessibility attributes.
- Edit dynamic service and industry names in the arrays in app.js.
- Adjust colors, spacing, typography, and breakpoints in style.css.
  Later rules override earlier rules, including hero and RTL refinements.
- Replace local imagery while preserving paths, or update image paths in
  index.html. Update asset-sources.json when replacing remote sources.
- Add portfolio entries with the work-item class and data-work-category
  set to websites, profiles, or identity. Include bilingual captions and
  alternative text, and update the initial HTML project-count copy.
- Change contact details in both index.html and app.js, including phone,
  WhatsApp destination, email links, and the form's mailto recipient.

STATIC HOSTING
Upload index.html, style.css, app.js, and the complete assets directory to
your static hosting root, such as public_html. Keep relative paths and
filenames intact. README.txt and asset-sources.json are documentation;
the page does not need them to run.

No Node.js process, application server, environment variables, or build
output is required. These are deployment instructions, not a statement
that this demo has been publicly deployed.

MANUAL REVIEW CHECKLIST
- Switch between English and Arabic; confirm copy, logos, and RTL layout.
- Reload and confirm the selected language is remembered.
- Review desktop and narrow mobile layouts, including mobile navigation.
- Open each service and check that its contact link selects the correct tag.
- Try industry and portfolio filters separately; check portfolio counts.
- Check required fields and invalid email feedback in both languages.
- Confirm WhatsApp and email drafts contain the entered brief; sending
  remains a separate action in the destination app.
- Review motion with the device's reduced-motion preference enabled.
- Check local image paths and remote photo/font loading after hosting.
This checklist describes suggested review steps, not completed test results.

ملخص بالعربية
هذا المشروع نسخة تجريبية لموقع سين للإعلام والدعاية، بواجهة إنجليزية
وعربية واتجاه RTL. يعرض نبذة الشركة، والتسويق الرقمي، وإنتاج المحتوى،
وتغطية الفعاليات، والقطاعات المستهدفة، وثمانية أعمال مع فلاتر مستقلة.
الخط العربي Alexandria. نموذج الاستفسار يجهّز رسالة لواتساب أو البريد
لمراجعتها وإرسالها داخل التطبيق المختار، ولا يتضمن خادمًا لحفظ الطلبات.
يمكن تشغيل الموقع بفتح index.html أو باستخدام خادم Python الموضح أعلاه.
الصور الخارجية والخطوط تحتاج اتصالًا بالإنترنت، أما الشعارات والأعمال
وأعلام الدول فهي ملفات محلية. لتعديل المحتوى والتصميم استخدم index.html
وstyle.css وapp.js مع الحفاظ على النسختين العربية والإنجليزية.

PACKAGE PROVENANCE
Original package source commit:
431acc47bb8e7d18cc8f85cd9833eee7f3ed5032
Retained from the original README. This folder does not contain a Git
repository for verifying that source history.
