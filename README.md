# Frontend Mentor - Fylo landing page with dark theme and features grid

![Design preview for the Fylo landing page with dark theme and features grid challenge](./design/desktop-preview.jpg)

# Frontend Mentor - NFT preview card component solution

This is a solution to the [Fylo dark theme landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/fylo-dark-theme-landing-page-5ca5f2d21e82137ec91a50fd). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
- [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![screenshot-final.png](screenshot-final.png)

### Links

[Demo](https://loquacious-pie-88f4f4.netlify.app/)

## My process

I used only flexbox, no media query for images, and HTML validator (so no JS to display error message)

### Built with

- Semantic HTML5 markup
- CSS
- Flexbox

### What I learned

I learned to use flexbox.

I also used `srcset` in `<picture>` to not use media query on picture display.


```html
<picture class="block-curvy-desktop">
  <source
    media="(max-width: 375px)"
    srcset="images/bg-curvy-mobile.svg">
  <img class="bg-curvy-desktop" src="images/bg-curvy-desktop.svg" alt="background curvy desktop" />
</picture>
```

I also use the HTML validator to avoid JS

```html
<input type="email" placeholder="email@example.com">
<div class="error-message">Please provide a valid email</div>
```

```css
.error-message {
  visibility: hidden;
  font-weight: 300;
  color: hsl(var(--ligh-red));
}
input:invalid ~ .error-message {
  visibility: visible;
}
```
