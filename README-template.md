# Frontend Mentor - Testimonials grid section solution

### Design preview for the Testimonials grid section solution coding challenge

| Desktop Version                                  | Mobile Version                                 |
| :----------------------------------------------- | :--------------------------------------------- |
| ![Desktop Screenshot](design/desktop-design.jpg) | ![Mobile Screenshot](design/mobile-design.jpg) |

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [AI Collaboration](#ai-collaboration)
- [Open for Opportunities & Collaboration](#open-for-opportunities--collaboration)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page


### Screenshots

|              Desktop View              |              Mobile View 1              |              Mobile View 2              |
| :------------------------------------: | :-------------------------------------: | :-------------------------------------: |
| ![Desktop](images/desktop-version.png) | ![Mobile 1](images/mobile-version1.jpg) | ![Mobile 2](images/mobile-version2.jpg) | 

### Links

- Solution URL: [GitHub Repository](https://github.com/naftalmambo/single-price-grid-component)
- Live Site URL: [Live Demo](https://naftalmambo.github.io/single-price-grid-component/)

## My process

### Built with

- **Semantic HTML5 markup**
- **CSS custom properties**
- **Grid**
- **Flexbox**
- **Mobile-first workflow**
- **Google Fonts (Figtree)**
- **VS Code** - My primary editor for writing clean, structured code.
- **Linux (Ubuntu/WSL)** - My development environment for a professional, stable workflow.
- **Windows Browser (Chrome)** - Used for cross-browser testing to ensure its responsive.

### What I learned from this work

This project was a major milestone in my journey toward mastering responsive layouts and web accessibility. Here are the key technical concepts I mastered:

#### **1. Mastering "Stretch" for Full-Width Backgrounds**

I learned that when using `flex-direction: column`, children often shrink to fit their content width. By using **`align-items: stretch`**, I ensured that the background colors for the Pricing and Features sections filled the entire card width, removing unwanted white gaps.

```css
.price-component {
  display: flex;
  flex-direction: column;
  /* Learned: This forces colored sections to fill the full width of the card */
  align-items: stretch;
}
```

#### **2. Perfecting Corners with `overflow: hidden`**

- I learned how to use overflow: hidden on a parent container to manage child element clipping. This allowed the internal sections to have distinct background colors while still respecting the card's overall border-radius, creating a much more polished UI.

```css
.price-component {
  border-radius: 8px;
  overflow: hidden;
}
```

#### **3. Responsive "T-Shaped" Grid Layout**

I learned how to use CSS Grid to transform a vertical frame into T-shaped layout. By defining a two-column grid and using the `span` property, I was able to make the introductory section stretch across the top while the pricing and features sections aligned side by side.

```css
@media (min-width: 40rem) {
  .price-component {
    display: grid;
    grid-template-columns: 1fr 1fr; /* Two equal columns */
  }

  .section-intro {
    /* Learned: This spans the top section across both columns for the "T" shape */
    grid-column: span 2;
  }
}
```

### Continued development

In future work, I intend to focus on:

- **Responsiveness:** I believe I've tried my best to make this project as responsive as possible through use of mobile-first approach, while also open to improvements.

### AI Collaborationices.

- **Tools Used:** Google AI.

Throughout this project, I used an AI-collaborative workflow to:

- **Refine Logic:** Instead of just copying code, I used AI to explain "why" certain properties like `align-items: stretch` were necessary.
- **Master Best Practices:** I learned to implement professional standards such as **REM units**, **semantic HTML**.
- **Debugging & Polish:** I collaborated with AI to solve specific UI bugs (like the rounded corner clipping issue) and to perfect micro-interactions like the button "shrink" effect.

## Open for Opportunities & Collaboration

This project marks the beginning of my journey toward becoming a professional Web Developer and ultimately a Java Full-Stack. I am currently:

- 🔭 **Open for work:** Looking for junior roles or freelance opportunities where I can apply my skills in HTML, CSS, and Javascript(in-progress).
- 🤝 **Open to contribute:** Interested in collaborating on open-source projects or team-based challenges.

If you like what you see or have a project you need help with, connect with:

**Author**

- Frontend Mentor - [@naftalmambo](https://frontendmentor.io)
- LinkedIn - [Naftal Mambo](https://linkedin.com)
- GitHub - [@naftalmambo](https://github.com)
- Discord - [devMambo](https://discordapp.com/users/1157321092482994246)

## Acknowledgments

### 🌟 Appreciation for Frontend Mentor

I want to express my sincere gratitude to **[Frontend Mentor](https://www.frontendmentor.io)** for providing these incredible, real-world challenges that I am sure will enable me to grow to be the developer I aspire.

This platform will be more than just a place to practice, it will be a gateway to building skills that truly **change lives**.

By bridging the gap between theory and professional workflows, Frontend Mentor will help me build a rock-solid skill for a future where I can create meaningful digital solutions.

## Credits

While this is a [Frontend Mentor](https://www.frontendmentor.io) challenge, the structural and styling knowledge used to build it was gained through;

- **freeCodeCamp**: For the consistent interactive practice that solidified my HTML and CSS fundamentals.
- **The Odin Project**: For teaching me how to set up my local working environment and to think like a developer.
