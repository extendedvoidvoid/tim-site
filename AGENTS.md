# AGENTS.md — Tim Site (Théophile Dereux Portfolio)

> Multi-CLI project rules (Grok · Claude · Codex · OpenCode).  
> Global law: `~/.grok/memory/MEMORY.md` · tools: `HARNESS.md`.  
> Setup: say **make pro** in a `~/projects` folder (skill `pro`).

## What this is

Portfolio and interactive book showcase website for Théophile Dereux (text, photos, audio, PDF assets). Hosted on GitHub Pages / Vercel.

## Stack

- **Framework:** Astro / HTML + Tailwind CSS (static site generator)
- **Deployment:** GitHub Pages / Vercel
- **Assets:** PDF source (`Book_Theophile_Dereux_2025_TEXT_edited_edited.pdf`), high-res photos, audio players

## Commands

```bash
npm run dev      # Local dev server
npm run build    # Build static output
npm run preview  # Preview build locally
```

## Agent Roles & Workflow

- **Main Agent (Architect & Dev):** Project layout, Astro components, page routing, styling, git commits.
- **Content Agent (PDF & Asset Extractor):** Extract text, parse structure from PDF book, map images/audio to page sections.
- **UI/UX Agent:** Responsive layouts, image gallery, custom audio player component.

## Rules (thin — grow when agents err)

1. Surgical changes; prefer reuse over rewrite.
2. No secrets in repo (keys → Keychain / `~/.secrets` / env not committed).
3. Keep media optimized (< 100MB Git repo or use LFS/external CDN for heavy audio/photos).
4. Ask before destructive operations or force pushes.

*Created 2026-08-01 by setup_project · minimal pack*
