# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa) on Frontend Mentor.

Frontend Mentor challenges help improve front-end development skills by building realistic projects from professional designs.

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
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size.
- See hover and focus states for interactive elements.
- View the product information, pricing, and add-to-cart button in a responsive layout.

### Screenshot

![Product preview card component](./images/Screenshot%202026-10-17%20194306.png)

### Links

- Solution URL: [GitHub Repository](https://github.com/AdanIrfan/frontend-mentor-challenges/tree/main/newbie/product-preview-card-component)
- Live Site URL: [Product Preview Card](https://productpreviewcard201.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Responsive design
- Mobile-first workflow
- Responsive images using the `<picture>` element
- CSS `clamp()` for fluid typography
- Custom fonts using `@font-face`

### What I learned

This project helped me improve my understanding of responsive layouts and how to translate a design into HTML and CSS.

#### Responsive images

I learned how to use the `<picture>` element to display different images depending on the screen size.

```html
<picture>
  <source
    media="(min-width: 600px)"
    srcset="./images/image-product-desktop.jpg"
  />
  <img
    src="./images/image-product-mobile.jpg"
    alt="Chanel Gabrielle Essence perfume bottle on a table beside green leaves"
  />
</picture>
```

This allowed me to use a different crop of the product image for mobile and desktop layouts.

#### Responsive typography

I also practised using `clamp()` to control font sizes across different viewport sizes.

```css
.product-card h1 {
  font-size: clamp(2.5rem, 2rem + 1vw, 3rem);
}
```

This helped me understand the difference between minimum, preferred, and maximum font sizes.

#### CSS custom properties

I used CSS variables to keep the main colors consistent and make the stylesheet easier to maintain.

```css
:root {
  --background-color: hsl(30, 38%, 92%);
  --white-color: hsl(0, 0%, 100%);
  --accent-colorgreen: hsl(158, 36%, 37%);
}
```

#### Flexbox

I used Flexbox to center the card and change the product card from a vertical layout on smaller screens to a horizontal layout on larger screens.

### Continued development

In future projects, I want to continue improving:

- Responsive typography and when to use fluid versus fixed font sizes.
- Matching spacing and typography more accurately to the reference design.
- Choosing responsive breakpoints based on the content rather than arbitrary screen widths.
- Accessibility and keyboard focus states.
- Responsive image techniques and image sizing.
- Writing cleaner and more maintainable CSS.

I also want to become more confident in judging design differences between my implementation and the reference without relying only on visual guessing.

### Useful resources

- [MDN - `<picture>` element](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/picture) - Helped me understand how to provide different images for different viewport conditions.
- [MDN - CSS `clamp()`](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp) - Helped me understand how to create fluid values with minimum and maximum limits.
- [MDN - CSS Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout) - Helped me understand the layout and alignment of the product card.
- [Frontend Mentor](https://www.frontendmentor.io/) - Used for the challenge design and project requirements.

### AI Collaboration

I used ChatGPT as a learning and review assistant during this project.

I mainly used AI to:

- Understand responsive CSS concepts.
- Ask questions about `clamp()`, `rem`, `vw`, Flexbox, and responsive images.
- Review my HTML and CSS for potential improvements.
- Get feedback on accessibility and responsive design.
- Understand why certain CSS approaches worked or caused layout issues.

I used AI primarily for explanations, debugging guidance, and code review rather than generating the entire project. I still wrote and tested the implementation myself.

One of the most useful parts of the collaboration was learning how to reason about responsive typography instead of simply adding `clamp()` values without understanding their effect.

## Author

- GitHub - [@AdanIrfan](https://github.com/AdanIrfan)
- Frontend Mentor - [@AdanIrfan](https://www.frontendmentor.io/profile/AdanIrfan)

## Acknowledgments

Thanks to [Frontend Mentor](https://www.frontendmentor.io/) for providing the challenge and design.

I also used feedback and AI-assisted code reviews to identify areas where I could improve my responsive design, typography, accessibility, and CSS structure.
