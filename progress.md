# North Shore Painting — Progress Tracker

> Last updated: 2026-03-21 (Site created from NORTH-SHORE-TILING fork, adapted for painting)

---

## Site Creation — COMPLETE

| Item | Status | Notes |
|------|--------|-------|
| Forked from NORTH-SHORE-TILING | Done | Clean copy, fresh git init |
| Painting homepage created | Done | New index.html with painting services, trust bar, FAQ, gallery placeholders |
| Accent colour: orange #E07B39 | Done | CSS variables updated from gold #C19A6B |
| Domain: northshorepainting.com.au | Done | All canonical, OG, JSON-LD URLs updated |
| Branding: North Shore Painting | Done | Nav, footer, titles, JSON-LD |
| Email: northshorepainting@gmail.com | Done | All contact sections, JSON-LD |
| Logo: NSPAINTLOGO-HD-FINAL.png | Done | Navbar, footer, hero across all pages |
| Instagram: @northshorepainting | Done | Nav, mobile menu, footer |
| Redirect pages | Done | tiling.html → northshoretiling.com.au, cleaning.html → northshorecleaning.com.au, northshore-removals.html → northshoreremovals.com |
| 17 painting suburb pages | Done | Renamed from tiling-*, content adapted for painting services |
| 2 painting blog posts | Done | Colour selection guide + interior vs exterior paint |
| Landing page | Done | landing/painting.html (was landing/tiling.html) |
| Sitemap rewritten | Done | 22 painting-focused URLs |
| Nav link structure | Done | Painting → index.html (homepage), Tiling → tiling.html (redirect) |
| Tiling images/videos deleted | Done | images/tiling/ and videos/ removed |
| CLAUDE.md rewritten | Done | Painting-specific repo docs |
| .gitignore | Done | Includes *.MOV/*.mov |

---

## REMAINING WORK

### High Priority (blocks launch)

| Item | Blocked By | Notes |
|------|-----------|-------|
| Form backend (`/api/contact`) | Hosting decision | Need serverless function or email service |
| Painting project photos | Photography | Gallery has placeholder items, no real photos yet |
| Privacy policy page (`privacy.html`) | Legal content | Currently 404 |
| Terms & conditions page (`terms.html`) | Legal content | Currently 404 |
| Favicon + apple-touch-icon | Asset creation | No `<link rel="icon">` on any page |

### Medium Priority (blocks marketing)

| Item | Blocked By | Notes |
|------|-----------|-------|
| Google Tag Manager container | GTM account | Replace placeholder |
| Meta Pixel installation | Meta Business account | Replace placeholder in landing page |
| Google My Business setup | GMB account | Needed for local SEO |
| Google Search Console | DNS verification | Submit sitemap.xml |
| Google Maps embed on contact page | Maps API key | Currently placeholder |

### Low Priority

| Item | Notes |
|------|-------|
| CSS minification | styles.min.css needs re-minifying with orange variables |
| JS minification | form-validation.js is unminified |
| 404 page | No custom 404.html |
| Accessibility audit | Needs WAVE/axe testing |

---

## KNOWN ISSUES

| Issue | Severity | Details |
|-------|----------|---------|
| ABN is placeholder | Medium | `12 345 678 901` is a dummy — needs real ABN |
| Aggregate ratings in schema | Medium | 4.9 stars / 100 reviews hardcoded — need real data or remove |
| Suburb page content is adapted from tiling | Low | Some phrasing may sound slightly mechanical from sed replacements |
| Gallery has no real photos | Medium | Placeholder divs in gallery, no actual painting project images |
