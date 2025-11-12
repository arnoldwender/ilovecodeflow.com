# ilovecodeflow.com

## 🎯 Project Context

**ilovecodeflow.com**
Do you love [Codeflow](https://developer.stackblitz.com/codeflow/what-is-codeflow)? We do!


## 💼 Business Context

### Client Project
This is a professional client website built by Wender Media.

**Wender Media Standards:**
- ✅ BFSG-compliant (Deadline: June 28, 2025)
- ✅ Lighthouse Score Target: 95+
- ✅ WCAG 2.2 AA Accessibility
- ✅ Mobile-First Design
- ✅ SEO-Optimized (100% Organic Strategy)
- ✅ DSGVO/GDPR Compliant

### Quality Standards
- **Performance**: Core Web Vitals optimized
- **Accessibility**: Full keyboard navigation, screen reader support
- **SEO**: Technical SEO, schema markup, semantic HTML
- **Security**: No external trackers, privacy-first
- **Responsiveness**: All breakpoints tested (mobile, tablet, desktop)

## 💻 Technology Stack

**Primary Technologies:** Astro
**Version**: 0.0.1

### Framework & Tools
- **Astro**: Static site generation for optimal performance

### Testing & Quality
- **Build Validation**: Zero errors policy

## 📁 Project Structure

This project uses a **standard structure** with source files in `src/`.

```
ilovecodeflow.com/
├── src/
│   ├── pages/             # Route pages
│   ├── components/        # Reusable components
│   ├── layouts/           # Layout templates
│   └── styles/            # Stylesheets
├── public/                # Static assets
├── tests/                 # Test files
├── .github/               # CI/CD workflows
└── package.json
```


**Main directories:**
- `src/`
- `public/`

## 🚀 Development Workflow

### Initial Setup
```bash
# Clone repository
git clone <repository-url>
cd ilovecodeflow.com

# Install dependencies
npm install
```

### Development Server
```bash
# Start dev server
npm run dev
```

### Build & Preview
```bash
# Build for production
npm run build

# Preview production build
npm run preview
```

### Testing
_No testing framework detected in package.json_

### Before Every Commit
```bash
# MANDATORY checks
npm run build          # MUST succeed with 0 errors

# Verify no broken links
# Check accessibility (keyboard navigation, screen readers)
# Test mobile responsiveness
```

## 🎨 Key Features & Components

- [**Codeflow IDE**](https://developer.stackblitz.com/codeflow/working-in-codeflow-ide) is a fully fledged desktop-grade dev environment capable of running your whole workflow - from production-level dev work to reviewing pull requests.
- [**Web Publisher**](https://developer.stackblitz.com/codeflow/content-updates-with-web-publisher) is a publishing tool that makes editing docs or blogs pleasant thanks to a realtime preview of the changes.
- [**pr.new**](https://developer.stackblitz.com/codeflow/using-pr-new) is a short URL that can be used on any repository to explore code, a branch or an issue, to review a PR, or even to edit a file, all in a live environment with a realtime preview.
- [**CodeflowApp**](https://developer.stackblitz.com/codeflow/integrating-codeflowapp-bot) is a friendly bot, which provides a one-click link that spins up the whole environment for pull requests and issues. No more context-switching or branch-checkouts, just a new browser tab with a full IDE and a dev server running.
- 📝 Take Web Publisher for a spin by adding your name to [ilovecodeflow.com](https://ilovecodeflow.com/)!
- 💻 Explore how we built [our docs site](https://pr.new/github.com/stackblitz/docs) in Codeflow IDE!
- 🕵️ Review [this suspicious PR](https://pr.new/stackblitz/docs/pull/40) in Codeflow IDE
- 🤖 See our CodeflowApp bot in action on [a PR](https://github.com/stackblitz/docs/pull/40#issue-1404169268)!

## 📝 Development Guidelines

### Code Style & Standards
- **JavaScript/TypeScript**: Modern ES6+ syntax
- **Components**: Modular, reusable, single-responsibility
- **Styling**: Semantic CSS, BEM methodology
- **Accessibility**: ARIA labels, semantic HTML, keyboard navigation
- **Performance**: Lazy loading, code splitting, optimized assets

### File Naming Conventions
- **Components**: PascalCase (e.g., `HeroSection.astro`, `ContactForm.tsx`)
- **Pages**: kebab-case (e.g., `about-us.astro`, `contact.astro`)
- **Utilities**: camelCase (e.g., `formatDate.ts`, `validateEmail.ts`)
- **Styles**: kebab-case (e.g., `global.css`, `hero-section.css`)

### Adding New Features
1. **Create feature branch**: `git checkout -b feature/feature-name`
2. **Implement changes** following existing patterns
3. **Add/update tests** if applicable
4. **Run build** and verify 0 errors
5. **Test across browsers** (Chrome, Firefox, Safari)
6. **Check accessibility** (keyboard nav, screen readers)
7. **Create PR** with clear description

### Accessibility Checklist
- [ ] All images have descriptive alt text
- [ ] Color contrast ratio ≥ 4.5:1
- [ ] Full keyboard navigation support
- [ ] ARIA labels for interactive elements
- [ ] Focus indicators visible
- [ ] Screen reader compatible
- [ ] `prefers-reduced-motion` support
- [ ] Semantic HTML structure (proper heading hierarchy)

### SEO Guidelines (CRITICAL for Client Projects)

**Arnold's SEO Philosophy:**
> "100% organic SEO - No paid ads, ever!"

#### On-Page SEO Requirements
1. **Meta Tags**
   - Unique meta description per page (max 160 chars)
   - Title tag with primary keyword (max 60 chars)
   - Open Graph tags for social sharing

2. **Content Structure**
   - Exactly ONE H1 per page
   - Logical heading hierarchy (H1 → H2 → H3)
   - Keyword-rich but natural content
   - Internal linking to related pages

3. **Technical SEO**
   - Clean URLs (kebab-case, descriptive)
   - XML sitemap (auto-generated)
   - Robots.txt configured
   - Schema.org markup
   - Canonical URLs set
   - Mobile-friendly design

4. **Performance SEO**
   - Lighthouse Performance Score: 95+
   - Core Web Vitals optimized (LCP, FID, CLS)
   - Fast page load times (<2s)
   - Optimized images (WebP + fallback)

#### ❌ NEVER Do (SEO)
- ❌ Suggest Google Ads or paid advertising
- ❌ Keyword stuffing
- ❌ Duplicate content
- ❌ Broken internal links
- ❌ Missing alt text on images
- ❌ Slow page loads (>3s)

## 🔧 Git Workflow & Commits

### Branch Strategy
- **main/master**: Production-ready code
- **feature/***: New features
- **fix/***: Bug fixes
- **docs/***: Documentation updates

### Commit Message Format
```
<type>(<scope>): <subject>

<body>

<footer>
```

**Types:**
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation
- `style`: CSS/formatting
- `refactor`: Code refactoring
- `test`: Testing
- `perf`: Performance improvement
- `a11y`: Accessibility
- `seo`: SEO optimization

**Example:**
```bash
git commit -m "feat(contact): add contact form with validation

- Implement form with email and message fields
- Add client-side validation
- Include ARIA labels for accessibility
- Test keyboard navigation

Tested on Chrome, Firefox, Safari
Lighthouse Score: 98"
```

## 🚨 Common Issues & Solutions

### Build Errors
- **Issue**: Build fails with TypeScript errors
  - **Solution**: Run `npm run build` and fix type errors

- **Issue**: Missing dependencies
  - **Solution**: `npm install`

### Development Server
- **Issue**: Port already in use
  - **Solution**: Kill process on port or use different port

### Performance
- **Issue**: Low Lighthouse score
  - **Solution**: Optimize images, minimize JavaScript, lazy load assets

## 📊 Quality Metrics & Goals

### Target Scores
- **Lighthouse Performance**: 95+
- **Lighthouse Accessibility**: 100
- **Lighthouse Best Practices**: 95+
- **Lighthouse SEO**: 95+

### Build Requirements
- ✅ Zero TypeScript errors
- ✅ Zero build warnings
- ✅ All tests passing
- ✅ No broken links
- ✅ WCAG 2.2 AA compliant

## 🔗 Resources & Documentation

- **README**: See [README.md](../README.md) for detailed documentation
- **Wender Media**: https://www.wendermedia.com
- **BFSG Info**: https://www.bfsg.de

## 💡 Tips & Best Practices

1. **Always test mobile-first** - Most users visit from mobile devices
2. **Accessibility is not optional** - BFSG compliance required by June 28, 2025
3. **Performance matters** - Every 100ms delay costs conversions
4. **SEO is ongoing** - Keep content fresh, fix broken links immediately
5. **Test across browsers** - Chrome, Firefox, Safari minimum
6. **Use semantic HTML** - Better for SEO and accessibility
7. **Optimize images** - WebP format with fallbacks
8. **Keep dependencies updated** - Security and performance

## ❌ Never Do

1. ❌ Commit without successful build (`npm run build`)
2. ❌ Skip accessibility testing
3. ❌ Ignore broken links
4. ❌ Add tracking cookies without consent
5. ❌ Use inline styles (except critical CSS)
6. ❌ Hardcode URLs (use config/env vars)
7. ❌ Skip alt text on images
8. ❌ Make breaking changes without discussion
9. ❌ Suggest paid advertising (Arnold is 100% organic SEO)
10. ❌ Deploy without client approval

---

**Project**: ilovecodeflow.com
**Version**: 0.0.1
**Last Updated**: 2025-11-12
**Maintained by**: Wender Media + Claude Code

*This comprehensive guide ensures quality, accessibility, and SEO excellence.*
