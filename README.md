# FORM — Designer Archive

A static concept storefront for CS001 / Introduction to Computing and Web Design. Plain HTML5 and CSS3 only; no JavaScript, framework, backend, database, installation or build step. Displayed prices are classroom reference values, not offers or appraisals. Every page states: “Concept store. Items are not for sale.”

**Public GitHub repository:** https://github.com/jaennviel/form  
**Live Vercel website:** https://form-vert-psi.vercel.app  
**Restricted working preview:** https://form-clothing-ipad.ciit-4080.chatgpt.site  
**Section:** `[Your section]`  
**Deadline:** `[Instructor to specify]`

Solo work is instructor-approved, as confirmed by the student. One real member owns one category with ten distinct garments. The public GitHub repository and live Vercel URL are verified above. Personal information and genuine coding contribution evidence remain pending.

| Member | GitHub username | Category | Owned page |
| --- | --- | --- | --- |
| `[Your full name: Last Name, First Name]` | `jaennviel` | Designer Archive — 10 products | `category-1.html` |

## Assignment source and current requirements

The complete supplied `1-Intro_to_Computing_Web_Design_Ecommerce_Project.docx` was reread on 25 November 2026, including all tables and the 100-point rubric. No storefront sentence is required to say “school project” or repeat the assignment explanation. About must retain the store story and member roles; Contact must retain labels, inputs and a submit button.

The Home blueprint lists “Hero banner, store intro, featured picks, category links.” Featured picks is omitted at the student’s latest explicit request. This is a documented exception to that Home blueprint, not a claim of full compliance. The brief requires a styled “View Details” or “Add to Cart” static link. At the student’s latest explicit request, the visible View details labels are omitted. Each Collection card remains one styled native link to its own product page, named from the garment heading and with a visible keyboard focus outline. The omitted wording is a documented exception to the brief’s named-action requirement.

## Files and basic use

Open root `index.html` in a browser, or host the same relative-path files directly. No build command is needed.

```text
index.html                        Hero, introduction and Collection link
category-1.html                   Single Collection page, all 10 garments
product-form-01.html ... -10.html One garment per dedicated page
about.html                        Store story, real member details/placeholders and assigned role
contact.html                      Labeled static inquiry form and no-message-sent result
details.html                      Compatibility landing page linking to Collection
css/style.css                     Shared layout, palette, type, navigation and responsive cards
images/                           Licensed local product, editorial and logo assets
fonts/                            Local Bebas Neue and SIL Open Font License
README.md                         Assignment mapping, CSS explanation, sources and publishing workflow
brand-guidelines.pdf             Implemented visual identity and usage
contribution-submission-sheet.pdf Fillable/printable submission and actual-work record
```

All ten Collection cards include the original image, title and peso price inside one clickable card. Short descriptions are omitted at the student’s latest explicit request; full descriptions remain on each dedicated product page. This is a documented exception to the brief’s per-card description requirement. Each single anchor is named from its garment heading; no separate View details label is displayed. All dedicated product pages retain the garment description, price, design note and complete photo attribution. A “Collection › product name” breadcrumb replaces the Back to collection button; Collection remains a working return link. Previous/Next links follow the displayed Collection order without wrapping at the ends. No garment substitutions from the separate research proposal have been applied.

## Explain all three CSS methods

1. **External:** every page links exactly to `<link rel="stylesheet" href="css/style.css">`. It defines the shared white layout, colors, typography, navigation, footer, responsive Grid/Flexbox cards and interaction styling.
2. **Internal:** `index.html` has a commented `<style>` block in its head. `.home-hero` defines the home-only full-width image layout and background. Its `.hero-copy` places the title/tagline beside the collection link, stacking that copy below 600px.
3. **Inline:** the Home tagline uses `style="letter-spacing: 0.02em;"`. This is a small, intentional one-off tracking override for that promotional line, identified by a source comment. Most styling remains external.

For normal declarations, inline styling takes precedence over ordinary stylesheet rules for the same property. When specificity is equal, later rules override earlier ones: a page-specific internal rule after the external link can specialize a shared rule. These examples need no `!important`; the existing reduced-motion override uses it to honor that preference.

