# Dreamland RP - Official Website

A modern, expandable web application for Dreamland RP, inspired by NoPixel's sleek design. Features a stunning home page with easy navigation to our Discord community.

## Features

- 🎨 Modern, sleek design with smooth animations
- 📱 Fully responsive (mobile, tablet, desktop)
- 🎬 Video background support with fallback
- 📊 Animated statistics counter
- 🔗 Easy Discord integration
- ⚡ Fast and lightweight
- 🚀 Easily expandable for future pages
- 🎯 SEO-friendly structure

## Quick Start

1. Clone or download this repository
2. Add your assets to the `assets/` folder:
   - `logo.png` - Your server logo (300x300px recommended)
   - `hero-video.mp4` - Background video (optional)
3. Update the Discord link in `index.html` (search for `discord.gg/dreamlandrp`)
4. Customize content in `index.html`
5. Open `index.html` in a browser or deploy to a web server

## Deployment

### Local Development
Simply open `index.html` in your browser.

### Web Hosting
Upload all files to your web host. The site works with:
- GitHub Pages
- Netlify
- Vercel
- Any static hosting service

### Custom Domain
Point your domain to your hosting provider and update DNS settings accordingly.

## Customization

### Update Server Name & Content
Edit `index.html` and modify:
- Hero title: Line 47
- Hero subtitle: Line 48
- About section content: Lines 66-87
- Statistics: Lines 95-110

### Change Colors & Theme
Edit `css/styles.css` variables (lines 10-17):
```css
:root {
    --primary-color: #5865f2;      /* Main brand color */
    --primary-hover: #4752c4;      /* Hover state */
    --background-dark: #0a0a0a;    /* Dark background */
    --background-light: #1a1a1a;   /* Light background */
    /* ... more variables */
}
```

### Discord Links
Update all Discord links throughout the site:
- Search for `https://discord.gg/dreamlandrp`
- Replace with your actual Discord invite link

### Adding New Pages
The site is built with a router system for easy expansion:

1. Add a new section in `index.html`:
```html
<section id="newpage" class="page">
    <!-- Your content here -->
</section>
```

2. Add navigation link:
```html
<li class="nav-item">
    <a href="#newpage" class="nav-link" data-page="newpage">New Page</a>
</li>
```

3. Add route in `js/main.js`:
```javascript
routes: {
    'home': () => showPage('home'),
    'newpage': () => showPage('newpage')  // Add this
}
```

## File Structure

```
fivem-splash/
├── index.html           # Main HTML file
├── css/
│   └── styles.css       # All styles and animations
├── js/
│   └── main.js          # JavaScript functionality & router
├── assets/
│   ├── logo.png         # Your logo (add this)
│   ├── hero-video.mp4   # Background video (optional)
│   └── README.md        # Asset guidelines
├── .gitkeep
└── README.md            # This file
```

## Features Breakdown

### Navigation
- Fixed header with smooth scrolling
- Mobile-responsive hamburger menu
- Active page indication
- Discord integration with icon

### Hero Section
- Full-screen video background (with fallback)
- Animated title and subtitle
- Call-to-action buttons
- Scroll indicator

### About Section
- Grid layout with feature cards
- Hover animations
- Icon support

### Statistics Section
- Animated counters
- Responsive grid
- Scroll-triggered animations

### Footer
- Links to important pages
- Copyright information
- Responsive layout

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- Optimized animations using CSS transforms
- Lazy-loaded scroll animations
- Minimal JavaScript
- Fast load times

## Future Expansion Ideas

- Rules page
- Staff page
- Application system
- Gallery/Screenshots
- Server statistics API integration
- News/Updates blog
- FAQ section

## License

MIT License - Feel free to modify and use for your community!

## Credits

Created for Dreamland RP
Inspired by NoPixel's modern design aesthetic

readme