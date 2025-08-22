# Electronic Music Artist Website

A modern, responsive website for electronic music artists, inspired by professional DJ/producer websites like Afrojack.com.

## Project Structure

```
electronic-artist-website/
├── index.html                 # Main HTML file
├── README.md                 # Project documentation
├── html-theme-font-reference.md  # Theme reference file
└── assets/
    ├── css/
    │   └── styles.css        # Main stylesheet
    ├── js/
    │   └── script.js         # JavaScript functionality
    └── images/
        ├── banner.png        # Hero section background
        ├── logo.svg          # Site logo
        ├── gallery_1.jpg     # Gallery/track images
        ├── gallery_2.jpg
        ├── gallery_3.jpg
        ├── gallery_4.jpg
        ├── school.jpg        # About section image
        ├── hero_fb.svg       # Social media icons
        ├── hero_insta.svg
        ├── hero_sc.svg
        ├── hero_spot.svg
        ├── hero_tube.svg
        ├── hero_whats.svg
        ├── social-facebook-svgrepo-com.svg
        ├── social-soundcloud-svgrepo-com.svg
        ├── social-spotify-svgrepo-com.svg
        ├── social-whats-app-svgrepo-com.svg
        └── social-youtube-svgrepo-com.svg
```

## Features

### Design
- **Dark theme** with vibrant orange/pink gradients
- **Modern typography** using Inter and Poppins fonts
- **Responsive design** that works on all devices
- **Smooth animations** and hover effects
- **Professional electronic music aesthetic**

### Sections
1. **Navigation** - Fixed header with logo and smooth scrolling
2. **Hero Section** - Full-screen banner with social media links
3. **Music Section** - Interactive track cards with play buttons
4. **Gallery** - Photo gallery with lightbox functionality
5. **About** - Artist information with statistics
6. **Contact** - Contact form and booking information
7. **Footer** - Social media links and copyright

### Interactive Features
- Mobile-responsive hamburger menu
- Smooth scrolling navigation
- Animated track cards with play buttons
- Gallery lightbox for viewing images
- Working contact form with validation
- Parallax effects on scroll
- Social media integration
- Easter eggs for engagement

## Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with CSS Grid, Flexbox, and animations
- **JavaScript (ES6+)** - Interactive functionality
- **Google Fonts** - Inter and Poppins typography
- **SVG Icons** - Scalable social media icons

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Setup Instructions

1. Clone or download the project files
2. Ensure all files are in the correct folder structure as shown above
3. Open `index.html` in a web browser
4. No server setup required - runs as static website

## Customization

### Colors
Edit the CSS variables in `assets/css/styles.css`:
```css
:root {
  --primary-color: #ff6b35;
  --secondary-color: #00d4ff;
  --accent-color: #ff0080;
  /* ... other colors */
}
```

### Content
- Update text content in `index.html`
- Replace images in `assets/images/`
- Modify social media links
- Update contact information

### Fonts
The website uses Google Fonts (Inter and Poppins). To change fonts:
1. Update the Google Fonts link in the HTML head
2. Modify the font-family properties in CSS

## Performance Optimizations

- Optimized images
- Minified CSS and JavaScript (production ready)
- Lazy loading for images
- Efficient animations using CSS transforms
- Responsive images for different screen sizes

## License

© 2024 Electronic Artist. All rights reserved.

## Credits

- Design inspired by modern electronic music artist websites
- Icons from SVG Repo
- Fonts from Google Fonts
- Built with modern web standards
