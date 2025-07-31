# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

- **Start development server**: `npm run dev` (runs with Turbopack for faster builds)
- **Build for production**: `npm run build`
- **Start production server**: `npm start`
- **Lint code**: `npm run lint`

## Project Architecture

This is a Next.js 15 application using the App Router architecture with TypeScript and Tailwind CSS.

### Key Structure
- **App Router**: Uses `src/app/` directory structure with `layout.tsx` and `page.tsx`
- **TypeScript**: Configured with strict mode and path aliases (`@/*` maps to `./src/*`)
- **Styling**: Tailwind CSS 4 with custom font configuration (Geist Sans and Geist Mono)
- **Optimization**: Uses `next/font` for automatic font optimization and `next/image` for image optimization

### Important Files
- **Root Layout**: `src/app/layout.tsx` - Defines global HTML structure and font loading
- **Home Page**: `src/app/page.tsx` - Main landing page component
- **Global Styles**: `src/app/globals.css` - Global CSS and Tailwind directives
- **TypeScript Config**: Path aliases configured for `@/*` imports

### Development Notes
- Uses React 19 and Next.js 15 with latest features
- Turbopack enabled for faster development builds
- ESLint configured with Next.js recommended rules
- PostCSS configured for Tailwind CSS processing