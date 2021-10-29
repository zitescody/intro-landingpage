# intro-landingpage
From Frontend Mentor. Simple landing page coded in HTML and CSS

# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

Users should be able to:

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![Desktop](https://user-images.githubusercontent.com/49009141/139499226-fe68b108-c695-49c0-84bc-43f4c6c0e227.png)

![Mobile](https://user-images.githubusercontent.com/49009141/139499204-26cefc60-7b30-4b4d-b44b-ce3742027630.png)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Soution File](https://github.com/zitescody/intro-landingpage)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Media Queries
- CSS Grid


### What I learned

I learned principles of CSS Grid and Media Queries:


CSS Grid
```css
/* Grid Styles */
div.col-1 {
    grid-area: one;
}

div.col-2 {
    grid-area: two;
    justify-self: center;
}

div.col-3 {
    grid-area: three;
    justify-self: center;
    align-self: end;
    margin-top: 10%;
}

div.col-4 {
    grid-area: four;
    justify-self: center;
    margin-top: 5%;
}
 
div.container {
    display: grid;
    grid-template-columns: [first] 5% [second] 90% [third] 5% [end];
    grid-template-rows: [first] 10% [second] 30% [third] 50% [fourth] 10% [end];
    grid-template-areas: 
        ". one ."
        ". two ."
        ". three ."
        ". four ."
    ;
}
```

Media Query
```css
/* Media Query (>1200px) */
@media (min-width: 1200px) {
    div.col-1 {
        margin-top: 5%;
    }
    div.col-2 {
        align-self: center;
        justify-self: start;
        margin-top: 5%;
    }

    div.col-3 {
        align-self: center;
        justify-self: center;
        margin-left: 5%;
        margin-top: 5%;
    }

    div.col-4 {
        justify-self: end;
    }
    div.container {
        display: grid;
        grid-template-columns: [first] 5% [second] 49.5% [third] 40.5% [fourth] 5% [end];
        grid-template-rows: [first] 10% [second] 30% [third] 50% [fourth] 10% [end];
        grid-template-areas: 
        ". one . ."
        ". two three ."
        ". two three ."
        ". . four ."
        ;
    }

    h1.title {
        text-align: start;
        font-size: 36pt;
    }

    p.content {
        text-align: start;
        font-size: 16pt;
    }

    button.btn {
        margin: 0;
        
    }

    ion-icon {
        width: 50px;
        height: 50px;
    }
}
```
### Continued development

This is my second project with responsive and mobile-first web design. I used CSS grid and media queries to complete this project. I want to learn more about how to incorporate JS into this.

### Useful resources

- [CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) - Assisted in grasping concepts of basic CSS grids.
- [Media Queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries) - Helped with setting up project for mobile-first responsive web design.

## Author

- Website - [Cody Zites](https://github.com/zitescody)
- Frontend Mentor - [zitecody](https://www.frontendmentor.io/profile/zitescody)

## Acknowledgements

Facebook and Twitter icon made by Stockio from www.flaticon.com
Instagram icons made by Freepik from www.flaticon.com