## Developer and course notes

About retains name and section placeholders, the verified GitHub username jaennviel, and the assigned Project owner role. Complete the missing personal details before submission. Actual contributions belong in the submission sheet and the student’s genuine GitHub history.

The Contact form uses a non-modal open `<dialog>` and `<form method="dialog">`. Valid submission closes the dialog without a network request; the adjacent result appears and the Back to form link reloads it. The storefront includes a short no-message-sent note. There is no working cart, checkout, stock system or order processing.

## Design and photography

FORM uses the existing dark geometric wordmark on white, Bebas Neue headings and Arial body copy. The header has no divider. Navigation stays gray when inactive and black for the current section; Collection remains active on product pages. Keyboard focus remains visible. The grayscale editorial hero and gray-to-black View collection link are retained with no underline.

On phones up to 44rem, FORM sits left and a three-dot navigation button sits right. The button opens the same four uppercase links in a full-screen white native HTML popover, with a labeled close button. The browser handles Enter/Space, Escape, and focus restoration; CSS hides the background controls while open. No JavaScript is used. At wider sizes the same navigation is shown inline and aligned to the right in the 224 px tall header. The logo is up to 224 px wide and shrinks with its available column.

The compact menu requires native Popover support (current Chromium, Firefox and Safari/iOS 18.3+). In older browsers without it, the four links stay visible and wrapped beneath the logo; the unsupported menu button stays hidden. This CSS-only fallback preserves navigation without adding a polyfill or script. The open menu also adapts to landscape rotation.

Current lead photography uses the existing 4:5 frames and individual CSS framing. No original photo files were changed in the copy pass. The two strongest flat Raf images have additional padding; the porcelain vest trims spare studio space at scale 1.12. Remaining side/mannequin views were previously accepted by the student. Product colors are not filtered; only the editorial hero is grayscale. Middleman Store was a visual reference, not an image source.

## Genuine contribution and GitHub → Vercel submission

