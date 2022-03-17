# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview
  Making a NFT Preview Card Component with HTML and CSS
### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./screenshots/Screenshot%20of%20Desktop%20Design.png)

### Links

- Solution URL: https://www.frontendmentor.io/solutions/responsive-nft-card-using-html-and-css-wVdp_JKLA
- Live Site URL: https://ipogeni.github.io/NFT-Preview-Card-Component/

## My process
  Finished making the basic markups for the design, set tags that seemed appropriate. Styled the markups as per the designs and went back to HTML for additional active and hover effects.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned
Learned how to use icons alongside texts and how to create an overlay

```html
<div class="card-img">
    <img src="./images/image-equilibrium.jpg" alt="a transparent cube in equilibrium on one of its vertices">
    <div class="overlay">
      <img src="./images/icon-view.svg" alt="view icon">
    </div>
  </div>
<div class="card-price-time">
      <div class="card-price">
        <img src="./images/icon-ethereum.svg" alt="etherium icon">
        <p>0.041 ETH</p>
      </div>
      <div class="card-time">
        <img src="./images/icon-clock.svg" alt="">
        <p>3 days left</p>
      </div>
    </div>
```
```css
.card-img{
    position: relative;
    width: 100%;
}

.overlay{
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    height: 100%;
    width: 100%;
    opacity: 0;
    transition: 0.4s ease-in;
    background-color: hsla(178, 100%, 50%, 0.5);
    border-radius: 8px;
}

.card-img:hover .overlay{
    opacity: 1;
    cursor: pointer;
}
```

## Author

- Github - [Protaya Roy](https://github.com/IPogenI)
- Frontend Mentor - [Pogen](https://www.frontendmentor.io/profile/IPogenI)
- LinkedIn - [Pogen](https://www.linkedin.com/in/protaya-roy-373022184/)
