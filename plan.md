# Academic Website Redesign Plan for carologic.com

## Current Website Content Inventory

The existing site (built with Webflow) has 4 pages plus a homepage:

1. **Homepage** — Bio, tagline, achievements (100 Brilliant Women in AI Ethics, ACM Distinguished Speaker)
2. **Speaking** — Introduction paragraph + 11 talks/keynotes/workshops with titles, venues, locations
3. **Writing** — 9 publications (papers, essays, book contributions) with full citation details
4. **Resources** — Curated AI ethics/UX resources organized into 7 categories (activities, tools, resource lists, organizations, books, Carol's own work)
5. **Contact** — Contact form + LinkedIn link

---

## Proposed Academic Website Structure

Academic personal websites typically follow a clean, content-first design with minimal decoration. The redesign will use **static HTML + CSS** (no framework, no build step) for maximum simplicity and portability.

### Tech Stack
- **Plain HTML5 + CSS3** — No JavaScript frameworks, no build tools, no dependencies
- **Single CSS file** — Clean, responsive stylesheet with a neutral academic palette
- **System font stack** — Using standard serif/sans-serif fonts common on academic sites (Georgia, system fonts) to avoid external dependencies
- **No JavaScript required** — Except optionally for the contact form

### Color Palette & Typography (Academic Style)
- Dark navy/charcoal text on white/light gray background
- Accent color: muted blue for links (common in academia)
- Body text: serif font (Georgia) for readability — a classic academic choice
- Headings: clean sans-serif (system font stack)
- Generous whitespace, single-column layout

### File Structure
```
website/
├── index.html          # Homepage: bio, photo placeholder, achievements
├── speaking.html       # Speaking engagements
├── publications.html   # Writing/publications (renamed to academic convention)
├── resources.html      # Curated resources
├── contact.html        # Contact information
├── css/
│   └── style.css       # Single stylesheet
├── LICENSE
└── README.md
```

### Page-by-Page Plan

#### 1. `index.html` — Home / About
- **Header**: Name "Carol J. Smith" as prominent heading, institutional affiliation (Carnegie Mellon University), role (Research Scientist; Adjunct Instructor, HCI Institute)
- **Tagline**: "Researching the complexities of human-AI interactions"
- **Navigation bar**: Home | Speaking | Publications | Resources | Contact
- **Bio section**: Full bio paragraph from the current site
- **Highlights/distinctions**: 100 Brilliant Women in AI Ethics (2023), ACM Distinguished Speaker (2021–2025)
- **Sidebar or footer links**: Google Scholar, LinkedIn, SlideShare

#### 2. `speaking.html` — Speaking
- **Intro paragraph**: Current speaking intro text (250+ talks, 45+ cities, ACM Distinguished Speaker, IEEE senior member, UXPA member)
- **Talks list**: All 11 talks presented in reverse-chronological academic style:
  - Talk title (bold)
  - Event/venue name
  - Location
  - Type (Keynote / Workshop / Panel / Presentation)
  - Link to video where available (YouTube links for MLUX and PyCon 2020)
- Google Scholar link for additional publications

#### 3. `publications.html` — Publications (renamed from "Writing")
- All 9 publications in **academic citation format**, grouped or listed chronologically (newest first):
  1. "Creating a Curious, Ethical AI Workforce" — War on the Rocks, 2020
  2. "Designing Trustworthy AI..." — arXiv:1910.03515, AAAI FSS-19, 2019
  3. "Intentionally Ethical AI Experiences" — JUS, Vol 14(4), 2019
  4. "AUX3: Making UX Research Track with Agile" — UX Magazine, 2019
  5. "A Turn of Phrase..." — UX Magazine, 2017
  6. "Getting the Most Out of Remote Research..." — ACM Interactions, 2017
  7. "The Lights Seemed Dimmer..." — Book chapter, 2013
  8. "Negotiation: You Already Do It..." — UX Magazine, 2013
  9. "Words Matter" — Book case study, 2012
- Each entry includes: authors, title, venue, date, DOI/URL where available
- Link to Google Scholar profile

#### 4. `resources.html` — Resources
- Introductory text preserved from current site
- Resources organized under the same 7 category headings:
  1. Curiosity Activating UX Activities (4 items)
  2. Tools for Supporting Ethical AI (4 items)
  3. Lists of Additional Resources (6 items)
  4. Organizations and Newsletters (7 items)
  5. Books (5 items)
  6. Carol Smith's Contributions (5 items)
- Each resource: title, author, brief description, link

#### 5. `contact.html` — Contact
- "Get in Touch" heading
- Contact form (First Name, Last Name, Email, Message) — form action can use Formspree or similar static-site-compatible service as a placeholder
- LinkedIn profile link
- Note: Without a backend, the form will be a styled HTML form with a placeholder action. A note will indicate how to connect it to a form service.

### Design Principles (Academic Website Conventions)
1. **Content-first**: No hero images, sliders, or decorative elements
2. **Clean typography**: Readable body text, clear heading hierarchy
3. **Simple navigation**: Persistent top nav bar across all pages
4. **Minimal color**: Mostly black text on white, one accent color for links
5. **Responsive**: Works on mobile but designed primarily for desktop reading
6. **Fast loading**: No external dependencies, no JavaScript frameworks
7. **Professional**: Similar in style to faculty pages at CMU, MIT, Stanford, etc.

### Content Mapping (Current → New)
| Current Site | New Site | Notes |
|---|---|---|
| Homepage bio | index.html | Restructured with academic layout |
| Speaking page | speaking.html | Same content, academic formatting |
| Writing page | publications.html | Renamed; academic citation format |
| Resources page | resources.html | Same structure and content |
| Contact Carol | contact.html | Same content |
| LinkedIn link | Footer on all pages | Consistent across site |
| Google Scholar | Footer/publications | Prominent academic link |
| SlideShare | Footer | Preserved |
| "100 Brilliant Women" badge | index.html | Listed as distinction |
| ACM Distinguished Speaker | index.html + speaking.html | Listed as distinction |
| © Carologic notice | Footer on all pages | Preserved |

### What Will NOT Change
- All text content preserved verbatim from current site
- All external links preserved
- All publication details preserved
- No new content added
