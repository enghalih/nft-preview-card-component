# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements (image overlay, titles, and creator name)

### Links

![screenshot image](image-1.png)  

- Live Site URL: [Live Site](https://enghalih.github.io/nft-preview-card-component)

## My process

### Built with

- Semantic HTML5 markup
- SCSS / SASS
- BEM (Block Element Modifier) methodology
- Flexbox
- Mobile-first workflow

### What I learned

I focused on writing maintainable code by combining BEM with SCSS nesting. This kept the stylesheet organized and easy to read.

One specific trick I used was managing the hover overlay transparency. To prevent the icon from becoming semi-transparent, I applied transparency directly to the background color using `hsla` instead of the `opacity` property:

```scss
.card {
  &__view {
    opacity: 0;
    transition: opacity 300ms ease, background-color 300ms ease;
    background-color: transparent;
    &:hover {
      background-color: hsla(178, 100%, 50%, 0.5);
      opacity: 1;
    }
}

```

### Continued development

I want to refine my SCSS workflow by creating a more robust system for [CSS Variables](https://developer.mozilla.org) that can be easily integrated into `hsla` functions for better theme management.

## Author

- Frontend Mentor - [@enghalih](https://www.frontendmentor.io/profile/enghalih)
- Github - [@enghalih](https://github.com/enghalih)
- Linkedin - [Wenning Ghalih](https://www.linkedin.com/in/enghalih/)
