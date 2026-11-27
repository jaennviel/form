# FORM — Designer Archive

A static concept storefront for CS001 / Introduction to Computing and Web Design. Plain HTML5 and CSS3 only; no JavaScript, framework, backend, database, installation or build step. Displayed prices are classroom reference values, not offers or appraisals. Every page states: “Concept store. Items are not for sale.”

**Public GitHub repository:** https://github.com/jaennviel/form  
**Live Vercel website:** https://form-vert-psi.vercel.app  
**Restricted working preview:** https://form-clothing-ipad.ciit-4080.chatgpt.site  
**Section:** CS001 - 2

**Deadline:** `[Instructor to specify]`

Solo work is instructor-approved, as confirmed by the student. One real member owns one category with ten distinct products: nine garments and one bag. The public GitHub repository and live Vercel URL are verified above. The member name and section were provided by the student; genuine coding contribution evidence remains pending.

| Member | GitHub username | Category | Owned page |
| --- | --- | --- | --- |
| Jaenn Viel F. Francisco | `jaennviel` | Designer Archive — 10 products | `category-1.html` |

## Assignment source and current requirements

The complete supplied `1-Intro_to_Computing_Web_Design_Ecommerce_Project.docx` was reread on 25 November 2026, including all tables and the 100-point rubric. No storefront sentence is required to say “school project” or repeat the assignment explanation. About must retain the store story and member roles; Contact must retain labels, inputs and a submit button.

The Home blueprint lists “Hero banner, store intro, featured picks, category links.” Featured picks is omitted at the student’s latest explicit request. This is a documented exception to that Home blueprint, not a claim of full compliance. The brief requires a styled “View Details” or “Add to Cart” static link. At the student’s latest explicit request, the visible View details labels are omitted. Each Collection card remains one styled native link to its own product page, named from the garment heading and with a visible keyboard focus outline. The omitted wording is a documented exception to the brief’s named-action requirement.

## Files and basic use

Open root `index.html` in a browser, or host the same relative-path files directly. No build command is needed.

