# Flaur Landing Page

Flaur is an Astro-based landing page for an AI-first investment education product.  
This project is optimized for static deployment and uses locally bundled image assets in `public/images` for production reliability.

## Tech Stack

- Astro 6
- Vanilla CSS (`src/styles/global.css`)
- Static assets served from `public/images`

## Project Structure

```text
.
├── public/
│   └── images/              # Localized visual assets used by the UI
├── src/
│   ├── layouts/
│   │   └── BaseLayout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## Getting Started

### Prerequisites

- Node.js 18+ (recommended: latest LTS)
- npm

### Install

```bash
npm install
```

### Run Locally

```bash
npm run dev
```

Open `http://localhost:4321`.

### Build for Production

```bash
npm run build
```

Build output is generated in `dist/`.

### Preview Production Build

```bash
npm run preview
```

## Production Notes

- All images are local files under `public/images` (no runtime Figma MCP dependency).
- The site is static and suitable for CDN hosting (Netlify, Vercel static output, Cloudflare Pages, S3 + CloudFront, etc.).

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Create static production build
- `npm run preview` - Preview built site locally

## License

This project is licensed under the Apache License 2.0.  
See [LICENSE](./LICENSE).

