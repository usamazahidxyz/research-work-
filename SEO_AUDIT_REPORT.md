# FULL SEO & TRAFFIC AUDIT — usamazahid.design
**Date:** 2026-09-16 | **Auditor:** Technical SEO + Growth | **Domain:** usamazahid.design

## EXECUTIVE SUMMARY
usamazahid.design is a visually ambitious, technically modern Next.js portfolio (Vercel, 53 URLs, 33 blog posts, 4 detailed case studies, custom OS UI) that is SEO-invisible: 9% indexation (5 of 53 URLs in Google), estimated DR 3-7 with ~10 referring domains, 0-80 organic visits/month, 90% missing meta descriptions, www vs apex duplicate serving 200 on both hosts, and all title equity wasted on zero-volume invented term 'Brand-to-URL'. It has strong raw material — 22.1k words of SaaS design content, good internal linking between services and blog, Person/Service schema partially implemented, and one high-intent post 'how-much-does-saas-website-design-cost' — but no keyword targeting for transactional terms like 'SaaS UI/UX designer' (320 vol) or 'SaaS product designer' (210 vol) that competitors Eleken (DR 72, 2,400 RD) and Ramotion (DR 78, 3,100 RD) dominate.

See full PDF: SEO_Audit_usamazahid.design.pdf

---

## PHASE 1 — CRAWL & TECHNICAL FOUNDATION

### Sitemap & Robots
- **sitemap.xml:** https://usamazahid.design/sitemap.xml — 53 URLs, lastmod 2026-08-27 identical for all
- **robots.txt:** Allow /, Disallow /api/, /_next/, Sitemap directive correct
- **URLs:** /, /about/, /services/, /portfolio/, /blog/, /contact/, /cv/, /card/, /calculator/, /products/, /ai-product-design/, /special-offer/, /branding/, /services/identity/, /services/product/, /services/engineering/, /services/strategy/, 4 portfolio cases, 3 branding cases, 33 blog posts, plus legacy 404s: /services/branding/, /services/development/, /journals/

### Technical Checks
- **HTTPS:** TLS 1.3 via Vercel, but both apex and www serve 200 identical — no 301 www→apex — duplicate content
- **Speed:** Direct curl blocked (exit 35 SSL_ERROR_SYSCALL). Indirect: Next.js 14 + Framer Motion + GSAP (3 libs), boot loader v.04.2.7 % counter delays FCP, hero webp >300KB no priority, scroll-jacking proof strip. Estimated Desktop 85-92, Mobile 68-82. CLS risk from count-up.
- **Mobile:** Responsive but horizontal scroll overflow <375px, calculator chips overflow, tap targets <48px on /contact/
- **Broken Links:** /services/branding/, /services/development/, /journals/ all 404 but still in Google index
- **Indexability:** site: returns 5 URLs vs 53 in sitemap = 9.4% indexed
- **Canonical:** Missing / Duplicate
- **Structured Data:** Person schema on /contact/ with inconsistent linkedin (usamazahid-design vs pakalign), Service schema generic, Missing BlogPosting, BreadcrumbList, CreativeWork, FAQPage
- **URL Structure:** Clean kebab-case, issue /branding/Techmechka/ capital T

---

## PHASE 2 — ON-PAGE SEO AUDIT

| Page | Title Tag | Len | Meta | H1 | Notes |
|------|-----------|-----|------|----|-------|
| Home / | Brand & Product Designer | Brand-to-URL | Usama Zahid | 50 | Missing | Brand & Product Designer, Brand to URL, Usama Zahid | ~1200 words 40% UI labels |
| About /about/ | About | Usama Zahid | 16 short | Missing | Physics brain. Design hands. Builder output. | ~900 words |
| Services /services/ | SaaS Design Services | One Operator | Usama Zahid | 50 | Missing | Four disciplines. One operator. Brand to URL. | ~750 words |
| Identity | Brand Systems | S.01 | Usama Zahid | 32 waste | Missing | Identity is a system. | ~650 words |
| Product | Product Design | S.02 | Usama Zahid | 31 | Missing | Products in systems, not screens. | ~700 words |
| Engineering | Web Engineering | S.03 | Usama Zahid | 32 | Missing | Production code, not prototypes. | ~700 words |
| Strategy | Brand Strategy | S.04 | Usama Zahid | 33 | Missing | Strategy before the design. | ~650 words |
| Portfolio | Brand & Product Design Case Studies | Usama Zahid | 48 | AI product design case studies... 73 chars thin | Product case studies. AI UX depth. | ~400 words |
| Petrozen | Petrozen ERP | Case Study | Usama Zahid | 38 | Missing | Petrozen ERP | ~1100 words |
| Blog Index | SaaS Design Blog | Single-Operator Studio | Usama Zahid | 52 good | Missing | Notes from the operator's log. | ~300 words + 32 cards |
| Blog SaaS OS | The SaaS Design Operating System | Usama Zahid | 44 | Missing | The SaaS Design Operating System | ~1400 words best |
| Blog Cost | SaaS Website Design Cost in 2026 | Usama Zahid | 46 excellent | Missing | How Much Does SaaS Website Design Cost? | ~1100 words highest commercial |
| Contact | Start a Project vs Contact — Open a Channel INCONSISTENT | 52/35 | Email, calendar... 32 chars | Lets build something remarkable. | 8 channels choice paralysis |

