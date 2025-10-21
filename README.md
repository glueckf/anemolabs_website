# AnemoLabs Website

A modern, single-page marketing website for AnemoLabs built with Vue 3 and Vite.

## Features

- **Responsive Design**: Fully responsive layout that works on all devices
- **Video Animation**: Intro animation that transitions to the main headline
- **Infinite Tech Carousel**: Smooth scrolling carousel showcasing the tech stack
- **Modern UI**: Clean, professional design following the AnemoLabs brand identity
- **Performance Optimized**: Built with Vite for fast development and optimized builds

## Tech Stack

- **Framework**: Vue 3 (Composition API)
- **Build Tool**: Vite
- **Styling**: CSS with Custom Properties
- **Font**: Figtree (Google Fonts)

## Project Structure

```
anemolabs_website/
├── src/
│   ├── assets/
│   │   ├── images/         # Images (trees.jpeg, founders.jpg)
│   │   ├── logos/          # SVG logos for tech stack and company
│   │   ├── videos/         # Logo animation video
│   │   └── styles/
│   │       └── main.css    # Global styles and brand identity
│   ├── components/
│   │   ├── TheHeader.vue           # Fixed header with logo
│   │   ├── LandingSection.vue      # Hero section with video
│   │   ├── WhatWeDoSection.vue     # Services overview
│   │   ├── TechCarousel.vue        # Infinite scrolling tech logos
│   │   ├── AboutUsSection.vue      # Team information
│   │   ├── ProjectsSection.vue     # Current projects
│   │   ├── ContactSection.vue      # Contact information
│   │   └── TheFooter.vue           # Footer with links
│   ├── App.vue             # Main application component
│   └── main.js             # Application entry point
├── index.html
├── vite.config.js
└── package.json
```

## Development

### Install Dependencies

```bash
npm install
```

### Run Development Server

```bash
npm run dev
```

The site will be available at `http://localhost:5173/`

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## Brand Identity

### Color Palette

- **Dark Primary**: `#183132`
- **Dark Secondary**: `#004D43`
- **Light Primary**: `#EBFFF5`
- **Accent**: `#D0FF71`
- **White**: `#FFFFFF`

### Typography

- **Font Family**: Figtree
- **Weights**: 300 (Light), 400 (Regular), 600 (Semibold)

## Sections

1. **Landing Section**: Full-screen hero with animated logo introduction
2. **What We Do**: Overview of services and approach
3. **About Us**: Team information and company background
4. **Projects**: Current projects and developments
5. **Contact**: Contact information and social links

## Contact

- **Email**: info@anemolabs.de
- **Location**: Berlin, Germany
- **LinkedIn**: [AnemoLabs](https://linkedin.com/company/anemolabs)
- **GitHub**: [AnemoLabs](https://github.com/anemolabs)

---

© 2025 AnemoLabs
