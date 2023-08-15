# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![Image](./screenshot.png)

### Links

- Solution URL: [Add solution URL here](https://github.com/Tabebash/Nft-preview-card-component)
- Live Site URL: [Add live site URL here](https://tabebash.github.io/Nft-preview-card-component/)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I am thankful for this knowledge

```html
<a href="#" class="click-link">
      <div class="container-overlay">
        <img src="./images/image-equilibrium.jpg" class="card-img-top border rounded-3 border-opacity-10" alt="...">
        <div class="overlay border rounded-3 border-opacity-0">
        </div>
        <div class="overlay-icon">
          <svg width="48" height="48" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path d="M0 0h48v48H0z"/><path d="M24 9C14 9 5.46 15.22 2 24c3.46 8.78 12 15 22 15 10.01 0 18.54-6.22 22-15-3.46-8.78-11.99-15-22-15Zm0 25c-5.52 0-10-4.48-10-10s4.48-10 10-10 10 4.48 10 10-4.48 10-10 10Zm0-16c-3.31 0-6 2.69-6 6s2.69 6 6 6 6-2.69 6-6-2.69-6-6-6Z" fill="#FFF" fill-rule="nonzero"/></g></svg>
        </div>
      </div>
    </a>
```
```css
 .container-overlay {
      position: relative;
      width: 100%;
    }

    .overlay {
      position: absolute;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;
      height: 100%;
      width: 100;
      opacity: 0;
      background: var(--CYAN);
      transition: 0.3 ease;
      border-color: var(--CARD-BG) !important;
    }

    .container-overlay:hover .overlay {
      opacity: 0.5;

    }

    .overlay-icon {
      color: var(--WHITE);
      font-size: 1rem;
      position: absolute;
      top:50%;
      left:50%;
      transform: translate(-50%, -50%);
      transition: 0.3 ease;
      opacity:0;
    }

    .container-overlay:hover .overlay-icon {
      opacity: 1 !important;
    }
```

### Useful resources

- [Example resource 1](https://www.w3schools.com/howto/howto_css_image_overlay_icon.asp) - helped me with the image hover design.
- [Example resource 2](https://stackoverflow.com/questions/35903574/how-to-make-a-whole-section-elements-area-clickable) - This helped me with the semantic solution to the clickable image overlay.

## Acknowledgments

Big thanks to everyone helping out via stackoverflow, and a special thanks to Mdn and w3schools for providing such valuable resources for free.