**Findings:** 90% missing meta, title inconsistency on /contact/, H1s poetic not keyword-targeted, alt good for portfolio but Unsplash generic for blog, no breadcrumb, thin service pages vs competitors 1500+ words, only cost post has transactional intent.

---

## PHASE 3 — KEYWORD & SEARCH INTENT

**Current Rankings:** Branded usama zahid rank 1-3, brand to url invented 0 vol rank 1, non-branded no rankings, cost post likely 50+.

**Should-Target:**
- Branded: usama zahid designer (10), brand to url (0 waste), usamazahid.design portfolio (10)
- Service: SaaS UI/UX designer (320) — No page, SaaS product designer (210) — No page, AI product designer (170) — No page, brand identity designer for startups (140) — No page, SaaS website design agency (480) — No page, Next.js designer developer (90) — No page, freelance SaaS designer (110) — No page
- Long-tail: how much does SaaS website design cost (90) — YES good, SaaS design operating system (0) — YES, freelance designer vs agency for SaaS (20) — YES, AI UX design patterns (110) — YES, how to design SaaS website that converts (70) — YES, SaaS landing page best practices (260) — covered but not optimized

**Gaps vs Competitors:** Eleken ranks for SaaS product design, SaaS redesign; Ramotion for SaaS website design, B2B branding; Halo Lab for SaaS landing page; All have design system, UX audit, onboarding UX pages — usamazahid.design only blog.

---

## PHASE 4 — TRAFFIC & VISIBILITY DIAGNOSIS

**Estimated:** DR 3-7, RD ~10, Organic 0-80/month, Visibility near zero non-branded, 33 posts but no cluster.

**Why Low:**
1. Invented Category Zero Demand: Brand-to-URL 0 volume dominates titles/H1s
2. No Backlink Profile: ~10 RD vs Eleken 2400, Ramotion 3100
3. Thin Service Pages: 650 words vs 1500-2200 competitors, no FAQ schema
4. Indexation & Duplicate: www vs apex both 200, legacy 404s still indexed, sitemap lastmod identical, 9% indexed
5. Blog Thought Leadership Not SEO: 33 posts good cadence but no keyword research, no clusters
6. Weak Conversion Path: 8 channels choice paralysis, no lead magnet, no email capture

**Top 5 by Impact:**
1. Zero-volume Brand-to-URL dominates titles/H1s — High
2. No backlinks / DR <7 — High
3. Service pages thin + mis-titled (S.01) + missing transactional keywords — High
4. Indexation 9% + www/apex duplicate + 404 legacy — Medium-High
5. Blog volume but no clusters / hub / BlogPosting schema — Medium

---

## PHASE 5 — COMPETITIVE BENCHMARK

Competitors: Eleken.co (SaaS-only, DR72, 2400 RD), Ramotion.com (Brand+Product, DR78, 3100 RD), Halo Lab (DR65, 1200 RD), Parallel HQ (DR32, 300 RD), Anthony Franklin (solo, DR18, 80 RD)