1. Read and be able to explain the HTML landmarks, one card, the three CSS methods and the responsive rules.
2. Make meaningful edits yourself using your real GitHub account. Record only actual work and genuine commit links/SHAs.
3. Add your actual name, section and username in About, this README and the contribution sheet.
4. Use the existing **public** [jaennviel/form](https://github.com/jaennviel/form) repository, with `index.html` at its root. Upload the prepared source and preserve genuine contribution history on `main`.
5. In Vercel, choose Add New → Project, import the public repository and use Framework Preset **Other**. Root Directory must contain `index.html`; use no build/install command and serve the project root (`.`) for this buildless static project.
6. Test the actual HTTPS deployment on desktop and mobile, then push a genuine later change and confirm continuous deployment works.
7. Add the verified GitHub and Vercel URLs to the README and submission sheet. Include the completed sheet and project ZIP in the instructor’s submission. A public Vercel production deployment is now verified; nothing has been submitted to the LMS.

The restricted Sites preview is a working review site; it does not replace the required public GitHub → Vercel workflow.

## Source-check status and rubric mapping

| Criterion | Location / evidence | Status |
| --- | --- | --- |
| HTML5 structure and completeness — 20 | Home, one category, About, Contact and ten product pages; semantic landmarks and relative links | Source checked; no score guaranteed |
| Three CSS methods — 25 | Shared stylesheet, Home head style, Home tagline inline tracking; code comments and explanation above | Source checked |
| Catalog depth — 25 | One approved solo category, 10 products with images, titles, peso prices and clickable cards; full descriptions on product pages | Source checked; card descriptions and named-action wording omitted at student request |
| UI/UX and responsiveness — 15 | Existing white theme, focus, contrast, 4:5 image handling, Grid/Flexbox and responsive rules | Source and local Chromium responsive navigation checks passed; physical-device testing pending |
| GitHub and Vercel — 15 | Public repository and production URL verified; GitHub upload commit automatically deployed on Vercel | Hosting verified; genuine student coding contribution evidence pending |

Personal details, submission-sheet completion and genuine contribution history remain unverified. The current navigation passed local Chromium checks at 320, 390, 704, 705, 768, 1024 and 1440 px widths, including full-screen phone presentation, Enter/Escape/close behavior, focus restoration, product navigation, active sections, and open-menu rotation to desktop and back. All fifteen pages passed phone menu open/close checks. These are viewport simulations; physical iPhone/iPad Safari and assistive-technology testing remain pending. Live source files are verified separately after deployment.

## Local image, logo and font sources

Each image remains local, with its recorded credit and license. Attribution does not claim museum endorsement, ownership, stock, condition or independent authentication. All relevant photo captions and license links remain visible.

<!-- IMAGE-SOURCES:START -->
| Local file / item | Record and original image | Credit / license |
| --- | --- | --- |
| [images/products/form-01.webp](images/products/form-01.webp) — Helmut Lang Nylon Jacket | [Record](https://sammlung.wienmuseum.at/en/object/1009506/) · [Original photo](https://sammlung.wienmuseum.at/images/objects/1009506/420266_full.jpg) | Helmut Lang; Foto: Wien Museum. CC BY 4.0 Wien Museum · [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) |
| [images/products/form-02.webp](images/products/form-02.webp) — Helmut Lang Open-Side Dress | [Record](https://sammlung.wienmuseum.at/en/object/687531/) · [Original photo](https://sammlung.wienmuseum.at/images/objects/687531/686666_full.jpg) | Helmut Lang; Foto: Wien Museum. CC BY 4.0 Wien Museum · [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) |
| [images/products/form-03.webp](images/products/form-03.webp) — Maison Margiela Porcelain Vest | [Record](https://commons.wikimedia.org/wiki/File:Martin_Margiela_Gilet_en_porcelaine.jpg) · [Original photo](https://upload.wikimedia.org/wikipedia/commons/0/00/Martin_Margiela_Gilet_en_porcelaine.jpg) | Martin Margiela / Museum Boijmans Van Beuningen; Wikimedia Commons. CC BY-SA 3.0 · [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| [images/products/form-04.webp](images/products/form-04.webp) — Raf Simons Black Sleeveless Top | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/haut) · [Original photo](https://www.parismuseescollections.paris.fr/sites/default/files/styles/pm_notice/public/atoms/images/GAL/lpdp_88558-14.jpg?itok=I4DzrZa0) | Paris Musées / Palais Galliera, musée de la Mode de la Ville de Paris. CC0 · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-05.webp](images/products/form-05.webp) — Raf Simons Textured Top | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/haut-17) · [Original photo](https://www.parismuseescollections.paris.fr/sites/default/files/styles/pm_notice/public/atoms/images/GAL/lpdp_88558-19.jpg?itok=a1h1Ie6F) | Paris Musées / Palais Galliera, musée de la Mode de la Ville de Paris. CC0 · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-06.webp](images/products/form-06.webp) — Comme des Garçons Tailcoat & Vest | [Record](https://commons.wikimedia.org/wiki/File:Comme_des_gar%C3%A7ons,_giacca_a_marsina_e_gilet,_cotone,_poliesteree_lana,_p-e_2004.jpg) · [Original photo](https://upload.wikimedia.org/wikipedia/commons/4/48/Comme_des_gar%C3%A7ons%2C_giacca_a_marsina_e_gilet%2C_cotone%2C_poliesteree_lana%2C_p-e_2004.jpg) | Sailko; Galleria del Costume, Florence; Wikimedia Commons. CC BY 3.0 · [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/) |
| [images/products/form-07.webp](images/products/form-07.webp) — Jean Paul Gaultier Halter Jumpsuit | [Record](https://commons.wikimedia.org/wiki/File:Gaultier_pink_jumpsuit_(24158).jpg) · [Original photo](https://upload.wikimedia.org/wikipedia/commons/2/24/Gaultier_pink_jumpsuit_%2824158%29.jpg) | Rhododendrites; The Museum at FIT; Wikimedia Commons. CC BY-SA 4.0 · [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| [images/products/form-08.webp](images/products/form-08.webp) — Yohji Yamamoto Printed Dress | [Record](https://commons.wikimedia.org/wiki/File:Yohji_Yamamoto_dress.jpg) · [Original photo](https://upload.wikimedia.org/wikipedia/commons/6/66/Yohji_Yamamoto_dress.jpg) | Photograph by Eileen Costa / The Museum at FIT; Wikimedia Commons. CC BY-SA 2.0 · [CC BY-SA 2.0](https://creativecommons.org/licenses/by-sa/2.0/) |
| [images/products/form-09.webp](images/products/form-09.webp) — Issey Miyake Indigo Batik Dress | [Record](https://commons.wikimedia.org/wiki/File:Issey_Miyake,_Summer_1984_-_Indigo_Batik_Dress_01.jpg) · [Original photo](https://upload.wikimedia.org/wikipedia/commons/5/5d/Issey_Miyake%2C_Summer_1984_-_Indigo_Batik_Dress_01.jpg) | Photographer from the Rhode Island School of Design Museum of Art; Wikimedia Commons. CC0 · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-10.webp](images/products/form-10.webp) — Issey Miyake Gunpowder Dress | [Record](https://commons.wikimedia.org/wiki/File:Gunpowder_Dress_by_Cai_Guo-Qiang_for_Issey_Miyake,_printed_polyester,_1998_01.jpg) · [Original photo](https://upload.wikimedia.org/wikipedia/commons/c/c4/Gunpowder_Dress_by_Cai_Guo-Qiang_for_Issey_Miyake%2C_printed_polyester%2C_1998_01.jpg) | Photographer from the Rhode Island School of Design Museum of Art; Wikimedia Commons. CC0 · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |

All ten product photograph files: proportion-preserving downsize only (maximum 1200 × 1600 pixels), EXIF orientation correction if needed, RGB conversion and WebP compression. No garment removal, recoloring, retouching or file cropping. Collection and featured images share a stationary 4:5 mat. The lead sequence opens with flat-lay and lighter studio photographs; display and exhibition views follow later. The Margiela vest and textured Raf top use selective CSS framing. Original image files, dedicated detail-page images and photo credits are unchanged. Retained image adaptations are offered under the same image license, including each applicable ShareAlike license; those licenses apply to the photos, not the HTML/CSS or unrelated assets.

About continues to use `form-01.webp`. The home hero is the separately credited editorial rack photograph below. Required Wien Museum citations:

Helmut Lang (fashion designer), Damenjacke, 1990–1999, Wien Museum Inv.-Nr. M 22627, CC BY 4.0, Foto: Wien Museum (https://sammlung.wienmuseum.at/en/object/1009506/) Edits: optimized and converted to WebP; no crop.

Helmut Lang (fashion designer), Kleid, 1985, Wien Museum Inv.-Nr. M 20067, CC BY 4.0, Foto: Wien Museum (https://sammlung.wienmuseum.at/en/object/687531/) Edits: optimized and converted to WebP; no crop.

Undercover and Number (N)ine were not included because permission-cleared garment images were not established. The student approved two museum-image replacements: Raf Simons Textured Top and Issey Miyake Gunpowder Dress. The Comme des Garçons ensemble is identified from the photographer’s file title; the vest by Martin Margiela is listed under Maison Margiela for contemporary brand recognition. No unsupported dates, measurements, condition, stock or independent authentication are claimed; dates in required museum citations are credited record metadata. Prices are plausible classroom examples, not valuations, source prices or offers.
<!-- IMAGE-SOURCES:END -->

The local [Bebas Neue font](fonts/BebasNeue-Regular.ttf) comes from the [Google Fonts source](https://raw.githubusercontent.com/google/fonts/main/ofl/bebasneue/BebasNeue-Regular.ttf) and is supplied with its [SIL Open Font License](fonts/OFL.txt). The external stylesheet loads it with `@font-face` and `font-display: swap`; readable fallback fonts remain available while it loads.

The original FORM wordmark, primary lockups, monograms, monochrome version, favicon and diagonal-cut pattern were drawn as SVG geometry for this project. They do not come from an icon pack or the garment-image sources. The PNG icons are exports of `images/brand/favicon.svg`.

## Editorial hero source and edits

Hero: [Vintage clothing displayed on racks in a store — Long Chung](https://unsplash.com/photos/vintage-clothing-displayed-on-racks-in-a-store-6tih6odK1Do), [photographer](https://unsplash.com/@chungj07), [Unsplash License](https://unsplash.com/license). The photo page explicitly identifies this image as free to use under that license; no Unsplash+ license is involved. Editorial atmosphere only, not FORM premises, staff, inventory or a photo of any listed product. Credit is visible below the hero.

Local optimized files: [1600 × 1000 WebP](images/archive-rack-1600.webp) and [800 × 500 WebP](images/archive-rack-800.webp). Source render URL: `https://images.unsplash.com/photo-1770012117407-02aa4bd203ec?fm=webp&w=1600&h=1000&fit=crop&crop=focalpoint&fp-x=0.5&fp-y=0.72&q=78` (800 × 500 variant uses the corresponding width/height). Edits: lower-rack focal crop from the portrait original, proportional resizing and WebP compression through Unsplash’s image server. No recoloring, generative alteration, garment retouching or brand overlay. Responsive `srcset` loads a smaller file when suitable; CSS cover framing fills the existing desktop/mobile image frame without distortion.

Only this editorial hero has a CSS grayscale filter. Product files retain their source colors.

## Current publication and verification — 26 November 2026

The student uploaded the prepared source in commit [21861c4](https://github.com/jaennviel/form/commit/21861c4c52f7ab10187b340ebced87608ba0e544), “Add FORM Designer Archive website and product catalog.” Vercel automatically built that GitHub main-branch commit as a Ready production deployment. Public HTTP checks passed for Home, Collection, About, Contact, all ten product pages, the shared stylesheet, ten product images, the editorial hero and wordmark. All ten card/detail prices match and Back to collection links resolve. No browser/device visual tests or interactive Contact tests are claimed.

The latest change removes only Home’s Featured picks section. The hero, tagline, introduction, collection link, ten Collection cards and product pages are retained. All three commented CSS methods remain: shared external CSS on every page, internal Home hero styling, and inline tagline tracking. Photo files, source credits and license notices are unchanged.

The GitHub-to-Vercel connection remains enabled. The student synced the homepage and handoff documents in commit [2b62031](https://github.com/jaennviel/form/commit/2b620317295802b9fe2f73ee9b100f95d30f1cdf), “Remove Featured picks and update project links.” Vercel automatically deployed that commit to production, and public Home and Collection checks matched the reviewed files. The repository and site both omit Featured picks.

The GitHub connector has now been installed and authorized for this account. Repository push permission and a GitHub blob write were both confirmed on 26 November 2026. The previous manual-sync limitation is resolved; future authorized updates can use the normal GitHub-to-Vercel workflow. This documentation update does not change the storefront.

The submission sheet includes the verified GitHub URL, Vercel URL and username jaennviel. Full name, section, deadline and actual coding contribution record remain for the student to complete. The existing restricted FORM preview retains its access settings. No domain was purchased and nothing was submitted for class.


## Product-page navigation and visible information

Each of the ten product pages has a labeled, ordered breadcrumb trail and separate Previous/Next product links. The first piece has only Next; the last has only Previous. The main header still marks Collection as active. No product, photo, crop, price or source wording changed.

The photo, designer-first product title and PHP reference price stay visible; the redundant standalone designer line is removed. Product-page titles use regular Arial at 28–40 px and prices use regular Arial at 20 px (at the default root text size). The original description, “Why it’s here” note and complete source/license credit are now visible as plain text. At widths above 600 px the photo is on the left and all product information on the right; phones stack the photo above the text. No dropdowns or + controls remain on product pages. Full license links remain visible and are recorded in the image-source table above.

Source checks confirmed that all original product paragraphs, images and credit links are preserved, all neighbor and collection destinations resolve, and the three CSS methods remain. Local Chromium checks passed at 320 × 740, 390 × 844, 768 × 1024, 1024 × 768 and 1440 × 1000 for visible product information, regular typography, responsive side-by-side/stacked layout, focus, and product/collection navigation. All ten pages also passed image-loading and phone-header-menu checks. Physical Safari/iPad and assistive-technology verification remain pending.
