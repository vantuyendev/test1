# Legendary Pokemon Index - CSS Styling Assignment

A beautifully designed Pokemon fan website showcasing legendary Pokemon from across all generations. This project demonstrates advanced CSS styling techniques including accessibility features, grid and flexbox layouts, the box model, and interactive elements.

## 🎮 About This Site

This website celebrates legendary Pokemon with:
- **Home Page**: Overview of legendary Pokemon groups (Birds, Beasts, Weather Trio, Creation Trio)
- **Legendaries Gallery**: Showcase of 6 iconic legendary Pokemon (Mewtwo, Lugia, Rayquaza, Giratina, Zekrom, Arceus)
- **About Page**: Pokemon franchise information and legendary Pokemon lore

## 🎯 Assignment Requirements Checklist

All requirements have been implemented in this project:

### ✅ HTML Structure
- [x] Three pages of HTML code (index.html, gallery.html, about.html)
- [x] Every page has at least one image
- [x] Gallery page has 6 images (exceeds 5 minimum requirement)
- [x] All HTML validates with W3C Validator

### ✅ Accessibility
- [x] **Skip to Main Content Link** - Implemented with position property and :focus pseudo-class (only visible when focused)
- [x] Semantic HTML structure (header, nav, main, section, footer)
- [x] Descriptive alt text for all images
- [x] Proper heading hierarchy (h1, h2, h3)

### ✅ Navigation
- [x] Attractive, styled navigation bar
- [x] Uses Flexbox for layout
- [x] Styled with multiple CSS properties:
  - Background color with transparency
  - Padding and border-radius
  - Font-weight and text-transform
  - Letter-spacing
  - Transition effects

### ✅ Box Model
- [x] All images styled using:
  - Border (4px solid with color)
  - Padding (4px inner spacing)
  - Border-radius (12px or 50% for variety)
  - Box-shadow for depth
  - Background color

### ✅ Layout Properties
- [x] **Grid Layout** - Used on `.features-grid` (index.html) with `repeat(auto-fit, minmax(250px, 1fr))`
- [x] **Grid Layout** - Also used on `.about-content` (about.html) with 2 columns
- [x] **Flexbox** - Used on `.nav-list` for navigation
- [x] **Flexbox** - Used on `.flex-gallery` (gallery.html) for image layout
- [x] **Flexbox** - Used on `.skills-list` (about.html) for skill badges

### ✅ Interactive Elements
- [x] **:hover Pseudo-class** - Multiple implementations:
  - Navigation links with transform and shadow
  - Feature cards with lift effect
  - Images with scale effect
  - Skill badges with scale effect
  - Links with color change

- [x] **:nth-child Selector** - Multiple implementations:
  - Gallery images alternate between circular (odd) and rounded (even) borders
  - Gallery images have alternating border colors
  - Feature cards have different colored top borders based on position

