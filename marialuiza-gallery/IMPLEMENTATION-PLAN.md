# Maria Luiza Gallery — Website Implementation Plan

## Overview
Repurpose the Arsenal of Art website layout (proven top-class design) for Maria Luiza Gallery.
Same tech stack: single-page HTML, GSAP animations, Lenis smooth scroll, Cinzel + Montserrat fonts.
Adapt content, branding, and color palette to match Maria Luiza's identity.

---

## Phase 1: Content Preparation & Branding

### 1.1 Color Palette Adaptation
- **Current Arsenal**: Dark theme with gold accent (#d4af37)
- **Proposed Maria Luiza**: Keep the dark/light dual theme system
  - Option A: Warm copper/burgundy accent — fits the bohemian bar-meets-gallery vibe
  - Option B: Deep wine red (#8B2252) or terracotta — references the historic atmosphere
  - Option C: Keep gold but shift warmer — aged brass tone
- **Decision needed**: Review their Instagram/Facebook for brand colors they already use

### 1.2 Logo & Visual Identity
- [ ] Request or download their logo from social media / Facebook page
- [ ] If no logo exists, create text-based logo using gallery name in Cinzel font
- [ ] Prepare logo in both dark and light variants

### 1.3 Photography & Media
- [ ] Collect high-quality images from their Instagram (@marialuiza.gallery)
- [ ] Collect images from their Facebook page
- [ ] Categories needed:
  - Gallery interior shots (the bar space, walls with paintings)
  - Exhibition opening events
  - Individual artworks
  - Artist portraits (Zhorj Sopadzhiev, Nikola Pevicharov, etc.)
  - The iconic black-and-white tile floor
  - Jazz/event nights
  - Food/bar atmosphere
  - Exterior / street view
- [ ] Convert all images to .webp format for performance
- [ ] Prepare hero image (gallery interior or dramatic artwork shot)

---

## Phase 2: Content Writing (BG + EN bilingual)

### 2.1 Hero Section
- Gallery name: "Галерия Мария Луиза"
- Tagline suggestions:
  - "Изкуство • Бохемия • Традиция" (Art • Bohemia • Tradition)
  - "Където изкуството среща духа на Пловдив" (Where art meets the spirit of Plovdiv)
  - "30 години арт бохемия в сърцето на Пловдив" (30 years of art bohemia in the heart of Plovdiv)

### 2.2 About Section
- History of the bar (1993, family of Boyan Sopadzhiev, royal naming permission)
- Gallery founding (2020) as natural extension
- Mission: presenting rising and established artists
- The bohemian atmosphere, multi-generational gathering place
- Location significance: foot of Old Town, between ancient temples

### 2.3 Exhibitions Section
- Current / upcoming exhibition (dynamic, updateable)
- Past exhibitions archive (scrollable gallery cards):
  - Stoyanova & Pevicharov "Настроени" (2026)
  - Zhorj Sopadzhiev "Фрагменти от виденията" (2026)
  - Lyuben Hranov memorial (2026)
  - Veneta Marinova "Точно време" (2025)
  - AMTII Photography (2025)
  - "Включване" 20 artists (2024)
  - Opening exhibition 12 artists (2020)

### 2.4 Artists Section
- Featured/resident artists with bios:
  - Zhorj Sopadzhiev (grandson of Paskal Struzhev, mosaics, paintings)
  - Nikola Pevicharov (doyen of Plovdiv art)
  - Other recurring exhibitors
- Art forms supported (painting, sculpture, graphics, photography, digital art, etc.)

### 2.5 Events Section
- Weekly jazz nights
- Exhibition openings
- NOŠ Plovdiv festival concerts
- Cultural gatherings

### 2.6 The Bar Section (unique differentiator)
- Food & drinks (Panti's artisanal menu)
- Bar atmosphere
- The iconic interior: black-and-white tiles, art on walls, bohemian vibe

### 2.7 Contact Section
- Address: бул. "Мария Луиза" 15, Пловдив 4000
- Phone: +359 89 035 6394
- Email: marialuiza.plovdiv@yahoo.com
- Social links: Instagram, Facebook
- Google Maps embed
- Working hours (to be confirmed with gallery)

---

## Phase 3: Technical Implementation

### 3.1 File Structure
```
marialuiza-gallery/
├── index.html          (main single-page site)
├── images/
│   ├── logo.png
│   ├── logo-light.png
│   ├── hero.webp
│   ├── about.webp
│   ├── gallery-*.webp  (exhibition photos)
│   ├── artist-*.webp   (artist portraits)
│   ├── bar-*.webp      (bar/food atmosphere)
│   └── event-*.webp    (events)
├── RESEARCH.md         (this file - reference)
├── IMPLEMENTATION-PLAN.md
└── sitemap.xml
```

### 3.2 Sections to Build (mapping from Arsenal layout)
| Arsenal Section | Maria Luiza Equivalent |
|----------------|----------------------|
| Hero + Canvas animation | Hero with gallery name + atmospheric animation |
| About the gallery | History & About (bar + gallery story) |
| Featured exhibition | Current/Next Exhibition highlight |
| Artist bio (Angel Geshev) | Featured Artists (multiple) |
| Events gallery grid | Exhibitions Archive + Events |
| Contact/Footer | Contact with map + social links |

### 3.3 Key Layout Features to Preserve
- [x] GSAP scroll-triggered animations
- [x] Lenis smooth scrolling
- [x] Dark/Light theme toggle
- [x] Canvas particle animation in hero
- [x] Parallax image effects
- [x] Elegant typography (Cinzel headings + Montserrat body)
- [x] Horizontal scroll gallery for exhibitions
- [x] Responsive mobile design
- [x] Animated navigation overlay

### 3.4 New/Modified Features
- [ ] **Exhibition cards** with dates, artists, and thumbnail — clickable to expand
- [ ] **Multiple artist profiles** instead of single artist (Arsenal had only Angel Geshev)
- [ ] **Bar/Food section** — unique to Maria Luiza, with menu highlights
- [ ] **Instagram feed integration** (optional, via embed or API)
- [ ] **Bilingual toggle** (BG/EN) — many tourists visit
- [ ] **Google Maps embed** in contact section

### 3.5 SEO & Meta
- Title: "Галерия Мария Луиза | Art Gallery & Bar Plovdiv"
- Description: Gallery + bar heritage, exhibitions, artists
- Open Graph tags for social sharing
- Schema.org markup: ArtGallery + BarOrPub
- Sitemap.xml

---

## Phase 4: Deployment

### 4.1 Domain Options (to discuss with client)
- marialuizagallery.com
- marialuiza-gallery.com
- galeria-marialuiza.com
- galeriamarialuiza.bg

### 4.2 Hosting
- Netlify (free tier, fast CDN) — same as Arsenal approach
- Or Vercel

---

## Phase 5: Content from Client (NEEDED)

### Must-Have from Gallery Owner
1. **Logo** (if they have one) or approval for text-based logo
2. **High-resolution photos** of gallery interior, exhibitions, artworks
3. **Working hours** and any seasonal schedule
4. **Preferred color scheme** or brand guidelines
5. **Current exhibition details** and upcoming schedule
6. **Artist bios** they want featured
7. **Menu/food offerings** if they want the bar section
8. **Any specific text** they want on the website
9. **Domain preference**

### Can Be Done Without Client Input
1. Layout and design (based on Arsenal template)
2. Animation and interaction design
3. Historical content (from research — bar history, gallery founding)
4. Exhibition archive (from press articles)
5. SEO setup
6. Responsive design
7. Performance optimization

---

## Timeline Estimate

| Phase | Duration | Notes |
|-------|----------|-------|
| Phase 1: Branding & Content Prep | 1-2 days | Depends on media availability |
| Phase 2: Content Writing | 1 day | BG text, EN can come later |
| Phase 3: Technical Build | 2-3 days | Main development |
| Phase 4: Polish & Deploy | 1 day | Testing, SEO, deploy |
| **Total** | **5-7 days** | Can start immediately with research content |

---

## Immediate Next Steps

1. **Download images** from Instagram and Facebook for placeholder/final use
2. **Clone Arsenal layout** into marialuiza-gallery/index.html
3. **Adapt color palette** — propose 2-3 options
4. **Replace all Arsenal-specific content** with Maria Luiza content
5. **Add new sections** (bar, multiple artists, exhibition archive)
6. **Preview and iterate**
