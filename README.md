# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

The goal was to recreate the design as closely as possible while ensuring responsiveness and accessibility.

### Screenshot

![Desktop Solution Preview](./screenshot.jpg)

### Links

- Solution URL: [GitHub Solution URL](https://github.com/whitgunt77/four-card-feature-section)
- Live Site URL: [Live Site URL](https://whitgunt77.github.io/four-card-feature-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (variables)
- Flexbox
- CSS Grid
- Mobile-first workflow
- Responsive typography using `clamp()`
- Clean component-based CSS structure

### What I learned

This project strengthened my understanding of combining **CSS Grid and Flexbox** for layout control.

One key improvement area was structuring the 3-column desktop layout while stacking cards correctly on mobile. Using nested grid containers made this much cleaner and easier to manage.

I also practiced:

- Creating reusable card components
- Using CSS custom properties for consistent design tokens
- Applying subtle box shadows for depth without overdoing it
- Keeping HTML semantic and accessible

Example of the grid structure used for the desktop layout:

```css
.cards {
  display: grid;
  gap: 1.6rem;
}

@media (min-width: 900px) {
  .cards {
    grid-template-columns: 1fr 1fr 1fr;
  }
}
```

And a reusable card pattern:

```css
.card {
  background: white;
  border-radius: 10px;
  box-shadow: 0 14px 24px rgba(0,0,0,0.08);
  padding: 1.7rem;
}
```

### Continued development

In future projects, I want to:

- Improve my layout precision when matching design files pixel-for-pixel
- Refine my responsive design approach for more complex grid systems
- Continue improving accessibility practices
- Add subtle animations and micro-interactions for enhanced UX

### Useful resources

- [MDN Web Docs &mdash; CSS Grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout) - MDN was my go-to for confirming syntax and understanding how nested grids behave. It's great for checking browser support and reinforcing best practices.
- [CSS Grid Layout Guide &mdash; CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This guide help me better understand how to structure the three-column desktop layout while keeping the middle cards stacked. The visual diagrams made it much easier to think through grid areas and column distribution.
- [A Complete Guide to Flexbox &mdash; CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - I referenced this while aligning content inside each card. It was especially helpful for understanding how to push the icons to the bottom using `margin-top: auto` and flex column behavior.
- [MDN Web Docs &mdash; CSS Custom Properties (Variables)](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) - This helped me confidently structure my design tokens using `:root` variables for consistent color management throughout my project.
- [Frontend Mentor Community Solutions](https://www.frontendmentor.io/solutions) - Reviewing other submissions helped me compare layout strategies and improve my responsiveness approach without copying solutions, It was useful for seeing alternative grid structures.
- [Google Fonts &mdash; Poppins](https://fonts.google.com//specimen/Poppins) - I used this to properly implement the font weights (200, 400, 600) required by the design while maintaining performance and readability.

## Author

- **Name:** Whitney Gunter
- **Frontend Mentor:** [Frontend Mentor Profile Link](https://www.frontendmentor.io/profile/whitgunt77)
- **GitHub:** [GitHub Profile Link](https://www.github.com/whitgunt77)

## Acknowledgments

Design and challenge provided by **Frontend Mentor**

[](https://www.frontendmentor.io)

All design files, starter assets, and challenge requirements belong to Frontend Mentor. This project was built as part of their front-end practice challenges.
