# CLAUDE.md

## Project Overview

Static slide-based guide site for AI Coding Agent setup (Claude Code + Codex + gstack + Ralph).
Three language versions (KO/EN/JA) with a shared landing page.

## File Structure

```
index.html                      # Landing page — language selector
ai-coding-setup-guide-ko.html   # Korean guide (slide deck)
ai-coding-setup-guide-en.html   # English guide (slide deck)
ai-coding-setup-guide-ja.html   # Japanese guide (slide deck)
images/                         # Slide images
og/                             # Open Graph images
```

## Key Conventions

- **Pure static HTML** — no build step, no framework, no bundler.
- All three guide files share the same slide structure and JS logic. Changes to navigation, styling, or shared behavior must be applied to all three files.
- Slide numbering uses `data-slide` attributes and section labels like `6-1`, `6-2`. When adding/removing slides, renumber subsequent labels accordingly.
- Slide navigation JS is embedded at the bottom of each guide HTML. Key classes: `setupKeyboardNav()`, `setupWheelNav()`, `setupTouchNav()`.
- Navigation mappings: ArrowRight/ArrowDown/Space/PageDown = next, ArrowLeft/ArrowUp/PageUp = prev.
- Mouse wheel uses delta accumulation (threshold 50, cooldown 300ms).

## Deployment

Hosted on **Vercel** under the `querypie` team.

```bash
vercel --prod --scope querypie
```

- Project name: `ai-coding-guide-with-gstack`
- Production URL: https://ai-coding-guide-with-gstack.vercel.app
- No build command — Vercel serves static files directly.
- Deploy after every change; takes ~7 seconds.

## Editing Guidelines

- When adding links, use `target="_blank"` and style with `color:var(--accent-light); text-decoration:none;`.
- GitHub reference links use the pattern:
  ```html
  <p class="reveal" style="margin-top:clamp(0.5rem,1vw,0.8rem); font-size:var(--small-size); color:var(--text-tertiary);">
      GitHub: <a href="https://..." target="_blank" style="color:var(--accent-light); text-decoration:none;">github.com/...</a>
  </p>
  ```
- Always apply the same change to all three language files (ko, en, ja).
