<div align="center">

# Bihar Bharaman

### Explore the heritage, spirituality, culture, and natural beauty of Bihar.

[![Live Demo](https://img.shields.io/badge/Live_Demo-Vercel-000000?logo=vercel&logoColor=white)](https://bihar-bharaman.vercel.app/)
[![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-5-646CFF?logo=vite&logoColor=white)](https://vite.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3-06B6D4?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)

[Live Website](https://bihar-bharaman.vercel.app/) · [GitHub Repository](https://github.com/shubhamthakur9771/Bihar-Bharaman-Vibe-Coding)

</div>

---

## Overview

**Bihar Bharaman** is a responsive tourism discovery website designed to introduce visitors to Bihar's historical landmarks, religious destinations, cultural attractions, and natural landscapes.

The application presents 15 destinations with dedicated detail pages, destination categories, photographs, historical descriptions, visitor information, and practical travel guidance. It is built as a modern single-page React application and deployed on Vercel.

<div align="center">

![Bihar Bharaman — Bihar tourism destination](src/assets/hero-bihar.jpg)

<sub>Hero image used by the application</sub>

</div>

## Live Preview

<div align="center">

**[Visit Bihar Bharaman →](https://bihar-bharaman.vercel.app/)**

</div>

## Features

### Destination Discovery
- Explore a curated collection of 15 destinations across Bihar.
- Browse destinations through image-led cards.
- Filter places by category: Religious, Historical, Cultural, and Nature.
- View each destination's location and short introduction.

### Destination Detail Pages
Each destination has a dedicated route with:
- Detailed destination description
- Key highlights and attractions
- Recommended time of year to visit
- Visiting timings
- Entry-fee information
- Directions and nearby connectivity information
- Links to discover other destinations

### Bihar Travel Guide
The homepage also includes:
- An introduction to Bihar's history and cultural significance
- Highlights covering heritage, spirituality, nature, and living culture
- General travel-planning tips
- Information about climate, transport, and local cuisine

### Responsive User Experience
- Responsive navigation with a mobile menu
- Layouts designed for desktop, tablet, and mobile screens
- Animated page sections and destination cards
- Smooth visual transitions and image overlays

## Destinations Covered

The destination data is maintained in `src/data/places.ts`.

| # | Destination | Category |
|---:|---|---|
| 1 | Mahabodhi Temple | Religious |
| 2 | Nalanda University Ruins | Historical |
| 3 | Rajgir | Religious |
| 4 | Vikramshila University | Historical |
| 5 | Vaishali | Historical |
| 6 | Pawapuri | Religious |
| 7 | Patna Sahib (Takht Sri Patna Sahib) | Religious |
| 8 | Mundeshwari Temple | Religious |
| 9 | Kesaria Stupa | Historical |
| 10 | Valmiki Nagar Wildlife Sanctuary | Nature |
| 11 | Sher Shah Suri Tomb | Historical |
| 12 | Darbhanga Raj (Royal Fort & Palace) | Cultural |
| 13 | Kakolat Waterfall | Nature |
| 14 | Patna Museum | Cultural |
| 15 | Golghar | Historical |

## Technology Stack

| Area | Technologies |
|---|---|
| Frontend framework | React 18 |
| Language | TypeScript |
| Build tool and development server | Vite 5 |
| Styling | Tailwind CSS, custom CSS |
| UI components | shadcn/ui patterns, Radix UI |
| Icons | Lucide React |
| Animation | Framer Motion |
| Routing | React Router DOM |
| Server-state utilities | TanStack React Query |
| Forms and validation dependencies | React Hook Form, Zod, Hook Form Resolvers |
| Notifications | Sonner, Radix-based toaster |
| Testing | Vitest, Testing Library, Playwright configuration |
| Deployment | Vercel |

## Application Routes

| Route | Description |
|---|---|
| `/` | Homepage with hero, destination catalogue, about section, and travel guide |
| `/place/:id` | Detail page for a destination identified by its data ID |
| `*` | Not-found page for unmatched routes |

Examples:

```text
/
/place/mahabodhi-temple
/place/nalanda-university
/place/rajgir
```

## Project Structure

```text
Bihar-Bharaman-Vibe-Coding/
│
├── public/
│   ├── favicon.ico
│   ├── placeholder.svg
│   └── robots.txt
│
├── src/
│   ├── assets/
│   │   ├── hero-bihar.jpg
│   │   └── destination images
│   │
│   ├── components/
│   │   ├── ui/
│   │   ├── AboutSection.tsx
│   │   ├── DestinationCard.tsx
│   │   ├── DestinationsSection.tsx
│   │   ├── Footer.tsx
│   │   ├── Hero.tsx
│   │   ├── Navbar.tsx
│   │   └── PlanSection.tsx
│   │
│   ├── data/
│   │   └── places.ts
│   │
│   ├── hooks/
│   ├── lib/
│   ├── pages/
│   │   ├── Index.tsx
│   │   ├── NotFound.tsx
│   │   └── PlaceDetail.tsx
│   │
│   ├── test/
│   ├── App.tsx
│   ├── App.css
│   ├── index.css
│   └── main.tsx
│
├── index.html
├── package.json
├── package-lock.json
├── tailwind.config.ts
├── tsconfig.json
├── vite.config.ts
├── vitest.config.ts
└── README.md
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (LTS recommended)
- npm (included with Node.js)
- Git

Check your installed versions:

```bash
node --version
npm --version
git --version
```

### 1. Clone the repository

```bash
git clone https://github.com/shubhamthakur9771/Bihar-Bharaman-Vibe-Coding.git
cd Bihar-Bharaman-Vibe-Coding
```

### 2. Install dependencies

```bash
npm install
```

The repository includes a `package-lock.json`, so npm can install the dependency versions recorded in the lockfile.

### 3. Start the development server

```bash
npm run dev
```

Vite is configured to use port `8080`. Open the local URL printed in your terminal (normally `http://localhost:8080`).

### 4. Create a production build

```bash
npm run build
```

The generated production files are written to the `dist/` directory.

### 5. Preview the production build locally

```bash
npm run preview
```

## Available Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start the Vite development server |
| `npm run build` | Create a production build |
| `npm run build:dev` | Build using Vite's development mode |
| `npm run preview` | Preview the production build |
| `npm run lint` | Run ESLint |
| `npm run test` | Run the Vitest test suite once |
| `npm run test:watch` | Run Vitest in watch mode |

## Deployment

The application is deployed on **Vercel**.

- **Live website:** [https://bihar-bharaman.vercel.app/](https://bihar-bharaman.vercel.app/)
- **Source repository:** [Bihar-Bharaman-Vibe-Coding](https://github.com/shubhamthakur9771/Bihar-Bharaman-Vibe-Coding)

The project uses Vite's standard production build. The build command is:

```bash
npm run build
```

The output directory is:

```text
dist/
```

For a Vercel project connected to this GitHub repository, pushes to the configured production branch can trigger a new deployment according to the Vercel project's deployment settings.

## Data and Content

Destination content is currently stored locally in `src/data/places.ts`. The application imports destination photographs from `src/assets/` and uses the local data to render the destination cards and detail pages.

**Current scope:** This is an informational tourism discovery website. The supplied source does not include a live booking system, user accounts, a backend API, a database, live transport availability, or an interactive route-planning service. Visitor information is presented as static project content and should be verified independently before travel.

## Future Enhancements

Potential areas to extend the project:

- Search destinations by name, district, or attraction
- Interactive map with destination locations
- Itinerary builder for multi-day trips
- Verified and regularly updated visitor information
- Local food, accommodation, and transport directories
- Multilingual content
- Accessibility improvements and richer destination galleries

## Author

**Shubham Kumar**

- GitHub: [@shubhamthakur9771](https://github.com/shubhamthakur9771)
- Project: [Bihar Bharaman](https://github.com/shubhamthakur9771/Bihar-Bharaman-Vibe-Coding)

---

<div align="center">

**Made with ❤️ to showcase the heritage and beauty of Bihar.**

[Explore Bihar Bharaman](https://bihar-bharaman.vercel.app/)

</div>
