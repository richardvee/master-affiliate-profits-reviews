# Master Affiliate Profits Landing Page - Maintenance Guide

This guide will help you maintain and customize the Master Affiliate Profits landing page. It's written for beginners with no prior coding experience.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your main navigation and logo. To update:

1. **Logo Text:**
```html
<!-- Find this line in the header section -->
<a href="#" class="text-xl font-bold bg-gradient-to-r from-blue-500 to-purple-600 bg-clip-text text-transparent">Master Affiliate Profits</a>
```
Simply replace "Master Affiliate Profits" with your desired text.

2. **Navigation Menu Items:**
```html
<a href="#features" class="text-gray-300 hover:text-white transition-colors duration-300">Features</a>
```
To modify menu items:
- Change the text between `<a>` tags
- Keep the `href` attribute matching your section IDs
- Maintain the existing classes for consistent styling

### Hero Section
Located at the top of the page:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8 bg-gradient-to-r from-blue-400 to-purple-500 bg-clip-text text-transparent">Master Affiliate Profits: The Ultimate All-in-One System</h1>
```

To update:
1. Replace the heading text
2. Keep all classes to maintain responsive sizing:
   - `text-4xl`: Mobile size
   - `md:text-5xl`: Tablet size
   - `lg:text-6xl`: Desktop size

### Tailwind CSS Classes Explained

Common classes used throughout:
- `container mx-auto`: Centers content with automatic margins
- `px-4 sm:px-6 lg:px-8`: Responsive padding
- `grid grid-cols-1 md:grid-cols-3`: Responsive grid layout
- `hover:scale-105`: Hover animation
- `transition-all duration-300`: Smooth transitions

## Managing Links

### Navigation Links
Current internal links:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
```

To update:
1. Ensure section IDs match these href values
2. For external links, replace "#" with full URL:
```html
<a href="https://yoursite.com/page">Link Text</a>
```

### Call-to-Action (CTA) Links
Current CTA link:
```html
<a href="https://masteraffiliateprofits.com/tdf/aNP0gN" class="inline-block bg-gradient-to-r from-blue-600 to-purple-600">Start Earning Today</a>
```

To update:
1. Replace the URL with your affiliate link
2. Keep all classes for consistent styling
3. Test the link after updating

## Adding Privacy and Terms Pages

### Step 1: Create New Pages
Create two new files in your website directory:
- `privacy.html`
- `terms.html`

### Step 2: Update Footer Links
Locate this section in the footer:
```html
<div>
    <h3 class="text-lg font-semibold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

Replace the `#` with proper paths:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

### Broken Styles
If styles aren't applying:
1. Check the Tailwind CDN link in the header
2. Verify class names are spelled correctly
3. Ensure no spaces in class names

### Links Not Working
If links aren't functioning:
1. Check for typos in URLs
2. Verify file paths are correct
3. Ensure section IDs match href values
4. Test links in different browsers

### Responsive Issues
If layout breaks on mobile:
1. Check responsive classes (sm:, md:, lg:)
2. Verify container widths
3. Test on multiple devices

Need additional help? Contact support at mail@sideincomehub.com

---

Remember to:
- Back up files before making changes
- Test all changes in multiple browsers
- Maintain consistent styling throughout
- Keep responsive design in mind
- Update meta tags when changing content

This guide covers basic maintenance. For advanced customization, consider consulting a web developer.