```text
index.html                        Hero, introduction and Collection link
category-1.html                   Single Collection page, all 10 products
product-form-01.html ... -10.html One product per dedicated page
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

All ten Collection cards include their matching local image, title and peso price inside one clickable card. The grid uses four columns above 1100px, three from 801–1100px, and two at 800px and below, including phones. On phones the column gap is 1rem, image mats keep a consistent 4:5 ratio, and regular-weight names and prices stay centered underneath. Short descriptions are omitted at the student’s latest explicit request; full descriptions remain on each dedicated product page. This is a documented exception to the brief’s per-card description requirement. Each single anchor is named from its garment heading; no separate View details label is displayed. All dedicated product pages retain the garment description, price, design note and complete photo attribution. A “Collection › product name” breadcrumb replaces the Back to collection button; Collection remains a working return link. Previous/Next links follow the displayed Collection order without wrapping at the ends. The approved white-background lineup contains nine Raf Simons garments and one Raf Simons bag. The ten existing product URLs are retained, with each listing updated to match its photograph.

## Explain all three CSS methods

1. **External:** every page links exactly to `<link rel="stylesheet" href="css/style.css">`. It defines the shared white layout, colors, typography, navigation, footer, responsive Grid/Flexbox cards and interaction styling.
2. **Internal:** `index.html` has a commented `<style>` block in its head. `.home-hero` defines the home-only full-width editorial image and centered introduction block. Its `.hero-copy` groups the title, tagline, introduction and collection link in one column. The photo uses a 2:1 crop on wider screens and 4:3 below 600px; the original image and source credit are retained.
3. **Inline:** the Home tagline uses `style="letter-spacing: 0.02em;"`. This is a small, intentional one-off tracking override for that promotional line, identified by a source comment. Most styling remains external.

For normal declarations, inline styling takes precedence over ordinary stylesheet rules for the same property. When specificity is equal, later rules override earlier ones: a page-specific internal rule after the external link can specialize a shared rule. These examples need no `!important`; the existing reduced-motion override uses it to honor that preference.

## Developer and course notes

About presents original manifesto copy under “Our point of view” and “Look beyond the label.” The text uses a bold Arial statement (40–64 px) and larger regular Arial body copy (20–26 px), scaling with the root font size. A collection link follows, along with a compact member credit: Jaenn Viel F. Francisco, section CS001 - 2, GitHub username jaennviel, and Project owner for Designer Archive. The required story and member role remain. About remains text-only; the current licensed product photographs and their full credits appear on the matching product pages and in the source log. Actual contributions belong in the submission sheet and the student’s genuine GitHub history.

The Contact form uses a non-modal open `<dialog>` and `<form method="dialog">`. Valid submission closes the dialog without a network request; the adjacent result appears and the Back to form link reloads it. The storefront includes a short no-message-sent note. There is no working cart, checkout, stock system or order processing.

## Design and photography

FORM uses the existing dark geometric wordmark on white, Bebas Neue headings and Arial body copy. The header has no divider. Navigation stays gray when inactive and black for the current section; Collection remains active on product pages. Keyboard focus remains visible. The grayscale editorial hero and gray-to-black View collection link are retained with no underline.

On phones up to 44rem, FORM sits left and a three-dot navigation button sits right. The button opens the same four uppercase links in a full-screen white native HTML popover, with a labeled close button. The browser handles Enter/Space, Escape, and focus restoration; CSS hides the background controls while open. No JavaScript is used. At wider sizes the same navigation is shown inline and aligned to the right in the 224 px tall header. The logo is up to 224 px wide and shrinks with its available column.

The compact menu requires native Popover support (current Chromium, Firefox and Safari/iOS 18.3+). In older browsers without it, the four links stay visible and wrapped beneath the logo; the unsupported menu button stays hidden. This CSS-only fallback preserves navigation without adding a polyfill or script. The open menu also adapts to landscape rotation.

The approved ten-piece lineup uses Raf Simons photographs from Paris Musées / Palais Galliera with explicit CC0 notices on the selected image views. All local lead files are 1000 × 1250 pixels on pure white. Non-generative background segmentation and reviewed edge cleanup retain source garment pixels; proportional scaling fits each item within an 840 × 1050 content area. No garment pixels were generated or recolored. The same white files appear on product pages. Product images remain stationary and in true source color; only the editorial hero is grayscale. Middleman Store was a visual reference, not an image source.

## Genuine contribution and GitHub → Vercel submission

1. Read and be able to explain the HTML landmarks, one card, the three CSS methods and the responsive rules.
2. Make meaningful edits yourself using your real GitHub account. Record only actual work and genuine commit links/SHAs.
3. Review your supplied name (Jaenn Viel F. Francisco), section (CS001 - 2) and username (jaennviel) in About, this README and the contribution sheet.
4. Use the existing **public** [jaennviel/form](https://github.com/jaennviel/form) repository, with `index.html` at its root. Upload the prepared source and preserve genuine contribution history on `main`.
5. In Vercel, choose Add New → Project, import the public repository and use Framework Preset **Other**. Root Directory must contain `index.html`; use no build/install command and serve the project root (`.`) for this buildless static project.
6. Test the actual HTTPS deployment on desktop and mobile, then push a genuine later change and confirm continuous deployment works.
7. Add the verified GitHub and Vercel URLs to the README and submission sheet. Include the completed sheet and project ZIP in the instructor’s submission. A public Vercel production deployment is now verified; nothing has been submitted to the LMS.

The older restricted Sites preview does not replace the required public GitHub → Vercel workflow; the Vercel address above is the current site.

## Source-check status and rubric mapping

| Criterion | Location / evidence | Status |
| --- | --- | --- |
| HTML5 structure and completeness — 20 | Home, one category, About, Contact and ten product pages; semantic landmarks and relative links | Source checked; no score guaranteed |
| Three CSS methods — 25 | Shared stylesheet, Home head style, Home tagline inline tracking; code comments and explanation above | Source checked |
| Catalog depth — 25 | One approved solo category, 10 products with images, titles, peso prices and clickable cards; full descriptions on product pages | Source checked; card descriptions and named-action wording omitted at student request |
| UI/UX and responsiveness — 15 | Existing white theme, focus, contrast, 4:5 image handling, Grid/Flexbox and responsive rules | Source and local Chromium responsive navigation checks passed; physical-device testing pending |
| GitHub and Vercel — 15 | Public repository and production URL verified; GitHub upload commit automatically deployed on Vercel | Hosting verified; genuine student coding contribution evidence pending |

The student supplied the displayed name and section. Submission-sheet completion and genuine coding contribution evidence remain unverified. For this photo pass, local Chromium checks passed at 320 × 740, 390 × 844, 768 × 1024, 1024 × 768 and 1440 × 1000: all ten card/product/return links, matching photos and prices, 4:5 white frames, centered regular labels, visible card focus, no horizontal overflow, and responsive product information. All fifteen phone menus open and close with Escape. Existing focus return after Escape is inconsistent in Chromium; the unchanged header is outside this photography pass. The Contact form passed native required-field validation and local completion without a POST request. All local page/assets paths, source credits and three commented CSS methods passed source checks. Physical iPhone/iPad Safari and assistive-technology testing remain pending. Live source files are verified separately after deployment.

## Local image, logo and font sources

Each image remains local, with its recorded credit and license. Attribution does not claim museum endorsement, ownership, stock, condition or independent authentication. All relevant photo captions and license links remain visible.

<!-- IMAGE-SOURCES:START -->
| Local file / item | Museum record / inventory | Photo credit and license |
| --- | --- | --- |
| [images/products/form-04.webp](images/products/form-04.webp) — Raf Simons Black Sleeveless Top | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/haut) · 2015.43.1.1 | CC0 Paris Musées / Palais Galliera, musée de la Mode de la Ville de Paris · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-06.webp](images/products/form-06.webp) — Raf Simons V-neck Jacket | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/veste-565) · 2015.43.2.1 | CC0 Paris Musées / Palais Galliera, Musée de la Mode de la Ville de Paris · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-07.webp](images/products/form-07.webp) — Raf Simons Lettered Jacket | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/veste-585) · 2015.43.4.1 | CC0 Paris Musées / Palais Galliera, musée de la Mode de la Ville de Paris · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-01.webp](images/products/form-01.webp) — Raf Simons Ivory Coat | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/manteau-306) · 2015.43.3.1 | CC0 Paris Musées / Palais Galliera, musée de la Mode de la Ville de Paris · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-05.webp](images/products/form-05.webp) — Raf Simons Textured Sleeveless Top | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/haut-17) · 2015.43.2.2 | CC0 Paris Musées / Palais Galliera, musée de la Mode de la Ville de Paris · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-02.webp](images/products/form-02.webp) — Raf Simons Black Trousers | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/pantalon-404) · 2015.43.4.2 | CC0 Paris Musées / Palais Galliera, musée de la Mode de la Ville de Paris · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-03.webp](images/products/form-03.webp) — Raf Simons Bermuda Shorts | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/bermuda-de-defile) · 2015.43.1.2 | CC0 Paris Musées / Palais Galliera, Musée de la Mode de la Ville de Paris · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-08.webp](images/products/form-08.webp) — Raf Simons Textured Shorts | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/short-4) · 2015.43.2.3 | CC0 Paris Musées / Palais Galliera, musée de la Mode de la Ville de Paris · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-09.webp](images/products/form-09.webp) — Raf Simons Black Pleated Shorts | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/short-5) · 2015.43.3.2 | CC0 Paris Musées / Palais Galliera, musée de la Mode de la Ville de Paris · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| [images/products/form-10.webp](images/products/form-10.webp) — Raf Simons Black-and-White Bag | [Record](https://www.parismuseescollections.paris.fr/fr/palais-galliera/oeuvres/sac-322) · 2015.43.1.3 | CC0 Paris Musées / Palais Galliera, musée de la Mode de la Ville de Paris · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |

[Detailed product image source log](images/products/sources.csv) records each exact original image URL, inventory number, credit, license, source SHA-256 and edit method. The selected full-object photograph for the bag is the first image view, not its close-up. Each view’s explicit CC0 notice was checked on 27 November 2026.

Edits: source-pixel alpha cutouts using non-generative background segmentation, shadow removal and reviewed silhouette/edge cleanup; proportional Lanczos resizing and compositing onto #FFFFFF; lossless WebP output at 1000 × 1250 pixels (4:5). Full sleeves, hems and bag handles remain visible. Each item is centered within the same maximum 840 × 1050 pixel content area; aspect ratios are retained without stretching. The photographs are not AI recreations. No garment recoloring, invented detail, dates, measurements, condition or provenance is claimed. All ten image adaptations remain available under CC0.

The student approved the new lineup, including the bag, before application. Two original Raf garment listings are retained; the other eight listings now identify their new exact products. Demo PHP prices are classroom examples, not source prices, valuations or offers. The catalog does not claim museum/designer endorsement, authentication or physical stock.
<!-- IMAGE-SOURCES:END -->

The local [Bebas Neue font](fonts/BebasNeue-Regular.ttf) comes from the [Google Fonts source](https://raw.githubusercontent.com/google/fonts/main/ofl/bebasneue/BebasNeue-Regular.ttf) and is supplied with its [SIL Open Font License](fonts/OFL.txt). The external stylesheet loads it with `@font-face` and `font-display: swap`; readable fallback fonts remain available while it loads.

The original FORM wordmark, primary lockups, monograms, monochrome version, favicon and diagonal-cut pattern were drawn as SVG geometry for this project. They do not come from an icon pack or the garment-image sources. The PNG icons are exports of `images/brand/favicon.svg`.

## Editorial hero source and edits

Hero: [Vintage clothing displayed on racks in a store — Long Chung](https://unsplash.com/photos/vintage-clothing-displayed-on-racks-in-a-store-6tih6odK1Do), [photographer](https://unsplash.com/@chungj07), [Unsplash License](https://unsplash.com/license). The photo page explicitly identifies this image as free to use under that license; no Unsplash+ license is involved. Editorial atmosphere only, not FORM premises, staff, inventory or a photo of any listed product. Credit is visible below the hero.

Local optimized files: [1600 × 1000 WebP](images/archive-rack-1600.webp) and [800 × 500 WebP](images/archive-rack-800.webp). Source render URL: `https://images.unsplash.com/photo-1770012117407-02aa4bd203ec?fm=webp&w=1600&h=1000&fit=crop&crop=focalpoint&fp-x=0.5&fp-y=0.72&q=78` (800 × 500 variant uses the corresponding width/height). Edits: lower-rack focal crop from the portrait original, proportional resizing and WebP compression through Unsplash’s image server. No recoloring, generative alteration, garment retouching or brand overlay. Responsive `srcset` loads a smaller file when suitable; CSS cover framing fills the existing desktop/mobile image frame without distortion.

