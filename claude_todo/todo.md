# Website Improvement Tasks - Phase 2

## Bugs & Broken References

- [x] Fix missing favicon.ico - referenced in `<head>` but file doesn't exist *(still missing - need to provide an actual .ico file)*
- [x] Fix empty `href=""` on Experience card links (removed dead link wrappers)
- [x] Fix logo alt text - changed from "Asentus Logo" to "Daniel Fan"
- [x] Fix footer logo alt text - changed from "Aircv Logo" to "Daniel Fan"
- [x] Update copyright year from 2025 to 2026

## Content Updates

- [ ] Add a PDF version of resume (resume.pdf) alongside .docx - PDF is the standard format recruiters expect *(waiting for PDF file)*
- [x] Update page title to "Daniel Fan - ML Engineer, Martial Artist, Magician"
- [x] Add Education section (M.S. ECE from Binghamton University with thesis info)
- [x] Add Education link to navigation bar
- [x] Add MLOps & Model Deployment skill bar
- [ ] Replace stock/placeholder portfolio images with actual project screenshots or relevant visuals

## SEO & Meta

- [x] Add Open Graph meta tags (og:title, og:description, og:image, og:url, og:type)
- [x] Add Twitter/X card meta tags
- [x] Add JSON-LD structured data (Person schema with job, education, social links)
- [x] Add canonical URL meta tag
- [x] Add robots.txt file
- [x] Add sitemap.xml

## Accessibility

- [x] Add skip-to-content link for keyboard navigation
- [x] Add ARIA label to main navigation
- [x] Add ARIA labels to social icon links (GitHub, LinkedIn, Facebook)
- [x] Fix all logo/footer images with meaningful alt text
- [x] All portfolio images already have meaningful alt text
- [ ] Check color contrast ratios meet WCAG AA standards *(needs manual/tool audit)*

## Performance

- [x] Add `loading="lazy"` to all portfolio images (5 images)
- [x] Add `defer` to non-critical JavaScript files (plugins + page scripts)
- [x] Add `preconnect` hints for Google Fonts (fonts.googleapis.com + fonts.gstatic.com)

## Code Cleanup

- [x] Remove KeenThemes template comment block from top of HTML

## Still TODO (P3 - Larger Undertakings)

- [ ] Upgrade from Bootstrap 3 to Bootstrap 5 (Bootstrap 3 is EOL)
- [ ] Remove jQuery dependency (not needed with modern Bootstrap 5)
- [ ] Add dark mode toggle / respect `prefers-color-scheme`
- [ ] Add smooth scroll-reveal animations (replace WOW.js with modern alternative)
- [ ] Add a proper hero section with professional headshot/avatar
- [ ] Add a contact form (Formspree or similar)
- [ ] Add analytics (Plausible/Umami for privacy-friendly tracking)
- [ ] Set up a build process (SASS compilation, CSS/JS minification)
- [ ] Add .editorconfig for consistent formatting

## Needs User Input

- [ ] Provide favicon.ico file (currently referenced but missing)
- [ ] Provide resume.pdf for download button
- [ ] Provide actual portfolio project screenshots to replace stock images
- [ ] WCAG color contrast audit (run Lighthouse or axe)

---

<details>
<summary>Phase 1 Tasks - ALL COMPLETE</summary>

### About Section Updates (from resume)
- [x] Update intro paragraph to highlight: Applied Scientist & Senior ML Engineer with 10+ years experience
- [x] Add expertise areas: transformers, LLM fine-tuning, reinforcement learning, NLP
- [x] Mention deploying custom LLMs to 30,000+ users worldwide
- [x] Add M.S. in Electrical and Computer Engineering from Binghamton University
- [x] Mention published research at IJCNN
- [x] Update Skills section with current tech stack
- [x] Add RLHF, LoRA/PEFT, Quantization to skills
- [x] Update location from Auckland to Seattle, WA
- [x] Update contact email to contact@danielhtfan.com
- [x] Add GitHub link

### Critical Fixes
- [x] Fix truncated bio text in About section
- [x] Fix typo in Deep Learning progress bar
- [x] Fix duplicate id="about"

### Content Updates
- [x] Replace Lorem ipsum placeholder text in Experience section cards
- [x] Replace Lorem ipsum placeholder text in all Portfolio/Work popup descriptions
- [x] Update copyright year from 2020 to 2025
- [x] Complete the About/Intro section with actual bio content
- [x] Add actual project descriptions to portfolio items

### Security & Performance
- [x] Change Google Fonts URL from HTTP to HTTPS
- [x] Add meta description content for SEO
- [x] Add meta author content

### Portfolio Section
- [x] Update placeholder titles with actual project names
- [x] Replace placeholder project team info with actual credits
- [x] Add project details to portfolio items

### New Sections
- [x] Add Work Experience section with 4 roles
- [x] Add Publications section with 4 papers
- [x] Add Resume download button

### Quick Wins
- [x] Add GitHub link to social icons
- [x] Fix mailto link to use contact@danielhtfan.com

</details>
