# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### Screenshot

![Recipe page preview](/assets/images/screenshot.png)

### Links

- Solution URL: [https://github.com/Segarur21/Recipe-page-main](https://github.com/Segarur21/Recipe-page-main)
- Live Site URL: [https://segarur21.github.io/Recipe-page-main/](https://segarur21.github.io/Recipe-page-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Mobile-first workflow
- CSS Table with `border-collapse`

### What I learned

During this challenge, I reinforced clean semantic HTML structure and CSS selectors to handle component dividers without cluttering the markup. 

Specifically, I learned how to style table borders efficiently using native properties:
```css
    .nutrition-table {
      width: 100%;
      border-collapse: collapse;
    }

    .nutrition-table tr:not(:last-child) {
      border-bottom: 1px solid var(--stone-150);
    }
```
I also practiced a Mobile-First approach, keeping the layout fluid on small screens while centering the card with `max-width` and rounded borders on desktop displays:
```css
    @media screen and (min-width: 768px) {
      body {
        display: flex;
        justify-content: center;
        background-color: var(--stone-100);
        padding-block: 10rem;
      }
      .recipe {
        max-width: 73.6rem;
        background-color: var(--white);
        border-radius: 1.6rem;
        padding: 4rem;
      }
    }
```
### AI Collaboration

I used an AI assistant to debug table border behavior without structural hacks, select proper semantic tags, and refine mobile-first CSS architecture. We worked together step-by-step to understand *why* properties like `border-collapse` and `:not(:last-child)` work, resulting in clean code without unnecessary `<div>` bloat or inline overrides.

## Author

- Frontend Mentor - [@Segarur21](https://www.frontendmentor.io/profile/segarur21)
- GitHub - [@Segarur21](https://github.com/segarur21)