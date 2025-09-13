# NFT Digital Renaissance

A modern, responsive landing page for an NFT marketplace featuring elegant design and interactive elements built with pure CSS Grid.

## My Approach

### Layout Strategy
- **CSS Grid Only**: Completely replaced all Flexbox layouts with CSS Grid to meet project requirements
- **Mobile-First Design**: Started with mobile layouts and progressively enhanced for larger screens
- **Semantic HTML**: Used proper HTML5 semantic elements for better accessibility and structure

### Responsive Design Implementation
- **CSS Grid + Media Queries**: Used CSS Grid's powerful layout capabilities combined with strategic breakpoints
- **Clamp() Values**: Implemented clamp() functions throughout for fluid typography and spacing that scales smoothly
- **Relative Units**: Used rem, em, and percentages for scalable design elements

### Interactive Elements
- **Hover Effects**: Added 4 distinct hover interactions:
  - Navigation links: color change + scale effect
  - Signup button: background color change + scale effect
  - NFT cards: translateY + scale + enhanced shadow
  - Start button: gradient background change + scale effect

## What I Struggled With

### CSS Grid Conversion
The most challenging aspect was converting the existing Flexbox-based layout to pure CSS Grid while maintaining the same visual design. The `.main-heading` class was particularly difficult due to:
- Complex gradient text effects that needed to work across different browsers
- Responsive typography using clamp() values
- Maintaining proper line-height with the gradient background
- Ensuring text remained readable at all screen sizes

### Responsive Navigation
Creating a responsive navigation without JavaScript while using only CSS Grid required careful planning of grid template areas and column configurations across different breakpoints.

### Element Positioning
Positioning the floating elements (stone, barcode, side text) while maintaining responsive behavior required precise absolute positioning calculations and responsive adjustments.

## Known Issues

### Browser Compatibility
- **Gradient Text**: The `-webkit-background-clip: text` property may not work in older browsers
- **Clamp() Support**: CSS clamp() function requires modern browser support (IE not supported)

### Performance Considerations
- **Large Images**: The hand sculpture and other images should be optimized for web delivery
- **Font Loading**: Multiple Google Fonts may impact initial page load time

### Responsive Behavior
- **Very Small Screens**: On screens smaller than 320px, some elements may need additional adjustments
- **Landscape Mobile**: Landscape orientation on mobile devices may need specific handling

## File Structure

```
integra manga/
├── index.html          # Main HTML file with semantic structure
├── style.css           # Pure CSS Grid stylesheet with responsive design
├── star.png           # Logo image
├── hand.png           # Hand sculpture image
├── stone.png          # Floating stone image
├── beer.png           # Bear NFT image
├── Lion.png           # Lion NFT image
├── Cat.png            # Cat NFT image
├── barcode.png        # Barcode image
└── README.md          # Project documentation
```

## Technologies Used

- **HTML5**: Semantic markup structure
- **CSS3**: Pure CSS Grid layout system
- **Google Fonts**: Playfair Display, Inter, Merriweather
- **CSS Features**: Grid, Gradients, Transforms, Transitions, Clamp()

## Browser Support

- **Recommended**: Chrome, Firefox, Safari, Edge (latest versions)
- **CSS Grid**: Supported in all modern browsers
- **Clamp()**: Requires modern browser support
- **Gradient Text**: Webkit-based browsers for full effect