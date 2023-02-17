# Frontend Mentor - 3-column preview card component

**Table of Contents**

## Welcome! 👋

Welcome to my solution page. I hope you'll find some good implemantions for this project here.

![3-column preview card component](./design/desktop-preview.jpg)

## Links

- [My Live Site](My-live-site-in-github.io)

- [My Solution Page](https://www.frontendmentor.io/solutions/fem4threecolumnpreviewcardcomponentv21-themobilefirst-jvW-eAl2Ll)

- [The Challenge Page](https://www.frontendmentor.io/challenges/3column-preview-card-component-pH92eAR2-)

## Overview

<!-- ## The Problems and Solutions -->

## My Questions for The Community

> Hi everyone.
>
> I've just finished the project. I got so many experiences here. This really works for us. I tried some modern properties like minmax() for layout but I couldn't use them properly, I'll try them later and I still couldn't solve the shaking problem. I think there are some strange properties in the design file like button's text position or cart positions etc. Should I push myself for that, are these the parts of the hard level challenge? If I push myself for these, my code will become non-readable. I don't want to change my clean version or there is a clear solution somewhere, idk.
>
> I also have a major problem. How can I use the h1 tag on this page? Should I keep the pattern or can I add the h1 tag to some titles? Do I need a hierarchy here?
>
> Thanks.
>
> Any comments, critique, advice is greatly appreciated. For those of you reading this, have a nice day!
>
> (Note: I separated style.css and media-queries.css for easy to read to code. I'll merge them later.)

## Community Feedbacks

1. From Grace Snow:

That is not a problem!!!
There are BIG issues in this solution though. It is not at all responsive and is missing some key semantics
You should not be using position absolute anywhere in this. But especially do not use it to try and place your component on the page. You need to understand what position absolute does - it removes elements from the normal document flow. So this is currently like the body has no content at all.
To center a component on a page, use flex/grid properties along with min-height 100%. The component will need a little bit of margin or the wrapping element a little bit of padding - just so the component cannot hit screen edges
.section-preview-card and the article-cards must not have height. Never limit height on elements containing text. Let the browser decide how tall they need to be.
.section-preview-card and article-cards must not have width. All you need on this is a max-width on the component (or cards) and that changes between desktop/mobile. It must be max-width in order to be properly responsive
The padding looks too much on mobile
You will need to add more margin-top / bottom to increase the space between buttons and paragraph once the heights have been removed.
HTML:
It is generally poor practice to include empty divs in html. And background images are less performant than including images in the html. For those reasons I’d recommend changing the icons to be in the HTML either as img tags or inline svgs. OPTIONAL though, just a recommendation
Whether or not you do that, these icons are decorative so should not have an alt description (or should not have role img or aria-label if on a div)
You must use heading elements not just strong tags

2. From ZMB

Hi,

Nice to complete this challenge, here is a sugessetion for your question about heading;

<strong class="article-card__title">Sedans</strong> <p class="article-card__description"> Choose a sedan for its affordability and excellent fuel economy. Ideal for cruising in the city or on your next road trip. </p>

Replace <strong> with <h1> and you can adjust font-size in css. For further reading please visit the Heading.

I hope this will help you .

Well done and best of luck for the next challenge.

<!-- ## Good Implementations -->

<!-- ## Useful Resources -->

<!-- - [The link title](The link) -->

## Acknowledgments

- Thanks Grace Snow for your helpful comment. [@grace-snow](https://www.frontendmentor.io/profile/grace-snow)

- Thanks ZMB for your helpful comment. [@ZMBAIG](https://www.frontendmentor.io/profile/ZMBAIG)

## Author

- My Frontend Mentor Profile Page - [@adonmez04](https://www.frontendmentor.io/profile/adonmez04)
- For those of you reading this, have a nice day!
