<h1 align="center">icon-comparison</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Svelte-5-FF3E00?style=flat-square&logo=svelte&logoColor=white" alt="Svelte 5" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-v4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS v4" />
  <img src="https://img.shields.io/badge/License-MIT-black?style=flat-square" alt="License" />
</p>

<p align="center">
  <strong>Side-by-side comparison of 5 popular Svelte icon libraries.</strong><br/>
  <sub>Visual preview • Import patterns • Bundle info • Brand icon coverage</sub>
</p>

---

## Libraries Compared

| Library | Icons | Brand Icons | Import Pattern | Notes |
|---------|-------|-------------|----------------|-------|
| `@lucide/svelte` | ~1,500+ | No | `Home` | Clean, minimal. Brand icons removed in v1.x |
| `@tabler/icons-svelte` | ~5,800+ | Yes | `IconHome` | Largest free set. 2px stroke default |
| `phosphor-svelte` | ~1,500+ | Yes | `House` | 6 weight variants. Unique naming |
| `svelte-remix` | ~2,800+ | Yes | `HomeLineBuildings` | Verbose naming with category suffix |
| `@hugeicons/svelte` | 5,100+ | Yes | `Home01Icon` | Data-driven. Separate icon data package |

---

## Quick Start

```bash
pnpm install
pnpm dev
```

Opens at [localhost:5555](http://localhost:5555).

---

## Stack

- **SvelteKit 5** with runes mode
- **Tailwind CSS v4** via Vite plugin
- **Dark theme** UI

---

## What It Shows

Each library gets a card displaying:

- **10 common icons** — Home, Search, Settings, Heart, Star, Calendar, Mail, Phone, Camera, ChevronRight
- **5 brand icons** — Instagram, WhatsApp, Github, Twitter/X, TikTok
- **Metadata** — icon count, tree-shakeability, bundle size per icon
- **Import pattern** — how each library names its exports

A summary comparison table at the bottom ties it all together.
