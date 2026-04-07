# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm install      # Install dependencies
npm run dev      # Start dev server at http://localhost:5173
npm run build    # Production build
npm run lint     # Run ESLint
npm run preview  # Preview production build
```

## Architecture

This is a single-page React app (Vite + React 19) with all logic in `src/App.jsx`. There is no routing, no backend, and no persistence — state lives entirely in React `useState`.

**Known issues (intentional, part of a course):**
- Bug: `amount` is stored as a string, so arithmetic on totals is broken (string concatenation instead of addition)
- UI needs improvement
- Code is intentionally messy for refactoring exercises
