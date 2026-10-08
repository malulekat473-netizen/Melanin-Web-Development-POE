# Melanin Son - Developer Guide

## Quick Start

### Running the Local Server
```bash
cd "c:\Users\Student\Documents\Melanin Son"
node server.js
```
Visit: **http://localhost:8000/**

---

## Project Structure

```
Melanin Son/
├── index.html                 # Home page
├── README.md                  # Project documentation
├── DEBUG_REPORT.md           # Debug report
├── server.js                 # Local test server
├── assets/
│   ├── css/
│   │   └── style.css         # Main stylesheet (600+ lines)
│   ├── images/               # Image assets (add here)
│   └── js/
│       └── script.js         # Interactive features
└── pages/
    ├── about.html            # About Us page
    ├── contact.html          # Contact page
    ├── donate.html           # Donation page
    └── shop.html             # Shop page
```

---

## CSS Variables (Customization)

Edit `:root` in `style.css` to change colors:

```css
:root {
    --primary-color: #D4AF37;      /* Gold */
    --secondary-color: #1a1a1a;    /* Black */
    --accent-color: #8B4513;       /* Brown */
    --text-dark: #2c2c2c;
    --text-light: #f5f5f5;
    --bg-light: #fafafa;
    --bg-white: #ffffff;
}
```

---

## Adding Content

### Add Images
1. Place images in `/assets/images/`
2. Reference in HTML: `<img src="../assets/images/filename.jpg" alt="Description">`

### Add Products to Shop
Edit `pages/shop.html` and add:
```html
<div class="product-card card">
    <img src="../assets/images/product.jpg" alt="Product Name">
    <h3>Product Name</h3>
    <p class="product-price" data-price="99.99">$99.99</p>
    <button class="btn">Add to Cart</button>
</div>
```

### Update Founder Info
Search for "Lethabo Sekati" in:
- `index.html`
- `pages/about.html`
- `README.md`

---

## JavaScript Features

### Form Validation
The script automatically validates contact forms with:
- Required field checking
- Email format validation
- User feedback with alerts

### Smooth Scrolling
Anchor links (`<a href="#section">`) scroll smoothly to target.

### Keyboard Shortcuts
- **Alt + M**: Jump to main content
- **Alt + H**: Go home

### Active Link Highlighting
Current page link in navigation highlights automatically.

---

## Responsive Breakpoints

```css
/* Desktop: 1200px and up (default) */
/* Tablet: 768px and below */
/* Mobile: 480px and below */
```

Edit media queries in `style.css` to adjust breakpoints.

---

## Accessibility Checklist

When adding new content:
- ✅ Use semantic HTML (header, nav, main, section, footer, article)
- ✅ Provide alt text for all images
- ✅ Ensure color contrast is adequate
- ✅ Use proper heading hierarchy (h1, h2, h3...)
- ✅ Label all form inputs
- ✅ Test keyboard navigation
- ✅ Test with screen readers

---

## Performance Tips

1. **Optimize Images**: Compress images to <200KB each
2. **Minify CSS/JS**: Use minifiers for production
3. **Lazy Loading**: Add `loading="lazy"` to images below fold
4. **Caching**: Set proper cache headers on server
5. **CDN**: Consider using CDN for assets

---

## Deployment Checklist

- [ ] Test all links on live server
- [ ] Verify forms send emails/submissions
- [ ] Check images load correctly
- [ ] Test on multiple devices
- [ ] Verify SSL certificate (HTTPS)
- [ ] Set up analytics
- [ ] Configure security headers
- [ ] Enable GZIP compression
- [ ] Set up error monitoring
- [ ] Create sitemap.xml
- [ ] Submit to search engines

---

## Useful Resources

### CSS
- [MDN CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [CSS Tricks](https://css-tricks.com)

### JavaScript
- [MDN JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [JavaScript.info](https://javascript.info)

### Accessibility
- [WebAIM](https://webaim.org)
- [WCAG 2.1](https://www.w3.org/WAI/WCAG21/quickref/)

### Web Development
- [Can I Use](https://caniuse.com)
- [W3C Validator](https://validator.w3.org)

---

## Troubleshooting

### Styles Not Loading
- Check file path in `<link>` tag
- Verify `assets/css/style.css` exists
- Clear browser cache (Ctrl+Shift+R)

### Forms Not Working
- Check JavaScript console for errors (F12)
- Ensure `script.js` is linked correctly
- Verify form field names match script

### Images Not Showing
- Verify image paths are correct
- Check image file exists in `/assets/images/`
- Confirm image format is supported (jpg, png, webp)

### Responsive Design Issues
- Test on actual devices, not just browser resize
- Check CSS media queries for correct breakpoints
- Ensure `<meta name="viewport">` is in head

---

## Git Ignore (for version control)

```
node_modules/
.DS_Store
*.log
.env
dist/
build/
```

---

## Contact Information

**Organization:** Melanin Son  
**Slogan:** The Son of Soil  
**Email:** malulekat473@gmail.com  
**Instagram:** @melanin_son1
**Location:** Pretoria North, North Park, South Africa

---

## Last Updated
August 19, 2026

## Status
✅ **PRODUCTION READY**
