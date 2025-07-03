# Bug Report - Personal Website

## Executive Summary
Found **11 bugs** across multiple categories including HTML validation errors, security vulnerabilities, accessibility issues, and configuration problems.

## Critical Issues (High Priority)

### 1. **Duplicate ID Attribute** 🔴
- **Location**: `index.html` lines 102 and 129
- **Issue**: Two `<div>` elements both have `id="about"`
- **Impact**: Breaks HTML validation, causes JavaScript errors, fails WCAG accessibility standards
- **Fix**: Change one ID to `id="skills"` to match its content

### 2. **Insecure HTTP Resources** 🔴
- **Location**: `index.html` line 23
- **Issue**: Google Fonts loaded over HTTP instead of HTTPS
- **Impact**: Mixed content warnings, blocked resources on HTTPS sites, security vulnerability
- **Fix**: Change `http://fonts.googleapis.com/css?family=Hind:300,400,500,600,700` to `https://`

### 3. **Malformed Email Link** 🔴
- **Location**: `index.html` line 489
- **Issue**: `<a href="mailto:#">` instead of proper email format
- **Impact**: Email client won't open correctly
- **Fix**: Change to `<a href="mailto:daniel.fan@appletreeacademics.com">`

## Security Issues (Medium Priority)

### 4. **External Links Without Security Attributes** 🟡
- **Location**: Multiple external links throughout `index.html`
- **Issue**: Links to external sites missing `rel="noopener noreferrer"`
- **Impact**: Potential security vulnerability (window.opener access)
- **Fix**: Add security attributes to external links

### 5. **Mixed Content Links** 🟡
- **Location**: `index.html` multiple lines (279-436, 485)
- **Issue**: Multiple HTTP links to keenthemes.com and other external sites
- **Impact**: Mixed content warnings on HTTPS deployment
- **Fix**: Update all HTTP links to HTTPS where available

## Accessibility Issues (Medium Priority)

### 6. **Empty href Attributes** 🟡
- **Location**: `index.html` lines 210, 222, 234
- **Issue**: `<a href="">` creates non-functional links
- **Impact**: Poor user experience, accessibility violations
- **Fix**: Either remove links or provide proper destinations

### 7. **Invalid Alt Text** 🟡
- **Location**: `index.html` lines 55-56
- **Issue**: Alt text says "Asentus Logo" but should reflect actual content
- **Impact**: Screen readers get incorrect information
- **Fix**: Update to "Daniel Fan Logo" or similar

## Code Quality Issues (Low Priority)

### 8. **Missing Package Dependencies** 🟡
- **Location**: `package.json`
- **Issue**: No dependencies listed despite using jQuery, Bootstrap, etc.
- **Impact**: Difficult to manage and update dependencies
- **Fix**: Add proper dependency management

### 9. **No Main Entry Point** 🟡
- **Location**: `package.json` line 5
- **Issue**: References `index.js` which doesn't exist
- **Impact**: Misleading package configuration
- **Fix**: Change to `index.html` or create `index.js`

### 10. **Debug Code in Vendor Files** 🟡
- **Location**: Multiple vendor JavaScript files
- **Issue**: Console.log statements found in production code
- **Impact**: Performance overhead, console pollution
- **Fix**: Use minified versions without debug statements

### 11. **Missing Favicon File** 🟡
- **Location**: `index.html` line 29 references `favicon.ico`
- **Issue**: File doesn't exist in workspace
- **Impact**: 404 error, poor user experience
- **Fix**: Add favicon.ico file or remove reference

## Recommendations

### Immediate Actions (Critical)
1. Fix duplicate ID attribute
2. Update Google Fonts to HTTPS
3. Fix malformed mailto link

### Short Term (1-2 weeks)
1. Add security attributes to external links
2. Fix empty href attributes
3. Update alt text for logos
4. Add missing favicon

### Long Term (Next sprint)
1. Implement proper dependency management
2. Update package.json configuration
3. Review and clean vendor files
4. Implement comprehensive testing

## Testing Checklist
- [ ] HTML validation passes
- [ ] All links functional
- [ ] HTTPS deployment works without mixed content warnings
- [ ] Accessibility audit passes WCAG 2.1 AA
- [ ] Email links open correctly
- [ ] No console errors in browser

## Impact Assessment
- **High**: 3 critical issues affecting functionality and security
- **Medium**: 5 issues affecting user experience and best practices
- **Low**: 3 issues affecting maintainability

**Total Issues**: 11 bugs found requiring attention.