# ChatGPT Images 2.0 — Prompt Gallery

A single-page gallery of all 45 images from OpenAI's [ChatGPT Images 2.0 launch](https://openai.com/index/introducing-chatgpt-images-2-0/), with the original prompts and a direct "Try in ChatGPT" link for each.

## Design decisions (TL;DR)

**Single `index.html`, no build step.** All 45 prompts are embedded directly in JS. No fetch, no CORS, no server — just open the file or push to GitHub Pages.

**Dark mode default.** Warm near-black (`#0e0d0a`) so images read as the primary content, not the chrome.

**Two views, one toggle.** *Grid* is for visual browsing; *Scan* puts a thumbnail on the left and the full prompt text in the remaining space so you can skim all 45 prompts without opening anything.

**Filter by category.** Six categories derived by looking at every image and prompt, not guessing:
- Photography (15) · Comics & Manga (9) · Poster & Ad (10) · Infographic (5) · Editorial (3) · Illustration (3)

**Lightbox with `?id=N` deep links.** Click any image to open a full-size lightbox. The URL updates so individual images are shareable. Arrow keys and Escape work. Filters carry into the lightbox — arrow navigation skips filtered-out items.

**"Try in ChatGPT" via `?q=`** Opens ChatGPT with the prompt pre-filled. No known URL param forces image generation mode; ChatGPT recognizes image prompts automatically.

**Fonts:** Sora (UI) + Source Serif 4 (prompt text) via Google Fonts.

## Notes

All images are AI-generated outputs collected from OpenAI's public announcement. Prompts sourced from `chatgpt-images-2-0-prompts.md`, which mirrors the original blog post credits.