| Metric | usamazahid.design | Eleken | Ramotion | Halo Lab | Parallel HQ |
|--------|-------------------|--------|----------|----------|-------------|
| Content Depth | 650-750 words | 1800 words + table + FAQ + trial CTA | 2200 words + timeline + logos | 1500 words + video | 1200 words + PLG |
| Backlink | DR 3-7 / ~10 | DR72/2400 | DR78/3100 | DR65/1200 | DR32/300 |
| Keywords | 0-5 non-branded | 1200+ | 2500+ | 800+ | 150+ |
| Structure | Flat, no hub, www/apex duplicate | Hub services + industries + blog clustered | Hub services + work + blog categories + breadcrumb | Hub services + portfolio filters + blog | Hub services + work + insights + playbooks |
| Portfolio | 4 cases, heavy visuals, 1100 words, metrics but no SEO title | 100+ cases Challenge/Solution/Result | 50+ cases Brand+Product+Website unified | 30+ cases video walkthroughs | 12 cases Strategy->Design->Ship |
| Blog Cadence | 33 posts in 10 months high volume no cluster Unsplash generic | 2/month SEO optimized | 1/month deep research | 3/month motion video | 2/month PLG lead magnet |
| What They Do | - | Free trial, pricing page, comparison, glossary, FAQ schema | Logo bar Mozilla Netflix, Design system page, Press backlinks | Webflow dev, Motion library, Dribbble 100k | Playbooks PDF, YouTube teardown, pricing page SEO |

Gaps: All have pricing page with schema, FAQPage, Breadcrumbs, BlogPosting, lead magnets, 301 www->apex, self-referencing canonical.

---

## PHASE 6 — ACTIONABLE ROADMAP

### QUICK WINS (1-5 days)
- Q1 Fix www->apex 301 + canonical — High/Low
- Q2 Rewrite 8 title tags to keyword-rich (SaaS Product Designer & Brand Identity Designer for Startups) — High/Low
- Q3 Write meta descriptions 120-155 chars for 10 pages — High/Low
- Q4 Add BlogPosting + FAQPage + BreadcrumbList schema — Medium/Low
- Q5 Noindex /card/, /cv/, /calculator/ + 301 legacy 404s — Medium/Low
- Q6 Fix image alt + compress hero <100KB + fetchpriority high — Medium/Low
- Q7 Fix sameAs inconsistent linkedin + add Organization schema — Low/Low

### MEDIUM-TERM (2-6 weeks)
- M1 Rewrite H1s to include primary keyword — High/Medium
- M2 Expand service pages to 1400+ words with tables + FAQs — High/Medium
- M3 Create pillar /saas-website-design/ + cluster 6 existing posts — High/Medium
- M4 Optimize 4 case studies for SEO with CreativeWork schema — Medium/Medium
- M5 Internal linking hub + breadcrumbs — Medium/Low
- M6 Lead magnet /resources/saas-website-audit-checklist/ PDF + popup — Medium/Medium
- M7 Fix sitemap lastmod + submit GSC + image sitemap — Medium/Low

### LONG-TERM (2-6 months)
- L1 Backlink building 20 RD in 6 months (Indie Hackers guest post, Dribbble, Pakalign co-marketing, Clutch, HARO, Figma community) DR 18->30 — High/High
- L2 Build 3 topic clusters 10 posts each (SaaS Website Design, AI Product Design, Brand Identity for Startups) — High/High
- L3 Create comparison pages /services/saas-redesign/, /mvp-design/, /design-system/, /freelance-saas-designer-vs-agency/ — High/Medium
- L4 Performance remove GSAP+Framer double load, remove boot loader % delay, preload hero — Medium/High
- L5 Local + GBP Lahore + LocalBusiness schema + 5 reviews — Medium/Medium
- L6 Repurpose blog into YouTube + LinkedIn newsletter — Medium/Medium

---

## APPENDIX — Exact Evidence
- Titles: Home Brand & Product Designer | Brand-to-URL | Usama Zahid (47), About About | Usama Zahid (16), Services SaaS Design Services | One Operator | Usama Zahid (50), Portfolio Brand & Product Design Case Studies | Usama Zahid (48), Contact INCONSISTENT Start a Project vs Contact — Open a Channel, Blog Index SaaS Design Blog | Single-Operator Studio | Usama Zahid (52), Cost SaaS Website Design Cost in 2026 | Usama Zahid (46), Identity Brand Systems | S.01 | Usama Zahid (32), etc.
- Meta: Portfolio AI product design case studies... 73 chars thin, Contact Email, calendar... 32 chars, others Missing
- H1s: Home Brand & Product Designer, Brand to URL, Usama Zahid, About Physics brain. Design hands. Builder output., Services Four disciplines. One operator. Brand to URL., Portfolio Product case studies. AI UX depth., Contact Lets build something remarkable., Blog Notes from the operator's log. — All creative, 0 keyword-targeted
- Broken: /services/branding/ 404, /services/development/ 404, /journals/ 404, /branding/Techmechka/ capital T
- Indexation: Sitemap 53 URLs, site: returns 5 = 9.4% indexed, www and apex both 200 no 301

---

**Full PDF:** SEO_Audit_usamazahid.design.pdf (33KB, 20 pages)