Only this editorial hero has a CSS grayscale filter. Product files retain their source colors.

## Current publication and verification — 27 November 2026

The existing public repository is connected to Vercel for automatic production deployments from `main`. The approved white-background photo pass updates all ten listings and their matching details, source records and demo prices while retaining their dedicated URLs. Home’s grayscale hero, the About manifesto, the labeled static Contact form and the existing responsive navigation remain in place. The prior working version is preserved in Git history and a local backup.

The submission sheet includes the verified GitHub URL, Vercel URL and username jaennviel. The supplied name and section are filled in. The deadline and actual coding contribution record remain for the student to complete. The older restricted Sites preview is not the current publishing target; its availability has not been verified. No domain was purchased and nothing was submitted for class.

## Product-page navigation and visible information

Each of the ten product pages has a labeled, ordered breadcrumb trail and separate Previous/Next product links. The first piece has only Next; the last has only Previous. The main header still marks Collection as active. Neighbor links follow the approved new lineup; every title, photo, demo price and credit identifies the same exact product.

The photo, designer-first product title and PHP reference price stay visible; the redundant standalone designer line is removed. Product-page titles use regular Arial at 28–40 px and prices use regular Arial at 20 px (at the default root text size). The matching description, “Why it’s here” note and complete source/license credit are now visible as plain text. At widths above 600 px the photo is on the left and all product information on the right; phones stack the photo above the text. No dropdowns or + controls remain on product pages. Full license links remain visible and are recorded in the image-source table above.

The current source and viewport checks are listed above. The dedicated product-page URLs are preserved while their product identities, photos, descriptions, demo prices and credits now match the approved lineup.
