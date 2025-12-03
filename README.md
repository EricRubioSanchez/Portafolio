# Portfolio — README

## Why Astro

This project was built with Astro. It was my first time using Astro and I wanted to try it after hearing it is a very good framework for building fast, component-based static sites. Astro made it easy to combine lightweight components, optimize the output for performance, and keep the development experience simple while producing a small, static dist folder.

## Running the project

### Install dependencies
```bash
# npm or
npm install

```

### Run in development
Starts Astro's dev server with live reload:
```bash
# npm
npm run dev

```
Open http://localhost:4321 (or the port shown in the console).

## Run from the static dist folder
```bash
# npm
npm run preview

```


## Project analysis

This repository contains the source code for a personal portfolio website built with Astro and Tailwind CSS. Its primary purpose is to showcase selected projects, provide an easy way to download the CV, and offer straightforward contact options for potential employers or collaborators. The project prioritizes performance, accessibility, and a consistent experience across mobile and desktop devices. The codebase is organized into reusable components (Header, Hero, Projects, Footer, etc.) and centralized global styles to make maintenance and future updates straightforward.

## Project structure

Project layout and key folders/files:

- public/                — static assets served as-is (images, CV PDF, favicon)
- src/
  - components/          — reusable UI components (Header, Hero, Projects, etc.)
  - layouts/             — page layouts (Layout.astro)
  - pages/               — route pages (index.astro)
  - styles/              — global and Tailwind entry CSS (global.css, tailwind.css)
  - icons/               — SVG/astro icon components
- dist/                  — production build output (generated after build)
- package.json           — scripts and dependencies
- tailwind.config.{js,cjs} — Tailwind configuration (content paths, theme)
- README.md              — this file


## User profile (User Persona)

- Name: Laura Martínez  
- Age: 28  
- Role: Technical recruiter at a tech startup  
- Goals: quickly evaluate a candidate’s experience, review relevant projects, download the CV, and find a direct way to contact the candidate if there is interest.  
- Pain points: slow websites, cluttered portfolios, missing links to demos or source code, and difficulty locating key information on mobile.  
- Technical level: basic to intermediate technical knowledge — expects working demos and GitHub links.  
- Behavior: accesses the portfolio from both mobile and desktop, skims content quickly and decides within seconds whether to continue or reach out.

## Information architecture

The site content is organized in clear, well-defined sections to enable fast scanning and rapid decision-making. The top area contains a fixed Header with anchor navigation pointing to the main sections: Education, Projects and Experience. The Hero section presents the candidate’s name, role, and primary CTAs (download CV and social links) to support immediate actions. The Projects section displays uniform cards that include an image, short description, technology tags, and buttons linking to a live demo or repository. Cards maintain consistent dimensions to preserve visual rhythm and easy comparison.

Experience and Education sections list roles and milestones in chronological order. Technically, each major block is implemented as an independent component to simplify reordering and reuse. Smooth scrolling and anchor-based navigation improve usability; IntersectionObserver highlights the active nav item according to the current viewport position to help users orient themselves. On smaller screens the layout stacks vertically and interactive elements become larger to ensure comfortable tapping. Headings (H1–H3) are used for semantic hierarchy and SEO benefits. Overall, the architecture aims to reduce cognitive load by prioritizing essential information and enabling progressive disclosure of details.

## Visual design

The visual approach combines a deep, dark background with warm accent tones (orange/peach) to create a professional yet personal feel. Typography uses a variable sans-serif that provides flexible weights for strong hierarchy, ensuring legibility on devices of all sizes. Generous spacing, rounded card corners, and soft shadows establish depth and separation without visual clutter. Project images are optimized and cropped to a consistent height to maintain a tidy grid when cards are tiled in columns.

Micro-interactions are subtle but purposeful: buttons scale slightly on hover/focus, background tints transition smoothly, and an animated border around the avatar adds a touch of personality. The UI supports a dark mode variant; colors and shadows adapt to preserve contrast and readability. Accessibility considerations include sufficient color contrast for primary text and action labels, appropriately sized touch targets for mobile users, and ARIA labeling where relevant. The design is responsive and content-first: on narrow viewports the layout focuses on key CTAs and project summaries, while wider screens leverage multi-column layouts to surface more context without sacrificing clarity. Design decisions favor usability and professionalism, balancing visual flair with clarity and speed.

## Links

- Figma (design file): https://www.figma.com/design/T06umencTZacHEvZMrby4u/Hypermedia-project.-Part-1.-Standard-submission?node-id=0-1&t=msYecyqaDlZWooUz-1