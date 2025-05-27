# Jewelry Landing Page - Maintenance Guide

This guide will help you maintain and customize the Jewelry Landing Page. It's written for beginners and provides detailed instructions for common maintenance tasks.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Policy Pages](#adding-policy-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your brand name and navigation menu. To update:

1. **Brand Name**: Locate this line in the header:
```html
<a href="#" class="text-2xl font-bold">JEWELRY</a>
```
Simply replace "JEWELRY" with your brand name.

2. **Navigation Menu Items**: Find these lines:
```html
<a href="#" class="text-gray-600 hover:text-black transition-colors duration-300">Shop</a>
<a href="#" class="text-gray-600 hover:text-black transition-colors duration-300">Collections</a>
<a href="#" class="text-gray-600 hover:text-black transition-colors duration-300">About</a>
<a href="#" class="text-gray-600 hover:text-black transition-colors duration-300">Contact</a>
```
Replace "Shop", "Collections", etc., with your desired menu items.

### Hero Section
To update the hero section:

1. **Main Heading**: Find:
```html
<h1 class="text-4xl md:text-6xl font-bold text-white mb-6 leading-tight">
    Jewelry Timeless Elegance and Crafted
</h1>
```
Replace the text while keeping the classes intact.

2. **Background Image**: Locate:
```html
<img src="https://images.unsplash.com/photo-1504093376055-b3094b674dcb?w=1600&h=900&fit=crop&q=80" 
```
Replace the URL with your image link.

### Tailwind CSS Classes Explained
Common classes used in this page:
- `text-{size}`: Controls text size (e.g., `text-xl`, `text-2xl`)
- `md:text-{size}`: Applies text size on medium screens and up
- `bg-{color}`: Sets background color
- `text-{color}`: Sets text color
- `py-{number}`: Adds padding top and bottom
- `px-{number}`: Adds padding left and right

## Managing Links

### Navigation Menu Links
1. Locate all `href="#"` attributes in the navigation:
```html
<div class="hidden md:flex items-center space-x-8">
    <a href="#" class="text-gray-600 hover:text-black transition-colors duration-300">Shop</a>
    <!-- Other menu items -->
</div>
```
2. Replace `#` with your actual URLs:
```html
<a href="/shop" class="text-gray-600 hover:text-black transition-colors duration-300">Shop</a>
```

### Call-to-Action Links
Update the "Explore Collection" and "Shop Now" buttons:
```html
<a href="https://www.landingpages.kalaharriwebagency.online" 
   class="inline-block bg-white text-black px-8 py-4 rounded-full">
    Explore Collection
</a>
```
Replace the URL with your collection page link.

## Adding Policy Pages

### Footer Policy Links
1. Locate the policies section in the footer:
```html
<div>
    <h3 class="text-xl font-bold mb-4">Policies</h3>
    <ul class="space-y-2 text-gray-400">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Shipping Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Return Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
    </ul>
</div>
```

2. Add links to your policy pages:
```html
<li><a href="/privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="/terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

### Social Media Links
Update social media links in the footer:
```html
<div class="flex space-x-4">
    <a href="https://instagram.com/your-account" class="text-2xl hover:text-gray-400">
        <i class="fab fa-instagram"></i>
    </a>
    <!-- Repeat for other social media -->
</div>
```

## Troubleshooting

### Common Issues

1. **Images Not Loading**
   - Verify image URLs are correct and accessible
   - Ensure images are properly hosted
   - Check for typos in the `src` attribute

2. **Responsive Design Issues**
   - Look for classes starting with `md:` for medium screen styles
   - Test the page at different screen sizes
   - Don't remove responsive classes unless you're sure about the impact

3. **Link Problems**
   - Test all links after updating
   - Ensure URLs start with `/` for internal links
   - Include `https://` for external links

### Need Help?
If you encounter issues:
1. Check the browser's developer tools (F12) for errors
2. Verify all HTML tags are properly closed
3. Ensure Tailwind CSS is properly loaded
4. Contact technical support if problems persist

Remember to always backup your code before making changes and test thoroughly after updates.