````markdown
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
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

The goal was to recreate the provided Four Card Feature Section design as closely as possible while making the layout responsive across different screen sizes.

### Screenshot

![Four card feature section](./images/Screenshot%202026-10-18%20210518.png)

### Links

- Solution URL: [GitHub Repository](https://github.com/AdanIrfan/frontend-mentor-challenges/tree/main/newbie/four-card-feature-section)
- Live Site URL: [Four Card Feature Section](https://fourcardfeature201.netlify.app/)

## My process

I started by studying the provided design and identifying the main layout structure, typography, spacing, colors, and card positioning.

I first created the semantic HTML structure for the page, including the introduction section and the four feature cards.

For the desktop layout, I used CSS Grid to position the four cards. The Supervisor and Calculator cards span two rows, while the Team Builder and Karma cards are positioned in the middle.

I then used Flexbox inside the individual cards to control the content layout and position the card icons.

After completing the desktop layout, I added responsive styles using a media query to change the grid into a single-column layout on smaller screens.

Throughout the project, I focused on matching the reference design while practicing responsive layout techniques, typography, spacing, and CSS maintainability.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Flexbox
- Responsive design
- Desktop-first responsive workflow
- CSS media queries
- CSS `clamp()` for responsive typography
- `@font-face` for local fonts

### What I learned

This project helped me improve my understanding of CSS Grid and how it can be used to create more complex layouts.

One of the main concepts I practiced was making a grid item span multiple rows:

```css
.card--supervisor {
  grid-column: 1;
  grid-row: 1 / 3;
  align-self: center;
}

.card--calculator {
  grid-column: 3;
  grid-row: 1 / 3;
  align-self: center;
}
```
````

Using `grid-row: 1 / 3` allows a card to occupy both the first and second grid rows.

I also learned how `align-self: center` can vertically center an individual grid item within its grid area.

Another useful concept I practiced was using Flexbox inside the cards:

```css
.card {
  display: flex;
  flex-direction: column;
}
```

This allowed me to control the vertical arrangement of the card content.

I also practiced using `margin-top: auto` to push the card icon toward the bottom of the card:

```css
.card img {
  margin-top: auto;
  align-self: flex-end;
}
```

### Responsive typography

I practiced using CSS `clamp()` to make typography responsive:

```css
.intro h1 {
  font-size: clamp(2rem, 2vw + 1rem, 3rem);
}
```

`clamp()` allows a value to have a minimum, preferred, and maximum size, making the typography adapt to different viewport sizes.

### CSS custom properties

I used CSS custom properties to store the colors used throughout the project:

```css
:root {
  --red: hsl(0, 78%, 62%);
  --cyan: hsl(180, 62%, 55%);
  --orange: hsl(34, 97%, 64%);
  --blue: hsl(212, 86%, 64%);
}
```

This makes the stylesheet easier to maintain because the colors can be changed from one central location.

### Continued development

In future projects, I want to continue improving:

- CSS Grid layout and positioning
- Choosing when to use Grid versus Flexbox
- Responsive typography
- Responsive spacing
- Choosing appropriate breakpoints
- Matching designs more accurately
- Testing layouts at intermediate screen sizes
- Accessibility and keyboard navigation
- Writing cleaner and more maintainable CSS
- Understanding when to use fixed versus fluid CSS values

I also want to become more comfortable with planning the layout before writing the CSS so I can reproduce designs more accurately and efficiently.

### Useful resources

- [MDN - CSS Grid Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout) - Helped me understand CSS Grid and how grid items can be positioned across rows and columns.

- [MDN - CSS Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout) - Helped me understand how to arrange and align elements inside the feature cards.

- [MDN - CSS `clamp()`](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp) - Helped me understand responsive values for typography.

- [MDN - `align-self`](https://developer.mozilla.org/en-US/docs/Web/CSS/align-self) - Helped me understand how individual grid and flex items can be aligned.

- [Frontend Mentor](https://www.frontendmentor.io/) - Provided the design challenge and assets used to build the project.

### AI Collaboration

I used ChatGPT as an AI learning and review assistant during this project.

I mainly used AI for:

- Understanding CSS Grid concepts
- Understanding how `grid-row` works
- Understanding how `align-self` can center grid items
- Debugging layout issues
- Getting guidance on responsive CSS
- Understanding responsive typography and `clamp()`
- Reviewing CSS structure and maintainability
- Getting feedback on responsive design decisions

AI was primarily used for explanations, debugging guidance, and code review rather than generating the complete project.

I wrote and tested the implementation myself and made the final design and coding decisions.

## Author

- GitHub - [@AdanIrfan](https://github.com/AdanIrfan)
- Frontend Mentor - [@AdanIrfan](https://www.frontendmentor.io/profile/AdanIrfan)

## Acknowledgments

Thanks to [Frontend Mentor](https://www.frontendmentor.io/) for providing the challenge, design, and assets.

I also used AI-assisted explanations and code reviews as part of my learning process. This helped me better understand CSS Grid, Flexbox, responsive design, and CSS layout techniques while working through the challenge.

```

```