### ✅ Validation
- [x] Code ready for W3C HTML Validator (https://validator.w3.org/)
- [x] Code ready for WAVE accessibility checker (https://wave.webaim.org/)

## 📁 Project Structure

```
├── index.html          # Home page with grid layout
├── gallery.html        # Gallery page with 6+ images and flexbox
├── about.html          # About page with profile and skills
├── styles.css          # Main stylesheet with all CSS requirements
├── images/             # Directory for your images
│   └── README.md       # Instructions for adding your images
└── README.md           # This file
```

## 🚀 Getting Started

### 1. Add Your Pokemon Images
Navigate to the `images/` folder and read the README.md file there. You need to add 11 images total:
- **4 legendary group images** for the home page (Birds, Beasts, Weather Trio, Creation Trio)
- **6 individual legendary Pokemon** for the gallery (Mewtwo, Lugia, Rayquaza, Giratina, Zekrom, Arceus)
- **1 Pokemon logo** or Pokeball image for the about page

**Where to get images:**
- Bulbapedia (official artwork)
- Pokemon Database
- Serebii.net
- Official Pokemon.com website
- Pokemon Trading Card Game artwork
- See `images/README.md` for detailed guidance

### 2. Customize Content (Optional)
- Update text to add your personal touch
- Change legendary Pokemon selections to your favorites
- Add more Pokemon information

### 3. Test Your Site
Open `index.html` in a web browser to view your Legendary Pokemon Index!

## ✅ Validation Steps

### HTML Validation
1. Go to https://validator.w3.org/
2. Choose "Validate by File Upload" or "Validate by Direct Input"
3. Upload or paste each HTML file (index.html, gallery.html, about.html)
4. Fix any errors or warnings that appear
5. Aim for "Document checking completed. No errors or warnings to show."

### Accessibility Validation
1. Go to https://wave.webaim.org/
2. Enter your live site URL (or use the WAVE browser extension for local testing)
3. Review the results:
   - Check for errors (red icons)
   - Review alerts (yellow icons)
   - Verify features (green icons)
4. Fix any critical accessibility issues

### Manual Testing
- **Skip Link**: Press Tab when the page loads - the "Skip to Main Content" link should appear
- **Navigation**: Verify all links work and highlight on hover
- **Responsive**: Resize browser window to test mobile layout
- **Images**: Confirm all images load and have proper borders/styling
- **Hover Effects**: Move mouse over cards, images, and links to see transitions

## 🎨 CSS Features Demonstrated

### Pokemon Color Scheme
The site uses the iconic Pokemon brand colors:
- **Primary Red**: #CC0000 (Pokeball red)
- **Primary Blue**: #3B4CCA (Pokemon blue)
- **Primary Yellow**: #FFDE00 (Pikachu yellow)
- **Gradients**: Combines all three colors for dynamic backgrounds

### Skip to Main Content (Accessibility)
```css
.skip-link {
    position: absolute;
    top: -40px;  /* Hidden by default */
}

.skip-link:focus {
    top: 0;      /* Visible when focused */
}
```

### Grid Layout (2+ columns)
```css
.features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
}
```

### Flexbox Layout
```css
.nav-list {
    display: flex;
    justify-content: center;
    gap: 2rem;
}
```

### Box Model on Images
```css
.feature-card img {
    border: 4px solid #667eea;
    padding: 4px;
    border-radius: 12px;
}
```

### Hover Effects
```css
.feature-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 12px 24px rgba(0, 0, 0, 0.2);
}
```

### nth-child Selector
```css
.gallery-item:nth-child(odd) img {
    border-radius: 50%;
}

.gallery-item:nth-child(even) img {
    border-radius: 12px;
}
```

## 📝 Before Submission

- [ ] All images added to the images/ folder
- [ ] Content customized with your own text
- [ ] HTML validated with W3C Validator (all 3 pages)
- [ ] Accessibility checked with WAVE
- [ ] All links tested and working
- [ ] Skip link tested (press Tab)
- [ ] Hover effects verified
- [ ] Site viewed in multiple browsers
- [ ] Mobile responsiveness checked

## 🌐 Deployment Options

To submit your site, you can deploy it using:
- **GitHub Pages** (recommended)
- **Netlify**
- **Vercel**
- Any other web hosting service

## 💡 Tips

- Use official Pokemon artwork (Ken Sugimori art) for the best results
- Bulbapedia and Pokemon Database have high-quality images
- The color scheme uses Pokemon's iconic red, blue, and yellow
- Customize legendary Pokemon selections to feature your favorites
- Test the site on different devices and browsers
- Make sure all images are optimized (under 500KB each)

## 📚 Resources

- [W3C HTML Validator](https://validator.w3.org/)
- [WAVE Accessibility Tool](https://wave.webaim.org/)
- [Pokemon Official Site](https://www.pokemon.com/)
- [Bulbapedia](https://bulbapedia.bulbagarden.net/)
- [Pokemon Database](https://pokemondb.net/)
- [Serebii.net](https://www.serebii.net/)
- [MDN Web Docs - CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)

---

**Note**: This is a fan-made educational project. Pokemon and all related content are owned by Nintendo, Game Freak, and The Pokemon Company. Not affiliated with or endorsed by The Pokemon Company.