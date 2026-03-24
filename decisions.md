# North Shore Painting — Architectural Decisions Log

> Records every significant design and technical decision in the project.
> Inherits decisions D01-D21 from the original NORTH-SHORE-PROJECTS repo.
> Format: Decision, rationale, and any trade-offs.

---

## D22: Site Split — Painting-Only Repo from NORTH-SHORE-TILING

**Decision:** Create the NORTH-SHORE-PAINTING repo by forking from NORTH-SHORE-TILING (which was itself forked from NORTH-SHORE-PROJECTS), then adapting all content for painting services at `northshorepaints.com.au`.

**What changed:**
- Forked NORTH-SHORE-TILING into NORTH-SHORE-PAINTING with fresh git history
- Created new painting homepage (index.html) with painting-specific services, trust bar, FAQ, and gallery placeholders
- Accent colour changed from gold (#C19A6B) to warm orange (#E07B39) in CSS variables
- Domain: northshoretiles.com.au → northshorepaints.com.au across all files
- Branding: "North Shore Tiling" → "North Shore Painting"
- Email: northshoretiling8@gmail.com → northshorepainting@gmail.com
- Logo: NSTLOGO-HD-FINAL.png → NSPAINTLOGO-HD-FINAL.png
- Instagram: @northshoretiling → @northshorepainting
- 17 suburb pages renamed from tiling-* to painting-* with painting-specific content
- 2 painting blog posts created (replacing tiling articles)
- Landing page renamed from landing/tiling.html → landing/painting.html
- Redirect pages: tiling.html → northshoretiles.com.au, cleaning.html → northshorecleans.com.au, northshore-removals.html → northshoreremovals.com
- Nav structure: Painting → index.html (homepage), Tiling → tiling.html (redirect to sister site)
- Tiling images and videos deleted

**Rationale:**
- Forking from NORTH-SHORE-TILING (rather than NORTH-SHORE-PROJECTS) provides a clean, already-split codebase with redirect pages and tiling-only structure that's easy to adapt
- Orange accent colour differentiates the painting brand visually from the tiling site's gold
- Same architectural patterns (suburb pages, blog, landing pages, redirect pages) ensure consistency across the family of sites

**Trade-offs:**
- Suburb page content was adapted via sed replacements — some phrasing may need manual editorial polish
- Gallery has placeholder items until real painting photos are added
- Blog posts are newly created rather than adapted from existing painting articles in the original NSP repo
